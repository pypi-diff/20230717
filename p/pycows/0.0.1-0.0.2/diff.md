# Comparing `tmp/pycows-0.0.1.tar.gz` & `tmp/pycows-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycows-0.0.1.tar", last modified: Wed Jan 12 09:25:22 2022, max compression
+gzip compressed data, was "pycows-0.0.2.tar", last modified: Mon Jul 17 14:16:12 2023, max compression
```

## Comparing `pycows-0.0.1.tar` & `pycows-0.0.2.tar`

### file list

```diff
@@ -1,94 +1,57 @@
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.113064 pycows-0.0.1/
--rw-r--r--   0 spfeifer   (501) staff       (20)      149 2022-01-04 11:00:06.000000 pycows-0.0.1/.coveragerc
--rw-r--r--   0 spfeifer   (501) staff       (20)      231 2022-01-04 11:00:06.000000 pycows-0.0.1/.readthedocs.yml
--rw-r--r--   0 spfeifer   (501) staff       (20)     3393 2022-01-07 11:29:42.000000 pycows-0.0.1/LICENSE.txt
--rw-r--r--   0 spfeifer   (501) staff       (20)      197 2022-01-05 16:31:11.000000 pycows-0.0.1/MANIFEST.in
--rw-r--r--   0 spfeifer   (501) staff       (20)     2397 2022-01-12 09:25:22.112783 pycows-0.0.1/PKG-INFO
--rw-r--r--   0 spfeifer   (501) staff       (20)     1796 2022-01-12 08:53:19.000000 pycows-0.0.1/README.rst
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.029633 pycows-0.0.1/ci/
--rw-r--r--   0 spfeifer   (501) staff       (20)     6148 2022-01-10 17:24:03.000000 pycows-0.0.1/ci/.DS_Store
--rwxr-xr-x   0 spfeifer   (501) staff       (20)     3062 2022-01-04 10:48:52.000000 pycows-0.0.1/ci/bootstrap.py
--rw-r--r--   0 spfeifer   (501) staff       (20)       66 2022-01-10 15:09:21.000000 pycows-0.0.1/ci/requirements.txt
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.030953 pycows-0.0.1/ci/templates/
--rw-r--r--   0 spfeifer   (501) staff       (20)     6148 2022-01-10 17:24:03.000000 pycows-0.0.1/ci/templates/.DS_Store
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.018334 pycows-0.0.1/ci/templates/.github/
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.031862 pycows-0.0.1/ci/templates/.github/workflows/
--rw-r--r--   0 spfeifer   (501) staff       (20)     2001 2022-01-04 10:48:52.000000 pycows-0.0.1/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.048593 pycows-0.0.1/docs/
--rw-r--r--   0 spfeifer   (501) staff       (20)     6148 2022-01-10 08:34:17.000000 pycows-0.0.1/docs/.DS_Store
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.049673 pycows-0.0.1/docs/.ipynb_checkpoints/
--rw-r--r--   0 spfeifer   (501) staff       (20)    33019 2022-01-10 18:12:46.000000 pycows-0.0.1/docs/.ipynb_checkpoints/example-checkpoint.ipynb
--rw-r--r--   0 spfeifer   (501) staff       (20)      175 2022-01-07 13:27:08.000000 pycows-0.0.1/docs/api.rst
--rw-r--r--   0 spfeifer   (501) staff       (20)     1309 2022-01-12 08:53:19.000000 pycows-0.0.1/docs/conf.py
--rw-r--r--   0 spfeifer   (501) staff       (20)      103 2022-01-07 13:32:29.000000 pycows-0.0.1/docs/cows.find_filaments.rst
--rw-r--r--   0 spfeifer   (501) staff       (20)      100 2022-01-07 13:32:29.000000 pycows-0.0.1/docs/cows.gen_catalogue.rst
--rw-r--r--   0 spfeifer   (501) staff       (20)      103 2022-01-07 13:32:29.000000 pycows-0.0.1/docs/cows.label_skeleton.rst
--rw-r--r--   0 spfeifer   (501) staff       (20)      112 2022-01-07 13:32:29.000000 pycows-0.0.1/docs/cows.separate_skeleton.rst
--rw-r--r--   0 spfeifer   (501) staff       (20)       92 2022-01-07 13:32:29.000000 pycows-0.0.1/docs/cows.skeletonize.rst
--rw-r--r--   0 spfeifer   (501) staff       (20)    33019 2022-01-10 18:12:46.000000 pycows-0.0.1/docs/example.ipynb
--rw-r--r--   0 spfeifer   (501) staff       (20)     2661 2022-01-10 18:12:56.000000 pycows-0.0.1/docs/example.py
--rw-r--r--   0 spfeifer   (501) staff       (20)      846 2022-01-10 10:56:02.000000 pycows-0.0.1/docs/index.rst
--rw-r--r--   0 spfeifer   (501) staff       (20)       32 2022-01-07 12:01:25.000000 pycows-0.0.1/docs/installation.rst
--rw-r--r--   0 spfeifer   (501) staff       (20)       53 2022-01-07 11:25:53.000000 pycows-0.0.1/docs/license.rst
--rw-r--r--   0 spfeifer   (501) staff       (20)       42 2022-01-12 09:10:29.000000 pycows-0.0.1/docs/requirements.txt
--rw-r--r--   0 spfeifer   (501) staff       (20)      109 2022-01-04 11:00:06.000000 pycows-0.0.1/docs/spelling_wordlist.txt
--rw-r--r--   0 spfeifer   (501) staff       (20)      199 2022-01-10 08:33:31.000000 pycows-0.0.1/docs/usage.rst
--rw-r--r--   0 spfeifer   (501) staff       (20)       38 2022-01-12 09:25:22.113157 pycows-0.0.1/setup.cfg
--rwxr-xr-x   0 spfeifer   (501) staff       (20)     5437 2022-01-12 08:53:19.000000 pycows-0.0.1/setup.py
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.051756 pycows-0.0.1/src/
--rw-r--r--   0 spfeifer   (501) staff       (20)     6148 2022-01-05 15:46:59.000000 pycows-0.0.1/src/.DS_Store
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.070057 pycows-0.0.1/src/cows/
--rw-r--r--   0 spfeifer   (501) staff       (20)     6148 2022-01-07 13:19:12.000000 pycows-0.0.1/src/cows/.DS_Store
--rw-r--r--   0 spfeifer   (501) staff       (20)      168 2022-01-12 08:54:20.000000 pycows-0.0.1/src/cows/__init__.py
--rw-r--r--   0 spfeifer   (501) staff       (20)   852230 2022-01-10 11:56:28.000000 pycows-0.0.1/src/cows/_filament.c
--rw-r--r--   0 spfeifer   (501) staff       (20)     9591 2022-01-10 11:55:55.000000 pycows-0.0.1/src/cows/_filament.pyx
--rw-r--r--   0 spfeifer   (501) staff       (20)  1102219 2022-01-12 08:45:31.000000 pycows-0.0.1/src/cows/_skeletonize_3d_cy.cpp
--rw-r--r--   0 spfeifer   (501) staff       (20)    24058 2022-01-10 10:51:31.000000 pycows-0.0.1/src/cows/_skeletonize_3d_cy.pyx
--rw-r--r--   0 spfeifer   (501) staff       (20)     2382 2022-01-06 12:56:57.000000 pycows-0.0.1/src/cows/arraycrop.py
--rw-r--r--   0 spfeifer   (501) staff       (20)     3575 2022-01-10 14:00:11.000000 pycows-0.0.1/src/cows/catalogue.py
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.078338 pycows-0.0.1/src/cows/cows.egg-info/
--rw-r--r--   0 spfeifer   (501) staff       (20)     2576 2022-01-10 08:54:23.000000 pycows-0.0.1/src/cows/cows.egg-info/PKG-INFO
--rw-r--r--   0 spfeifer   (501) staff       (20)      938 2022-01-10 08:54:23.000000 pycows-0.0.1/src/cows/cows.egg-info/SOURCES.txt
--rw-r--r--   0 spfeifer   (501) staff       (20)        1 2022-01-10 08:54:23.000000 pycows-0.0.1/src/cows/cows.egg-info/dependency_links.txt
--rw-r--r--   0 spfeifer   (501) staff       (20)        1 2022-01-10 08:49:04.000000 pycows-0.0.1/src/cows/cows.egg-info/not-zip-safe
--rw-r--r--   0 spfeifer   (501) staff       (20)       11 2022-01-10 08:54:23.000000 pycows-0.0.1/src/cows/cows.egg-info/top_level.txt
--rw-r--r--   0 spfeifer   (501) staff       (20)    17710 2022-01-06 12:57:07.000000 pycows-0.0.1/src/cows/dtype.py
--rw-r--r--   0 spfeifer   (501) staff       (20)     2840 2022-01-10 13:33:22.000000 pycows-0.0.1/src/cows/filament.py
--rw-r--r--   0 spfeifer   (501) staff       (20)     2868 2022-01-06 12:57:12.000000 pycows-0.0.1/src/cows/skeletonize.py
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.073905 pycows-0.0.1/src/cows.egg-info/
--rw-r--r--   0 spfeifer   (501) staff       (20)     2384 2022-01-10 17:42:21.000000 pycows-0.0.1/src/cows.egg-info/PKG-INFO
--rw-r--r--   0 spfeifer   (501) staff       (20)     2011 2022-01-10 17:42:21.000000 pycows-0.0.1/src/cows.egg-info/SOURCES.txt
--rw-r--r--   0 spfeifer   (501) staff       (20)        1 2022-01-10 17:42:21.000000 pycows-0.0.1/src/cows.egg-info/dependency_links.txt
--rw-r--r--   0 spfeifer   (501) staff       (20)        1 2022-01-05 15:34:52.000000 pycows-0.0.1/src/cows.egg-info/not-zip-safe
--rw-r--r--   0 spfeifer   (501) staff       (20)        5 2022-01-10 17:42:21.000000 pycows-0.0.1/src/cows.egg-info/top_level.txt
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.081185 pycows-0.0.1/src/pycows.egg-info/
--rw-r--r--   0 spfeifer   (501) staff       (20)     2397 2022-01-12 09:25:21.000000 pycows-0.0.1/src/pycows.egg-info/PKG-INFO
--rw-r--r--   0 spfeifer   (501) staff       (20)     2245 2022-01-12 09:25:21.000000 pycows-0.0.1/src/pycows.egg-info/SOURCES.txt
--rw-r--r--   0 spfeifer   (501) staff       (20)        1 2022-01-12 09:25:21.000000 pycows-0.0.1/src/pycows.egg-info/dependency_links.txt
--rw-r--r--   0 spfeifer   (501) staff       (20)        1 2022-01-10 17:49:10.000000 pycows-0.0.1/src/pycows.egg-info/not-zip-safe
--rw-r--r--   0 spfeifer   (501) staff       (20)        5 2022-01-12 09:25:21.000000 pycows-0.0.1/src/pycows.egg-info/top_level.txt
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.095647 pycows-0.0.1/tests/
--rw-r--r--   0 spfeifer   (501) staff       (20)     6148 2022-01-10 14:48:13.000000 pycows-0.0.1/tests/.DS_Store
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.096749 pycows-0.0.1/tests/reports/
--rw-r--r--   0 spfeifer   (501) staff       (20)     6148 2022-01-10 14:48:08.000000 pycows-0.0.1/tests/reports/.DS_Store
-drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2022-01-12 09:25:22.111918 pycows-0.0.1/tests/reports/coverage-html/
--rw-r--r--   0 spfeifer   (501) staff       (20)       27 2022-01-10 10:35:46.000000 pycows-0.0.1/tests/reports/coverage-html/.gitignore
--rw-r--r--   0 spfeifer   (501) staff       (20)    19770 2022-01-10 14:48:54.000000 pycows-0.0.1/tests/reports/coverage-html/coverage_html.js
--rw-r--r--   0 spfeifer   (501) staff       (20)     4472 2022-01-10 10:35:46.000000 pycows-0.0.1/tests/reports/coverage-html/d_b36689deeda1f735___init___py.html
--rw-r--r--   0 spfeifer   (501) staff       (20)    20981 2022-01-10 13:01:01.000000 pycows-0.0.1/tests/reports/coverage-html/d_b36689deeda1f735_arraycrop_py.html
--rw-r--r--   0 spfeifer   (501) staff       (20)    31472 2022-01-10 14:02:31.000000 pycows-0.0.1/tests/reports/coverage-html/d_b36689deeda1f735_catalogue_py.html
--rw-r--r--   0 spfeifer   (501) staff       (20)   138436 2022-01-10 10:35:46.000000 pycows-0.0.1/tests/reports/coverage-html/d_b36689deeda1f735_dtype_py.html
--rw-r--r--   0 spfeifer   (501) staff       (20)    23116 2022-01-10 13:38:45.000000 pycows-0.0.1/tests/reports/coverage-html/d_b36689deeda1f735_filament_py.html
--rw-r--r--   0 spfeifer   (501) staff       (20)    22547 2022-01-10 10:43:17.000000 pycows-0.0.1/tests/reports/coverage-html/d_b36689deeda1f735_skeletonize_py.html
--rw-r--r--   0 spfeifer   (501) staff       (20)     1732 2022-01-10 14:48:54.000000 pycows-0.0.1/tests/reports/coverage-html/favicon_32.png
--rw-r--r--   0 spfeifer   (501) staff       (20)     5391 2022-01-10 14:48:54.000000 pycows-0.0.1/tests/reports/coverage-html/index.html
--rw-r--r--   0 spfeifer   (501) staff       (20)     9004 2022-01-10 14:48:54.000000 pycows-0.0.1/tests/reports/coverage-html/keybd_closed.png
--rw-r--r--   0 spfeifer   (501) staff       (20)     9003 2022-01-10 14:48:54.000000 pycows-0.0.1/tests/reports/coverage-html/keybd_open.png
--rw-r--r--   0 spfeifer   (501) staff       (20)     1559 2022-01-10 14:48:54.000000 pycows-0.0.1/tests/reports/coverage-html/status.json
--rw-r--r--   0 spfeifer   (501) staff       (20)    12278 2022-01-10 14:48:54.000000 pycows-0.0.1/tests/reports/coverage-html/style.css
--rw-r--r--   0 spfeifer   (501) staff       (20)     1690 2022-01-10 13:07:55.000000 pycows-0.0.1/tests/test_arraycrop.py
--rw-r--r--   0 spfeifer   (501) staff       (20)     5397 2022-01-10 14:23:21.000000 pycows-0.0.1/tests/test_catalogue.py
--rw-r--r--   0 spfeifer   (501) staff       (20)  2097232 2022-01-07 15:34:03.000000 pycows-0.0.1/tests/test_data.npy
--rw-r--r--   0 spfeifer   (501) staff       (20)     9587 2022-01-10 13:37:12.000000 pycows-0.0.1/tests/test_filament.py
--rw-r--r--   0 spfeifer   (501) staff       (20)     2689 2022-01-10 11:01:24.000000 pycows-0.0.1/tests/test_skeletonize.py
--rw-r--r--   0 spfeifer   (501) staff       (20)     3273 2022-01-12 08:49:32.000000 pycows-0.0.1/tox.ini
+drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2023-07-17 14:16:12.900740 pycows-0.0.2/
+-rw-r--r--   0 spfeifer   (501) staff       (20)      149 2023-07-17 13:03:15.000000 pycows-0.0.2/.coveragerc
+-rw-r--r--   0 spfeifer   (501) staff       (20)      231 2023-07-17 13:03:15.000000 pycows-0.0.2/.readthedocs.yml
+-rw-r--r--   0 spfeifer   (501) staff       (20)     3393 2023-07-17 13:03:15.000000 pycows-0.0.2/LICENSE.txt
+-rw-r--r--   0 spfeifer   (501) staff       (20)      197 2023-07-17 13:03:15.000000 pycows-0.0.2/MANIFEST.in
+-rw-r--r--   0 spfeifer   (501) staff       (20)     2305 2023-07-17 14:16:12.900281 pycows-0.0.2/PKG-INFO
+-rw-r--r--   0 spfeifer   (501) staff       (20)     2014 2023-07-17 14:12:28.000000 pycows-0.0.2/README.rst
+drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2023-07-17 14:16:12.869100 pycows-0.0.2/ci/
+-rwxr-xr-x   0 spfeifer   (501) staff       (20)     3062 2023-07-17 13:03:15.000000 pycows-0.0.2/ci/bootstrap.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)       66 2023-07-17 13:03:15.000000 pycows-0.0.2/ci/requirements.txt
+drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2023-07-17 14:16:12.864788 pycows-0.0.2/ci/templates/
+drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2023-07-17 14:16:12.864989 pycows-0.0.2/ci/templates/.github/
+drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2023-07-17 14:16:12.869589 pycows-0.0.2/ci/templates/.github/workflows/
+-rw-r--r--   0 spfeifer   (501) staff       (20)     2001 2023-07-17 13:03:15.000000 pycows-0.0.2/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2023-07-17 14:16:12.878373 pycows-0.0.2/docs/
+-rw-r--r--   0 spfeifer   (501) staff       (20)      175 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/api.rst
+-rw-r--r--   0 spfeifer   (501) staff       (20)     1309 2023-07-17 14:12:28.000000 pycows-0.0.2/docs/conf.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)      103 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/cows.find_filaments.rst
+-rw-r--r--   0 spfeifer   (501) staff       (20)      100 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/cows.gen_catalogue.rst
+-rw-r--r--   0 spfeifer   (501) staff       (20)      103 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/cows.label_skeleton.rst
+-rw-r--r--   0 spfeifer   (501) staff       (20)      112 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/cows.separate_skeleton.rst
+-rw-r--r--   0 spfeifer   (501) staff       (20)       92 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/cows.skeletonize.rst
+-rw-r--r--   0 spfeifer   (501) staff       (20)    33019 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/example.ipynb
+-rw-r--r--   0 spfeifer   (501) staff       (20)     2661 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/example.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)     1014 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/index.rst
+-rw-r--r--   0 spfeifer   (501) staff       (20)       32 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/installation.rst
+-rw-r--r--   0 spfeifer   (501) staff       (20)       53 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/license.rst
+-rw-r--r--   0 spfeifer   (501) staff       (20)       42 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/requirements.txt
+-rw-r--r--   0 spfeifer   (501) staff       (20)      109 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 spfeifer   (501) staff       (20)      199 2023-07-17 13:03:15.000000 pycows-0.0.2/docs/usage.rst
+-rw-r--r--   0 spfeifer   (501) staff       (20)       38 2023-07-17 14:16:12.901001 pycows-0.0.2/setup.cfg
+-rwxr-xr-x   0 spfeifer   (501) staff       (20)     5437 2023-07-17 14:12:28.000000 pycows-0.0.2/setup.py
+drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2023-07-17 14:16:12.865628 pycows-0.0.2/src/
+drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2023-07-17 14:16:12.888455 pycows-0.0.2/src/cows/
+-rw-r--r--   0 spfeifer   (501) staff       (20)      169 2023-07-17 14:12:28.000000 pycows-0.0.2/src/cows/__init__.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)   852230 2023-07-17 13:03:15.000000 pycows-0.0.2/src/cows/_filament.c
+-rw-r--r--   0 spfeifer   (501) staff       (20)     9591 2023-07-17 13:03:15.000000 pycows-0.0.2/src/cows/_filament.pyx
+-rw-r--r--   0 spfeifer   (501) staff       (20)  1102219 2023-07-17 13:03:15.000000 pycows-0.0.2/src/cows/_skeletonize_3d_cy.cpp
+-rw-r--r--   0 spfeifer   (501) staff       (20)    24058 2023-07-17 13:03:15.000000 pycows-0.0.2/src/cows/_skeletonize_3d_cy.pyx
+-rw-r--r--   0 spfeifer   (501) staff       (20)     2382 2023-07-17 13:03:15.000000 pycows-0.0.2/src/cows/arraycrop.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)     3724 2023-07-17 13:03:15.000000 pycows-0.0.2/src/cows/catalogue.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)    17710 2023-07-17 13:03:15.000000 pycows-0.0.2/src/cows/dtype.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)     2840 2023-07-17 13:03:15.000000 pycows-0.0.2/src/cows/filament.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)     2868 2023-07-17 13:03:15.000000 pycows-0.0.2/src/cows/skeletonize.py
+drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2023-07-17 14:16:12.891189 pycows-0.0.2/src/pycows.egg-info/
+-rw-r--r--   0 spfeifer   (501) staff       (20)     2305 2023-07-17 14:16:12.000000 pycows-0.0.2/src/pycows.egg-info/PKG-INFO
+-rw-r--r--   0 spfeifer   (501) staff       (20)     1011 2023-07-17 14:16:12.000000 pycows-0.0.2/src/pycows.egg-info/SOURCES.txt
+-rw-r--r--   0 spfeifer   (501) staff       (20)        1 2023-07-17 14:16:12.000000 pycows-0.0.2/src/pycows.egg-info/dependency_links.txt
+-rw-r--r--   0 spfeifer   (501) staff       (20)        1 2023-07-17 13:03:39.000000 pycows-0.0.2/src/pycows.egg-info/not-zip-safe
+-rw-r--r--   0 spfeifer   (501) staff       (20)        5 2023-07-17 14:16:12.000000 pycows-0.0.2/src/pycows.egg-info/top_level.txt
+drwxr-xr-x   0 spfeifer   (501) staff       (20)        0 2023-07-17 14:16:12.899614 pycows-0.0.2/tests/
+-rw-r--r--   0 spfeifer   (501) staff       (20)     1690 2023-07-17 13:03:15.000000 pycows-0.0.2/tests/test_arraycrop.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)     5397 2023-07-17 13:03:15.000000 pycows-0.0.2/tests/test_catalogue.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)  2097232 2023-07-17 13:03:15.000000 pycows-0.0.2/tests/test_data.npy
+-rw-r--r--   0 spfeifer   (501) staff       (20)     9587 2023-07-17 13:03:15.000000 pycows-0.0.2/tests/test_filament.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)     2689 2023-07-17 13:03:15.000000 pycows-0.0.2/tests/test_skeletonize.py
+-rw-r--r--   0 spfeifer   (501) staff       (20)     3273 2023-07-17 13:03:15.000000 pycows-0.0.2/tox.ini
```

### Comparing `pycows-0.0.1/LICENSE.txt` & `pycows-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/PKG-INFO` & `pycows-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pycows
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cosmic filament finder
 Home-page: https://github.com/SimonPfeifer/python-cows
 Author: Simon Pfeifer
 Author-email: spfeifer@aip.de
 License: BSD-3-Clause
 Project-URL: Documentation, https://python-cows.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/SimonPfeifer/cows/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
@@ -21,24 +20,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
-
-
-
 ====
 COWS
 ====
 
+
+
+
 The *cows* python package is an implementation of the cosmic filament finder COsmic Web Skeleton (COWS). The cosmic filament finder works on Hessian-based cosmic web idetifier (such as the V-web) and returns a catalogue of filament spines.
 
-It works by identifying the medial axis, or skeleton, of cosmic web filaments and then separating this skeleton into individual filaments. For more information of the specifics of the method, see `here <https://arxiv.org/search/astro-ph?searchtype=author&query=Pfeifer%2C+S>`_.
+It works by identifying the medial axis, or skeleton, of cosmic web filaments and then separating this skeleton into individual filaments. For more information of the specifics of the method, see `here <https://arxiv.org/pdf/2201.04624.pdf>`_.
 
 
 Requirements
 ------------
 ::
 
     numpy>=1.19.3
@@ -65,11 +64,9 @@
 
 
 Citing
 ======
 
 When using COWS in a publication, please cite the following paper:
 
-`arXiv:XXXX.XXXXX <https://arxiv.org/search/astro-ph?searchtype=author&query=Pfeifer%2C+S>`_ : "COWS: A filament finder for Hessian cosmic web identifiers"
-
-
+`arXiv:2201.04624 <https://arxiv.org/abs/2201.04624>`_ : "COWS: A filament finder for Hessian cosmic web identifiers"
```

### Comparing `pycows-0.0.1/README.rst` & `pycows-0.0.2/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,38 @@
+====
+COWS
+====
 
 .. start-badges
 
-.. image:: https://img.shields.io/github/commits-since/SimonPfeifer/python-cows/v0.0.1.svg
+.. image:: https://img.shields.io/pypi/v/pycows.svg
+    :alt: PyPi version
+    :target: https://pypi.com/v/pycows
+
+
+.. image:: https://img.shields.io/github/commits-since/SimonPfeifer/python-cows/v/v/v0.0.2...master.svg.svg
     :alt: Commits since latest release
-    :target: https://github.com/SimonPfeifer/python-cows/compare/v0.0.1...master
+    :target: https://github.com/SimonPfeifer/python-cows/compare/v/v/v0.0.2...master.svg...master
+
+
+.. image:: https://img.shields.io/pypi/pyversions/pycows.svg
+    :alt: Python versions
+    :target: https://pypi.python.org/pypi/pycows/
+
 
 .. image:: https://readthedocs.org/projects/python-cows/badge/?version=latest
-    :target: https://python-cows.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
+    :target: https://python-cows.readthedocs.io/en/latest/?badge=latest
 
 .. end-badges
 
-====
-COWS
-====
 
 The *cows* python package is an implementation of the cosmic filament finder COsmic Web Skeleton (COWS). The cosmic filament finder works on Hessian-based cosmic web idetifier (such as the V-web) and returns a catalogue of filament spines.
 
-It works by identifying the medial axis, or skeleton, of cosmic web filaments and then separating this skeleton into individual filaments. For more information of the specifics of the method, see `here <https://arxiv.org/search/astro-ph?searchtype=author&query=Pfeifer%2C+S>`_.
+It works by identifying the medial axis, or skeleton, of cosmic web filaments and then separating this skeleton into individual filaments. For more information of the specifics of the method, see `here <https://arxiv.org/pdf/2201.04624.pdf>`_.
 
 
 Requirements
 ------------
 ::
 
     numpy>=1.19.3
@@ -48,8 +59,8 @@
 
 
 Citing
 ======
 
 When using COWS in a publication, please cite the following paper:
 
-`arXiv:XXXX.XXXXX <https://arxiv.org/search/astro-ph?searchtype=author&query=Pfeifer%2C+S>`_ : "COWS: A filament finder for Hessian cosmic web identifiers"
+`arXiv:2201.04624 <https://arxiv.org/abs/2201.04624>`_ : "COWS: A filament finder for Hessian cosmic web identifiers"
```

### Comparing `pycows-0.0.1/ci/bootstrap.py` & `pycows-0.0.2/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/ci/templates/.github/workflows/github-actions.yml` & `pycows-0.0.2/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/docs/.ipynb_checkpoints/example-checkpoint.ipynb` & `pycows-0.0.2/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/docs/conf.py` & `pycows-0.0.2/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'cows'
 year = '2022'
 author = 'Simon Pfeifer'
 copyright = '{0}, {1}'.format(year, author)
-version = release = '0.0.1'
+version = release = '0.0.2'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/SimonPfeifer/python-cows/issues/%s', '#'),
     'pr': ('https://github.com/SimonPfeifer/python-cows/pull/%s', 'PR #'),
 }
```

### Comparing `pycows-0.0.1/docs/example.py` & `pycows-0.0.2/docs/example.py`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/docs/index.rst` & `pycows-0.0.2/docs/index.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ==================
 COWS documentation
 ==================
 
 The *cows* python package is an implementation of the cosmic filament finder COsmic Web Skeleton (COWS). The cosmic filament finder works on Hessian-based cosmic web idetifier (such as the V-web) and returns a catalogue of filament spines.
 
-It works by identifying the medial axis, or skeleton, of cosmic web filaments and then separating this skeleton into individual filaments. For more information of the specifics of the method, see `here <https://arxiv.org/search/astro-ph?searchtype=author&query=Pfeifer%2C+S>`_.
+It works by identifying the medial axis, or skeleton, of cosmic web filaments and then separating this skeleton into individual filaments. For more information of the specifics of the method, see `here <https://arxiv.org/pdf/2201.04624.pdf>`_.
 
 
 
 Installation
 ------------
 
 .. toctree::
@@ -38,7 +38,15 @@
 License
 -------
 
 .. toctree::
    :maxdepth: 1
    
    license
+
+
+Citing
+======
+
+When using COWS in a publication, please cite the following paper:
+
+`arXiv:2201.04624 <https://arxiv.org/abs/2201.04624>`_ : "COWS: A filament finder for Hessian cosmic web identifiers"
```

### Comparing `pycows-0.0.1/setup.py` & `pycows-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             encoding=kwargs.get('encoding', 'utf8')
         ) as fh:
             return fh.read()
 
 
     setup(
         name='pycows',
-        version='0.0.1',
+        version='0.0.2',
         license='BSD-3-Clause',
         description='Cosmic filament finder',
         long_description='%s\n' % (
             re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst'))),
         long_description_content_type = 'text/x-rst',
         author='Simon Pfeifer',
         author_email='spfeifer@aip.de',
```

### Comparing `pycows-0.0.1/src/cows/_filament.c` & `pycows-0.0.2/src/cows/_filament.c`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/src/cows/_filament.pyx` & `pycows-0.0.2/src/cows/_filament.pyx`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/src/cows/_skeletonize_3d_cy.cpp` & `pycows-0.0.2/src/cows/_skeletonize_3d_cy.cpp`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/src/cows/_skeletonize_3d_cy.pyx` & `pycows-0.0.2/src/cows/_skeletonize_3d_cy.pyx`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/src/cows/arraycrop.py` & `pycows-0.0.2/src/cows/arraycrop.py`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/src/cows/catalogue.py` & `pycows-0.0.2/src/cows/catalogue.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,20 @@
 
     # Classify the skeleton to identify endpoints and regular cells
     data = label_skeleton(data, periodic=periodic)
 
     # Connect cells within a 3x3x3 neighbourhood from endpoint to endpoint
     # and store in the first column 
     _, cat = find_filaments(data, periodic=periodic)
+
+    # Crop the catalogue if not completely full
+    if np.any(cat[:, 0] == 0):
+        cat = cat[:np.argmin(cat[:, 0])]
+
+    # Copy into new array
     catalogue = np.zeros([cat.shape[0], 8], order='c')
     catalogue[:,0] = cat[:,0]
 
     # Return the empty catalogue if no filaments were found
     if catalogue.shape[0] == 0:
         return catalogue
 
@@ -95,8 +101,8 @@
     # Add direction to appropriate indices
     dxyz_tmp = dxyz_tmp * idx_diff[:,None] # set to 0 between filaments
     dxyz[:-1] += dxyz_tmp 
     dxyz[1:] += dxyz_tmp
 
     # Noramlise direction vector
     r = np.sqrt(np.sum(dxyz**2, axis=1))
-    return dxyz/r[:,None]
+    return dxyz/r[:,None]
```

### Comparing `pycows-0.0.1/src/cows/cows.egg-info/PKG-INFO` & `pycows-0.0.2/src/pycows.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,72 @@
 Metadata-Version: 2.1
-Name: cows
-Version: 0.0.0
+Name: pycows
+Version: 0.0.2
 Summary: Cosmic filament finder
-Home-page: https://github.com/SimonPfeifer/cows
+Home-page: https://github.com/SimonPfeifer/python-cows
 Author: Simon Pfeifer
 Author-email: spfeifer@aip.de
 License: BSD-3-Clause
 Project-URL: Documentation, https://python-cows.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/SimonPfeifer/cows/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
-
-
-
 ====
 COWS
 ====
 
-The *cows* python package is an implelemtation of the cosmic filament finder COsmic Web Skeleton (COWS). The cosmic filament finder works on Hessian-based cosmic web idetifier (such as the V-web) and returns a catalogue of filament spines.
 
-It works by identifying the medial axis, or skeleton, of cosmic web filaments and then speparating this skeleton into individual filaments. For more information of the specifics of the method, see `here <https://arxiv.org/search/astro-ph?searchtype=author&query=Pfeifer%2C+S>`_.
+
+
+The *cows* python package is an implementation of the cosmic filament finder COsmic Web Skeleton (COWS). The cosmic filament finder works on Hessian-based cosmic web idetifier (such as the V-web) and returns a catalogue of filament spines.
+
+It works by identifying the medial axis, or skeleton, of cosmic web filaments and then separating this skeleton into individual filaments. For more information of the specifics of the method, see `here <https://arxiv.org/pdf/2201.04624.pdf>`_.
 
 
 Requirements
 ------------
 ::
 
-    numpy
+    numpy>=1.19.3
 
 Quick installation
 ------------------
 
 To install the *cows* python package using PyPI::
 
-    pip install cows
+    pip install pycows
 
 To install the package from source::
 
     python setup.py install
 
 For more inforamtion on installation, see `INSTALL.rst <https://github.com/SimonPfeifer/cows/blob/master/INSTALLATION.rst>`_.
 
 Documentation
 ==============
 
 The full documentation can be accessed at `readthedocs <https://python-cows.readthedocs.io/en/latest/index.html>`_ or generated as a set of local files by running::
 
-    sphinx-build ./doc ./docs/_build
+    sphinx-build ./docs ./docs/_build
 
 
 Citing
 ======
 
 When using COWS in a publication, please cite the following paper:
 
-`arXiv:XXXX.XXXXX <https://arxiv.org/search/astro-ph?searchtype=author&query=Pfeifer%2C+S>`_ : "COWS: A filament finder for Hessian cosmic web identifiers"
-
-
+`arXiv:2201.04624 <https://arxiv.org/abs/2201.04624>`_ : "COWS: A filament finder for Hessian cosmic web identifiers"
```

### Comparing `pycows-0.0.1/src/cows/dtype.py` & `pycows-0.0.2/src/cows/dtype.py`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/src/cows/filament.py` & `pycows-0.0.2/src/cows/filament.py`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/src/cows/skeletonize.py` & `pycows-0.0.2/src/cows/skeletonize.py`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/tests/test_arraycrop.py` & `pycows-0.0.2/tests/test_arraycrop.py`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/tests/test_catalogue.py` & `pycows-0.0.2/tests/test_catalogue.py`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/tests/test_data.npy` & `pycows-0.0.2/tests/test_data.npy`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/tests/test_filament.py` & `pycows-0.0.2/tests/test_filament.py`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/tests/test_skeletonize.py` & `pycows-0.0.2/tests/test_skeletonize.py`

 * *Files identical despite different names*

### Comparing `pycows-0.0.1/tox.ini` & `pycows-0.0.2/tox.ini`

 * *Files identical despite different names*

