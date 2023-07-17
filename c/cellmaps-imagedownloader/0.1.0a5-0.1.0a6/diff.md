# Comparing `tmp/cellmaps_imagedownloader-0.1.0a5.tar.gz` & `tmp/cellmaps_imagedownloader-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_imagedownloader-0.1.0a5.tar", last modified: Tue May 23 16:32:00 2023, max compression
+gzip compressed data, was "dist/cellmaps_imagedownloader-0.1.0a6.tar", last modified: Mon Jul 17 19:13:47 2023, max compression
```

## Comparing `cellmaps_imagedownloader-0.1.0a5.tar` & `cellmaps_imagedownloader-0.1.0a6.tar`

### file list

```diff
@@ -1,59 +1,63 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.955100 cellmaps_imagedownloader-0.1.0a5/
--rw-r--r--   0 churas     (504) staff       (20)      150 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3731 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a5/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-11 22:14:34.000000 cellmaps_imagedownloader-0.1.0a5/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5191 2023-05-23 16:32:00.955244 cellmaps_imagedownloader-0.1.0a5/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3284 2023-05-22 22:23:15.000000 cellmaps_imagedownloader-0.1.0a5/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.938564 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/
--rw-r--r--   0 churas     (504) staff       (20)      341 2023-05-23 16:21:03.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     9182 2023-05-11 21:43:55.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py
--rw-r--r--   0 churas     (504) staff       (20)      145 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    14323 2023-05-22 22:15:28.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/gene.py
--rw-r--r--   0 churas     (504) staff       (20)    27797 2023-05-23 16:31:16.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.940710 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5191 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1360 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       36 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       25 2023-05-23 16:32:00.000000 cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.948811 cellmaps_imagedownloader-0.1.0a5/docs/
--rw-r--r--   0 churas     (504) staff       (20)      625 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.934265 cellmaps_imagedownloader-0.1.0a5/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.934335 cellmaps_imagedownloader-0.1.0a5/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.949701 cellmaps_imagedownloader-0.1.0a5/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a5/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a5/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a5/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1027 2023-05-03 22:58:28.000000 cellmaps_imagedownloader-0.1.0a5/docs/cellmaps_imagedownloader.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6214 2023-05-22 22:22:34.000000 cellmaps_imagedownloader-0.1.0a5/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      292 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      243 2023-05-22 21:38:15.000000 cellmaps_imagedownloader-0.1.0a5/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1254 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      472 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       83 2023-05-22 23:09:36.000000 cellmaps_imagedownloader-0.1.0a5/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4424 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      739 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a5/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      407 2023-05-23 16:32:00.955705 cellmaps_imagedownloader-0.1.0a5/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1899 2023-05-18 20:34:04.000000 cellmaps_imagedownloader-0.1.0a5/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.953964 cellmaps_imagedownloader-0.1.0a5/tests/
--rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a5/tests/__init__.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-23 16:32:00.954726 cellmaps_imagedownloader-0.1.0a5/tests/data/
--rw-r--r--   0 churas     (504) staff       (20)      166 2023-05-22 20:49:48.000000 cellmaps_imagedownloader-0.1.0a5/tests/data/test_single_sample.tsv
--rw-r--r--   0 churas     (504) staff       (20)      122 2023-05-22 20:51:02.000000 cellmaps_imagedownloader-0.1.0a5/tests/data/test_single_unique.tsv
--rw-r--r--   0 churas     (504) staff       (20)     1429 2023-05-22 21:41:10.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_cellmaps_imagedownloadercmd.py
--rw-r--r--   0 churas     (504) staff       (20)     7543 2023-05-11 21:09:17.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_cellmapsimagedownloader.py
--rw-r--r--   0 churas     (504) staff       (20)     2245 2023-05-04 00:03:34.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_genenodegenerator.py
--rw-r--r--   0 churas     (504) staff       (20)     2739 2023-05-22 21:29:59.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_genequery.py
--rw-r--r--   0 churas     (504) staff       (20)     8830 2023-05-22 21:58:39.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_imagegenenodegenerator.py
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_integration_cellmaps_downloader.py
--rw-r--r--   0 churas     (504) staff       (20)     1018 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a5/tests/test_multiprocessimagedownloader.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.116332 cellmaps_imagedownloader-0.1.0a6/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-07-17 19:13:09.000000 cellmaps_imagedownloader-0.1.0a6/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3731 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a6/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-11 22:14:34.000000 cellmaps_imagedownloader-0.1.0a6/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5242 2023-07-17 19:13:47.116462 cellmaps_imagedownloader-0.1.0a6/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3281 2023-06-07 18:23:11.000000 cellmaps_imagedownloader-0.1.0a6/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.102169 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/
+-rw-r--r--   0 churas     (504) staff       (20)      354 2023-07-17 19:13:09.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    11048 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      145 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    16811 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/gene.py
+-rw-r--r--   0 churas     (504) staff       (20)     7244 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/proteinatlas.py
+-rw-r--r--   0 churas     (504) staff       (20)    29631 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.104744 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5242 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1517 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       36 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       25 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.110537 cellmaps_imagedownloader-0.1.0a6/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      625 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.096461 cellmaps_imagedownloader-0.1.0a6/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.096598 cellmaps_imagedownloader-0.1.0a6/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.111593 cellmaps_imagedownloader-0.1.0a6/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a6/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a6/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a6/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1027 2023-05-03 22:58:28.000000 cellmaps_imagedownloader-0.1.0a6/docs/cellmaps_imagedownloader.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6214 2023-05-22 22:22:34.000000 cellmaps_imagedownloader-0.1.0a6/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      292 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      243 2023-05-22 21:38:15.000000 cellmaps_imagedownloader-0.1.0a6/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1254 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      472 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       83 2023-05-22 23:09:36.000000 cellmaps_imagedownloader-0.1.0a6/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4424 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      739 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      407 2023-07-17 19:13:47.117022 cellmaps_imagedownloader-0.1.0a6/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2242 2023-07-17 19:13:09.000000 cellmaps_imagedownloader-0.1.0a6/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.115487 cellmaps_imagedownloader-0.1.0a6/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a6/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.116033 cellmaps_imagedownloader-0.1.0a6/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)      166 2023-05-22 20:49:48.000000 cellmaps_imagedownloader-0.1.0a6/tests/data/test_single_sample.tsv
+-rw-r--r--   0 churas     (504) staff       (20)      122 2023-05-22 20:51:02.000000 cellmaps_imagedownloader-0.1.0a6/tests/data/test_single_unique.tsv
+-rw-r--r--   0 churas     (504) staff       (20)     1429 2023-06-14 20:42:24.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_cellmaps_imagedownloadercmd.py
+-rw-r--r--   0 churas     (504) staff       (20)    26236 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_cellmapsimagedownloader.py
+-rw-r--r--   0 churas     (504) staff       (20)      896 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_genenodegenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)     2739 2023-06-14 20:42:15.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_genequery.py
+-rw-r--r--   0 churas     (504) staff       (20)     4286 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_imagedownloadtuplegenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)    20366 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_imagegenenodegenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_integration_cellmaps_downloader.py
+-rw-r--r--   0 churas     (504) staff       (20)     1018 2023-06-14 20:38:55.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_multiprocessimagedownloader.py
+-rw-r--r--   0 churas     (504) staff       (20)     2447 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_proteinatlasimageurlreader.py
+-rw-r--r--   0 churas     (504) staff       (20)     3639 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_proteinatlasreader.py
```

### Comparing `cellmaps_imagedownloader-0.1.0a5/CONTRIBUTING.rst` & `cellmaps_imagedownloader-0.1.0a6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/LICENSE` & `cellmaps_imagedownloader-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/PKG-INFO` & `cellmaps_imagedownloader-0.1.0a6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cellmaps_imagedownloader
-Version: 0.1.0a5
-Summary: Downloads IF data needed for CM4AI MuSIC pipeline
+Version: 0.1.0a6
+Summary: A tool to download specified image data from the Human Protein Atlas website using CSV file
 Home-page: https://github.com/idekerlab/cellmaps_imagedownloader
-Author: Gege Qian
-Author-email: geqian@ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
 Description: =========================
         cellmaps_imagedownloader
         =========================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_imagedownloader.svg
@@ -52,15 +52,15 @@
         **Or directly from source:**
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_imagedownloader
            cd cellmaps_imagedownloader
            make dist
-           pip install dist/cellmaps_imagedownloadercmd*whl
+           pip install dist/cellmaps_imagedownloader*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_imagedownloader-0.1.0a5/README.rst` & `cellmaps_imagedownloader-0.1.0a6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 **Or directly from source:**
 
 .. code-block::
 
    git clone https://github.com/idekerlab/cellmaps_imagedownloader
    cd cellmaps_imagedownloader
    make dist
-   pip install dist/cellmaps_imagedownloadercmd*whl
+   pip install dist/cellmaps_imagedownloader*whl
 
 
 Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
 
 .. code-block::
 
    make
```

### Comparing `cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py` & `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from cellmaps_utils import logutils
 from cellmaps_utils import constants
 import cellmaps_imagedownloader
 from cellmaps_imagedownloader.runner import MultiProcessImageDownloader
 from cellmaps_imagedownloader.runner import FakeImageDownloader
 from cellmaps_imagedownloader.runner import CellmapsImageDownloader
 from cellmaps_imagedownloader.gene import ImageGeneNodeAttributeGenerator
+from cellmaps_imagedownloader.proteinatlas import ProteinAtlasReader
+from cellmaps_imagedownloader.proteinatlas import ProteinAtlasImageUrlReader
+from cellmaps_imagedownloader.proteinatlas import ImageDownloadTupleGenerator
+
 
 logger = logging.getLogger(__name__)
 
 
 def _parse_arguments(desc, args):
     """
     Parses command line arguments
@@ -49,14 +53,19 @@
     parser.add_argument('--provenance',
                         help='Path to file containing provenance '
                              'information about input files in JSON format. '
                              'This is required and not including will output '
                              'and error message with example of file')
     parser.add_argument('--image_url', default='https://images.proteinatlas.org',
                         help='Base URL for downloading IF images')
+    parser.add_argument('--proteinatlasxml',
+                        default='https://www.proteinatlas.org/download/proteinatlas.xml.gz',
+                        help='URL or path to proteinatlas.xml or proteinatlas.xml.gz file '
+                             'used to look for images not found in the standard location '
+                             'on HPA')
     parser.add_argument('--fake_images', action='store_true',
                         help='If set, 1st image of each color is downloaded '
                              'and subsequent images are just copies of those '
                              'images')
     parser.add_argument('--poolsize', type=int,
                         default=4,
                         help='If using multiprocessing image downloader, '
@@ -117,14 +126,26 @@
 from HPA via --samples flag
 
 Format of CSV file:
 
 filename,if_plate_id,position,sample,status,locations,antibody,ensembl_ids,gene_names
 /archive/1/1_A1_1_,1,A1,1,35,Golgi apparatus,HPA000992,ENSG00000066455,GOLGA5
 
+Definition of columns:
+
+* filename - Filename of image (string)
+* if_plate_id - ID of plate for acquired image (int)
+* position - Position in plate for acquired image (string)
+* sample - Sample number identifier for acquired image (int)
+* status - Unknown 
+* locations - Comma delimited list of manual annotations for image (string)
+* antibody - Name of antibody used for acquired image (string)
+* ensembl_ids - Comma delimited list of Ensembl IDs (string)
+* gene_names - Comma delimited list of genes (string)
+
 The downloaded images are stored under the output directory
 specified on the command line in color specific directories
 (red, blue, green, yellow) with name format of: 
 <NAME>_color.jpg 
 
 Example: 1_A1_1_blue.jpg
 
@@ -132,14 +153,23 @@
 use. 
 
 Format of CSV file:
 
 antibody,ensembl_ids,gene_names,atlas_name,locations,n_location
 HPA040086,ENSG00000094914,AAAS,U-2 OS,Nuclear membrane,1
 
+Definition of columns:
+
+* antibody - Name of antibody used for acquired image (string)
+* ensembl_ids - Comma delimited list of ensembl IDs for target protein(s) (string)
+* gene_names - Comma delimited list of gene names for target proteins(s) (string)
+* atlas_name - Cell line (string)
+* locations - Comma delimited list of subcellular locations (string)
+* n_location - Number of subcellular locations (int)
+
 In addition, the --provenance flag is required and must be set to a path 
 to a JSON file. 
 
 If datasets are already registered with FAIRSCAPE then the following is sufficient:
 
 {withguids}
 
@@ -170,29 +200,33 @@
             sys.stderr.write('If datasets are NOT registered, then the following is required:\n\n')
             sys.stderr.write(register_json + '\n\n')
             return 1
 
         # load the provenance as a dict
         with open(theargs.provenance, 'r') as f:
             json_prov = json.load(f)
-
         imagegen = ImageGeneNodeAttributeGenerator(unique_list=ImageGeneNodeAttributeGenerator.get_unique_list_from_csvfile(theargs.unique),
                                                    samples_list=ImageGeneNodeAttributeGenerator.get_samples_from_csvfile(theargs.samples))
 
         if theargs.fake_images is True:
             warnings.warn('FAKE IMAGES ARE BEING DOWNLOADED!!!!!')
             dloader = FakeImageDownloader()
         else:
             dloader = MultiProcessImageDownloader(poolsize=theargs.poolsize,
                                                   skip_existing=theargs.skip_existing)
+
+        proteinatlas_reader = ProteinAtlasReader(theargs.outdir, proteinatlas=theargs.proteinatlasxml)
+        proteinatlas_urlreader = ProteinAtlasImageUrlReader(reader=proteinatlas_reader)
+        imageurlgen = ImageDownloadTupleGenerator(reader=proteinatlas_urlreader,
+                                                  samples_list=imagegen.get_samples_list())
         return CellmapsImageDownloader(outdir=theargs.outdir,
                                        imagedownloader=dloader,
                                        imgsuffix=theargs.imgsuffix,
                                        imagegen=imagegen,
-                                       image_url=theargs.image_url,
+                                       imageurlgen=imageurlgen,
                                        skip_logging=theargs.skip_logging,
                                        input_data_dict=theargs.__dict__,
                                        provenance=json_prov,
                                        skip_failed=theargs.skip_failed).run()
     except Exception as e:
         logger.exception('Caught exception: ' + str(e))
         return 2
```

### Comparing `cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/gene.py` & `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/gene.py`

 * *Files 16% similar despite different names*

```diff
@@ -80,46 +80,14 @@
     """
     def __init__(self):
         """
         Constructor
         """
         pass
 
-    @staticmethod
-    def add_geneids_to_set(gene_set=None,
-                           ambiguous_gene_dict=None,
-                           geneid=None):
-        """
-        Examines **geneid** passed in and if a comma exists
-        in value split by comma and assume multiple genes.
-        Adds those genes into **gene_set** and add entry
-        to **ambiguous_gene_dict** with key set to each gene
-        name and value set to original **geneid** value
-
-        :param gene_set: unique set of genes
-        :type gene_set: set
-        :param geneid: name of gene or comma delimited string of genes
-        :type geneid: str
-        :return: genes found in **geneid** or None if **gene_set**
-                 or **geneid** is ``None``
-        :rtype: list
-        """
-        if gene_set is None:
-            return None
-        if geneid is None:
-            return None
-
-        split_str = re.split('\W*,\W*', geneid)
-        gene_set.update(split_str)
-        if ambiguous_gene_dict is not None:
-            if len(split_str) > 1:
-                for entry in split_str:
-                    ambiguous_gene_dict[entry] = geneid
-        return split_str
-
     def get_gene_node_attributes(self):
         """
         Should be implemented by subclasses
 
         :raises NotImplementedError: Always
         """
         raise NotImplementedError('Subclasses should implement')
@@ -281,20 +249,83 @@
             for row in reader:
                 unique_entry = {}
                 for key in ImageGeneNodeAttributeGenerator.UNIQUE_HEADER_COLS:
                     unique_entry[key] = row[key]
                 u_list.append(unique_entry)
         return u_list
 
+    def write_unique_list_to_csvfile(self, csvfile=None):
+        """
+        Writes unique list to file
+
+        :param csvfile: path to file to write
+        :type csvfile: str
+        """
+        if csvfile is None:
+            raise CellMapsImageDownloaderError('csvfile is None')
+        with open(csvfile, 'w', newline='') as f:
+            writer = csv.DictWriter(f,
+                                    fieldnames=ImageGeneNodeAttributeGenerator.UNIQUE_HEADER_COLS,
+                                    delimiter=',')
+            writer.writeheader()
+            for unique_entry in self._unique_list:
+                writer.writerow(unique_entry)
+
+    def write_samples_to_csvfile(self, csvfile=None):
+        """
+        Writes samples to file
+
+        :param csvfile: path to file to write
+        :type csvfile: str
+        """
+        if csvfile is None:
+            raise CellMapsImageDownloaderError('csvfile is None')
+        with open(csvfile, 'w', newline='') as f:
+            writer = csv.DictWriter(f,
+                                    fieldnames=ImageGeneNodeAttributeGenerator.SAMPLES_HEADER_COLS,
+                                    delimiter=',')
+            writer.writeheader()
+            for sample in self._samples_list:
+                writer.writerow(sample)
+
+    def _get_unique_ids_from_samplelist(self, column='ensembl_ids'):
+        """
+        Gets a unique list of ids split by comma from the samples
+        under **column**.
+
+        For example for a sample with these values and column set to ``ensembl_ids``:
+
+        .. code-block:: python
+
+            {'ensembl_ids': 'ENSG00000240682,ENSG00000261796'}
+
+        The resulting tuple would be:
+
+        .. code-block:: python
+
+            ['ENSG00000240682', 'ENSG00000261796']
+
+        :return: split values from corresponding **column** in samples list
+        :rtype: list
+        """
+        id_set = set()
+
+        for row in self._samples_list:
+            geneid=row[column]
+            split_str = re.split('\W*,\W*', geneid)
+            id_set.update(split_str)
+
+        return list(id_set)
+
     def _get_set_of_antibodies_from_unique_list(self):
         """
         Extract a unique set of antibodies from antibodies list
         passed in via constructor
 
-        :return:
+        :return: unique antibodies
         :rtype: set
         """
         if self._unique_list is None:
             raise CellMapsImageDownloaderError('unique list is None')
 
         antibody_set = set()
         for a in self._unique_list:
@@ -303,138 +334,176 @@
                                'in unique entry: ' + str(a))
                 continue
             antibody_set.add(a['antibody'])
         return antibody_set
 
     def get_dicts_of_gene_to_antibody_filename(self, allowed_antibodies=None):
         """
-        Gets a dictionary where key is ensembl id and value is
-        the file_name value
+        Gets a tuple of dictionaries from the sample list passed in via
+        the constructor.
 
-        :return:
-        :rtype: dict
+
+        :param allowed_antibodies: Skip samples whose antibody is NOT in this list.
+                                   If ``None`` then all samples are included
+        :type allowed_antibodies: list or set
+        :return: (:py:class:`dict` of ensembl_id => antibody,
+                  :py:class:`dict` of antibody => filename,
+                  :py:class:`dict` of antibody => comma delimited ambiguous ensembl_ids)
+
+        :rtype: tuple
         """
         if self._samples_list is None:
             raise CellMapsImageDownloaderError('samples list is None')
 
         g_antibody_dict = {}
-        g_filename_dict = {}
+        antibody_filename_dict = {}
+        ambiguous_antibody_dict = {}
 
         for sample in self._samples_list:
-            if allowed_antibodies is not None and sample['antibody'] not in allowed_antibodies:
+            antibody = sample['antibody']
+            if allowed_antibodies is not None and antibody not in allowed_antibodies:
                 # skipping cause antibody is not in allowed set
                 continue
 
             ensembl_ids = sample['ensembl_ids'].split(',')
+            if len(ensembl_ids) > 1:
+                ambiguous_antibody_dict[antibody] = sample['ensembl_ids']
+
+            if antibody not in antibody_filename_dict:
+                antibody_filename_dict[antibody] = set()
+            antibody_filename_dict[antibody].add(sample['if_plate_id'] + '_' +
+                                   sample['position'] + '_' +
+                                   sample['sample'] + '_')
             for g in ensembl_ids:
-                if g not in g_antibody_dict:
-                    g_antibody_dict[g] = set()
-                if g not in g_filename_dict:
-                    g_filename_dict[g] = set()
-                g_antibody_dict[g].add(sample['antibody'])
-                g_filename_dict[g].add(sample['if_plate_id'] + '_' +
-                                       sample['position'] + '_' +
-                                       sample['sample'] + '_')
+                #if gene already has nonambgiuous antibody, use that one
+                if g in g_antibody_dict:
+                    if g in ambiguous_antibody_dict:
+                        continue
+                g_antibody_dict[g] = sample['antibody']
 
-        return g_antibody_dict, g_filename_dict
+        return g_antibody_dict, antibody_filename_dict, ambiguous_antibody_dict
 
-    def _get_unique_ids_from_samplelist(self, column='ensembl_ids'):
+    def get_gene_node_attributes(self, fold=1):
         """
-        Gets a unique list of ids split by comma from the samples
-        under **column**. In addition a dict is also created where
-        key is split id and value is original unsplit values
+        Using **samples_list** and **unique_list**, builds
+        a list of :py:class:`dict` objects with updated Gene Symbols.
 
-        For example for a sample with these values and column set to ``ensembl_ids``:
+        Format of each resulting :py:class:`dict`:
 
-        .. code-block:: python
+        .. code-block::
 
-            {'ensembl_ids': 'ENSG00000240682,ENSG00000261796'}
+            {'name': GENE_SYMBOL,
+             'represents': ENSEMBL_ID,
+             'ambiguous': AMBIGUOUS_GENES,
+             'antibody': ANTIBODY,
+             'filename': FILENAME}
 
-        The resulting tuple would be:
+        **Example**
 
-        .. code-block:: python
+        .. code-block::
 
-            (['ENSG00000240682', 'ENSG00000261796'],
-             {'ENSG00000240682': 'ENSG00000240682,ENSG00000261796',
-              'ENSG00000261796': 'ENSG00000240682,ENSG00000261796'})
+            {'ENSG00000066455': {'name': 'GOLGA5',
+                                 'represents': 'ensembl:ENSG00000066455',
+                                 'ambiguous': '',
+                                 'antibody': 'HPA000992',
+                                 'filename': '1_A1_2_,1_A1_1_'}}
 
-        :return: (list of ids, dict where key is id and value is original unsplit value)
+        :return: (list of dict, list of errors)
         :rtype: tuple
         """
-        id_set = set()
-        ambiguous_id_dict = {}
-
-        for row in self._samples_list:
-            GeneNodeAttributeGenerator.add_geneids_to_set(gene_set=id_set,
-                                                          ambiguous_gene_dict=ambiguous_id_dict,
-                                                          geneid=row[column])
-        return list(id_set), ambiguous_id_dict
+        # Todo: Refactor because this method is doing waaay too much
 
-    def get_gene_node_attributes(self):
-        """
-        TODO: need to implement this
-
-        :return:
-        """
         t = tqdm(total=5, desc='Get updated gene symbols',
                  unit='steps')
 
         t.update()
         # get the unique set of ensembl_ids for mygene query
-        ensembl_id_list, _ = self._get_unique_ids_from_samplelist()
+        ensembl_id_list = self._get_unique_ids_from_samplelist()
 
         t.update()
+
+        # queries mygene and gets a list of dicts that look like this:
+        # {'query': 'ENSG00000066455',
+        #  '_id': '9950',
+        #  '_score': 25.046944,
+        #  'ensembl': {'gene':'ENSG00000066455'},
+        #  'symbol': 'GOLGA5'
+        # }
         query_res = self._genequery.get_symbols_for_genes(genelist=ensembl_id_list,
                                                           scopes='ensembl.gene')
-        t.update()
-        # get mapping of ambiguous genes
-        _, ambiguous_gene_dict = self._get_unique_ids_from_samplelist(column='gene_names')
 
         t.update()
+
         # get the unique or best antibodies to use
         unique_antibodies = self._get_set_of_antibodies_from_unique_list()
 
         t.update()
         # create a mapping of ensembl id to antibody and ensembl_id to filenames
         # where entries NOT in unique_antibodies are filtered out
-        g_antibody_dict, g_filename_dict = self.get_dicts_of_gene_to_antibody_filename(allowed_antibodies=unique_antibodies)
+        # get mapping of ambiguous genes
+        g_antibody_dict, antibody_filename_dict, ambiguous_antibody_dict = self.get_dicts_of_gene_to_antibody_filename(allowed_antibodies=unique_antibodies)
 
         errors = []
         gene_node_attrs = {}
         for x in query_res:
+
+            # skips item that lacks a symbol like this one:
+            # {'query': 'ENSG00000282988',
+            #  '_id': 'ENSG00000282988',
+            #  '_score': 25.04868,
+            #  'ensembl': {'gene': 'ENSG00000282988'}}
             if 'symbol' not in x:
                 errors.append('Skipping ' + str(x) +
                               ' no symbol in query result: ' + str(x))
                 logger.error(errors[-1])
                 continue
+
             ensemblstr = 'ensembl:'
+
+            # skips item that lacks anything like this one:
+            # {'query': 'ENSG000001', 'notfound': True}
             if 'ensembl' not in x:
                 errors.append('Skipping ' + str(x) +
                               ' no ensembl in query result: ' + str(x))
                 logger.error(errors[-1])
                 continue
 
             ensembl_id = None
 
+            # check if item 'ensembl' has more then 1 element
+            #
+            # {'query': 'ENSG00000273706',
+            #  '_id': '3975', '_score': 24.515644,
+            #  'ensembl': [{'gene': 'ENSG00000273706'},
+            #              {'gene': 'ENSG00000274577'}],
+            #  'symbol': 'LHX1'}
             if len(x['ensembl']) > 1:
                 for g in x['ensembl']:
                     if g['gene'] in g_antibody_dict:
+                        # we need an ensembl id for filename and antibody
+                        # lookup so just grab the 1st one
                         ensembl_id = g['gene']
                         break
+                # concatenate ensembl ids and delimit with ;
                 ensemblstr += ';'.join([g['gene'] for g in x['ensembl']])
             else:
                 ensemblstr += x['ensembl']['gene']
                 ensembl_id = x['ensembl']['gene']
 
-            filename_str = ','.join(list(g_filename_dict[ensembl_id]))
-            antibody_str = ','.join(list(g_antibody_dict[ensembl_id]))
+            antibody_str = g_antibody_dict[ensembl_id]
+
+            filenames = list(antibody_filename_dict[antibody_str])
+            if len(filenames) < fold:
+                filename_str = filenames[0]
+            else:
+                filename_str = filenames[fold - 1]
 
             ambiguous_str = ''
-            if x['symbol'] in ambiguous_gene_dict:
-                ambiguous_str = ambiguous_gene_dict[x['symbol']]
+            if antibody_str in ambiguous_antibody_dict:
+                ambiguous_str = ambiguous_antibody_dict[antibody_str]
 
             gene_node_attrs[x['query']] = {'name': x['symbol'],
                                            'represents': ensemblstr,
                                            'ambiguous': ambiguous_str,
                                            'antibody': antibody_str,
                                            'filename': filename_str}
```

### Comparing `cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader/runner.py` & `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,15 +104,16 @@
     Creates fake download by downloading
     the first image in each color from
     `Human Protein Atlas <https://www.proteinatlas.org/>`__
     and making renamed copies. The :py:func:`download_file` function
     is used to download the first image of each color
 
     """
-    def __abs__(self):
+
+    def __init__(self):
         """
         Constructor
 
         """
         super().__init__()
         warnings.warn('This downloader generates FAKE images\n'
                       'You have been warned!!!\n'
@@ -235,15 +236,15 @@
     SAMPLES_FILEKEY = 'samples'
     UNIQUE_FILEKEY = 'unique'
 
     def __init__(self, outdir=None,
                  imgsuffix='.jpg',
                  imagedownloader=MultiProcessImageDownloader(),
                  imagegen=None,
-                 image_url='https://images.proteinatlas.org',
+                 imageurlgen=None,
                  skip_logging=False,
                  provenance=None,
                  input_data_dict=None,
                  provenance_utils=ProvenanceUtil(),
                  skip_failed=False):
         """
         Constructor
@@ -273,15 +274,15 @@
             raise CellMapsImageDownloaderError('outdir is None')
         self._outdir = os.path.abspath(outdir)
         self._imagedownloader = imagedownloader
         self._imgsuffix = imgsuffix
         self._start_time = int(time.time())
         self._end_time = -1
         self._imagegen = imagegen
-        self._image_url = image_url
+        self._imageurlgen = imageurlgen
         self._provenance = provenance
         self._input_data_dict = input_data_dict
         if skip_logging is None:
             self._skip_logging = False
         else:
             self._skip_logging = skip_logging
         self._samples_datasetid = None
@@ -348,51 +349,66 @@
         :raises CellMapsProvenanceError: If fairscape call fails
         """
         self._softwareid = self._provenance_utils.register_software(self._outdir,
                                                                     name=cellmaps_imagedownloader.__name__,
                                                                     description=cellmaps_imagedownloader.__description__,
                                                                     author=cellmaps_imagedownloader.__author__,
                                                                     version=cellmaps_imagedownloader.__version__,
-                                                                    file_format='.py',
+                                                                    file_format='py',
                                                                     url=cellmaps_imagedownloader.__repo_url__)
 
-    def _register_image_gene_node_attrs(self):
+    def _register_image_gene_node_attrs(self, fold=1):
         """
-        Registers image_gene_node_attributes.tsv file with create as a dataset
+        Registers <fold>_image_gene_node_attributes.tsv file with
+        ro-crate as a dataset
 
+        :param fold: name of fold
+        :type fold: int
         """
-        data_dict = {'name': cellmaps_imagedownloader.__name__ + ' output file',
-                     'description': 'Image gene node attributes file',
+        if self._image_gene_attrid is None:
+            self._image_gene_attrid = []
+        data_dict = {'name': cellmaps_imagedownloader.__name__ +
+                             ' output file',
+                     'description': 'Fold ' + str(fold) +
+                                    ' Image gene node attributes file',
                      'data-format': 'tsv',
                      'author': cellmaps_imagedownloader.__name__,
                      'version': cellmaps_imagedownloader.__version__,
                      'date-published': date.today().strftime('%m-%d-%Y')}
-        self._image_gene_attrid = self._provenance_utils.register_dataset(self._outdir,
-                                                                          source_file=self.get_image_gene_node_attributes_file(),
-                                                                          data_dict=data_dict)
+        src_file = self.get_image_gene_node_attributes_file(fold)
+        self._image_gene_attrid.append(self._provenance_utils.register_dataset(self._outdir,
+                                                                          source_file=src_file,
+                                                                          data_dict=data_dict))
 
     def _add_dataset_to_crate(self, data_dict=None,
                               source_file=None, skip_copy=True):
         """
+        Adds a dataset to rocrate
 
-        :param crate_path:
-        :param data_dict:
+        :param crate_path: Path to rocrate
+        :type crate_path: str
+        :param data_dict: information needed to add dataset
+        :type data_dict: dict
         :return:
         """
         return self._provenance_utils.register_dataset(self._outdir,
                                                        source_file=source_file,
                                                        data_dict=data_dict,
                                                        skip_copy=skip_copy)
 
     def _register_computation(self):
         """
+        Registers computation with rocrate.
+        Current implementation only registers the 1st 2000 images
 
-        :return:
         """
-        generated = [self._image_gene_attrid]
+        if self._image_gene_attrid is not None:
+            generated = self._image_gene_attrid
+        else:
+            generated = []
         if self._image_dataset_ids is not None:
             if len(self._image_dataset_ids) > 2000:
                 logger.error('Too many images to register with FAIRSCAPE. registering 1st 2,000')
                 warnings.warn('Too many images to register with FAIRSCAPE. registering 1st 2,000')
                 generated.extend(self._image_dataset_ids[0:2000])
             else:
                 generated.extend(self._image_dataset_ids)
@@ -418,45 +434,65 @@
                                                     organization_name=self._provenance['organization-name'],
                                                     project_name=self._provenance['project-name'])
         except TypeError as te:
             raise CellMapsImageDownloaderError('Invalid provenance: ' + str(te))
         except KeyError as ke:
             raise CellMapsImageDownloaderError('Key missing in provenance: ' + str(ke))
 
-    def _register_input_datasets(self):
+    def _register_samples_dataset(self):
         """
-        Registers samples and unique input datasets with FAIRSCAPE
-        setting **self._samples_datasetid** and **self._unique_datasetid**
-        values.
 
         :return:
         """
-
         if 'guid' in self._provenance[CellmapsImageDownloader.SAMPLES_FILEKEY]:
             self._samples_datasetid = self._provenance[CellmapsImageDownloader.SAMPLES_FILEKEY]['guid']
+            return
+
+        # if input file for samples was not set then write the samples we
+        # have to the output directory and use that path as dataset to register
+        if self._input_data_dict is None or CellmapsImageDownloader.SAMPLES_FILEKEY not in self._input_data_dict:
+            samples_file = os.path.join(self._outdir, 'samplescopy.csv')
+            self._imagegen.write_samples_to_csvfile(csvfile=samples_file)
+            skip_samples_copy = True
+        else:
+            samples_file = self._input_data_dict[CellmapsImageDownloader.SAMPLES_FILEKEY]
+            skip_samples_copy = False
+
+        # add samples dataset
+        self._samples_datasetid = self._add_dataset_to_crate(
+            data_dict=self._provenance[CellmapsImageDownloader.SAMPLES_FILEKEY],
+            source_file=samples_file,
+            skip_copy=skip_samples_copy)
+        logger.debug('Samples dataset id: ' + str(self._samples_datasetid))
+
+    def _register_unique_dataset(self):
+        """
+
+        :return:
+        """
         if 'guid' in self._provenance[CellmapsImageDownloader.UNIQUE_FILEKEY]:
             self._unique_datasetid = self._provenance[CellmapsImageDownloader.UNIQUE_FILEKEY]['guid']
-
-        if self._samples_datasetid is not None and self._unique_datasetid is not None:
-            logger.debug('Both samples and unique have dataset ids. Just returning')
             return
 
-        if self._samples_datasetid is None:
-            # write file and add samples dataset
-            self._samples_datasetid = self._add_dataset_to_crate(data_dict=self._provenance[CellmapsImageDownloader.SAMPLES_FILEKEY],
-                                                                 source_file=self._input_data_dict[CellmapsImageDownloader.SAMPLES_FILEKEY],
-                                                                 skip_copy=False)
-            logger.debug('Samples dataset id: ' + str(self._samples_datasetid))
-
-        if self._unique_datasetid is None:
-            # write file and add unique dataset
-            self._unique_datasetid = self._add_dataset_to_crate(data_dict=self._provenance[CellmapsImageDownloader.UNIQUE_FILEKEY],
-                                                                source_file=self._input_data_dict[CellmapsImageDownloader.UNIQUE_FILEKEY],
-                                                                skip_copy=False)
-            logger.debug('Unique dataset id: ' + str(self._unique_datasetid))
+        # if input file for unique list was not set then write the unique list we
+        # have to the output directory and use that path as dataset to register
+        if self._input_data_dict is None or CellmapsImageDownloader.UNIQUE_FILEKEY not in self._input_data_dict:
+            unique_file = os.path.join(self._outdir, 'uniquecopy.csv')
+            self._imagegen.write_unique_list_to_csvfile(csvfile=unique_file)
+            skip_unique_copy = True
+        else:
+            unique_file = self._input_data_dict[CellmapsImageDownloader.UNIQUE_FILEKEY]
+            skip_unique_copy = False
+
+        # add unique dataset
+        self._unique_datasetid = self._add_dataset_to_crate(
+            data_dict=self._provenance[CellmapsImageDownloader.UNIQUE_FILEKEY],
+            source_file=unique_file,
+            skip_copy=skip_unique_copy)
+        logger.debug('Unique dataset id: ' + str(self._unique_datasetid))
 
     def _register_downloaded_images(self):
         """
         Registers all the downloaded images
         :return:
         """
         data_dict = {'name': cellmaps_imagedownloader.__name__ + ' downloaded image file',
@@ -496,39 +532,26 @@
         :rtype: dict
         """
         color_d_map = {}
         for c in constants.COLORS:
             color_d_map[c] = os.path.join(self._outdir, c)
         return color_d_map
 
-    def _get_sample_url_and_filename(self, sample=None, color=None):
+    def _get_download_tuples(self):
         """
-
-        :param sample:
-        :return:
-        """
-        file_name = sample['if_plate_id'] + '_' + sample['position'] + '_' + sample['sample'] + '_' + color + self._imgsuffix
-        return self._image_url + '/' + re.sub('^HPA0*|^CAB0*', '', sample['antibody']) + '/' + file_name, file_name
-
-    def _get_download_tuples_from_csv(self):
-        """
-        Gets download list from CSV file for the 4 colors
+        Gets download list from **imageurlgen** object set via constructor
 
         :return: list of (image download URL prefix,
                           file path where image should be written)
         :rtype: list
         """
         dtuples = []
-
-        color_d_map = self._get_color_download_map()
-        for row in self._imagegen.get_samples_list():
-            for c in constants.COLORS:
-                image_url, file_name = self._get_sample_url_and_filename(sample=row, color=c)
-                dtuples.append((image_url,
-                                os.path.join(color_d_map[c], file_name)))
+        color_map = self._get_color_download_map()
+        for image_url, image_dest in self._imageurlgen.get_next_image_url(color_map):
+            dtuples.append((image_url, image_dest))
         return dtuples
 
     def _write_task_start_json(self):
         """
         Writes task_start.json file with information about
         what is to be run
 
@@ -563,77 +586,96 @@
     def _download_images(self, max_retry=5):
         """
         Uses downloader specified in constructor to download images noted in
         tsvfile file also specified in constructor
 
         :raises CellMapsImageDownloaderError: if image downloader is ``None`` or
                                          if there are failed downloads
-        :return: 0 upon success otherwise, failure
-        :rtype: int
+        :return: (int with value of 0 upon success otherwise failure, list of failed downloads)
+        :rtype: tuple
         """
         if self._imagedownloader is None:
             raise CellMapsImageDownloaderError('Image downloader is None')
 
-        downloadtuples = self._get_download_tuples_from_csv()
+        downloadtuples = self._get_download_tuples()
 
         failed_downloads = self._imagedownloader.download_images(downloadtuples)
         retry_count = 0
         while len(failed_downloads) > 0 and retry_count < max_retry:
             retry_count += 1
             logger.error(str(len(failed_downloads)) +
                          ' images failed to download. Retrying #' + str(retry_count))
 
             # try one more time with files that failed
             failed_downloads = self._retry_failed_images(failed_downloads=failed_downloads)
 
         if len(failed_downloads) > 0 and (self._skip_failed is None or self._skip_failed is False):
             raise CellMapsImageDownloaderError('Failed to download: ' +
                                                str(len(failed_downloads)) + ' images')
-        return 0
+        return 0, failed_downloads
 
-    def get_image_gene_node_attributes_file(self):
+    def get_image_gene_node_attributes_file(self, fold):
         """
         Gets full path to image gene node attribute file under output directory
         created when invoking :py:meth:`~cellmaps_imagedownloader.runner.CellmapsImageDownloader.run`
 
         :return: Path to file
         :rtype: str
         """
-        return os.path.join(self._outdir,
+        return os.path.join(self._outdir, str(fold) + '_' +
                             constants.IMAGE_GENE_NODE_ATTR_FILE)
 
     def get_image_gene_node_errors_file(self):
         """
         Gets full path to image gene node attribute errors file under output directory
         created when invoking :py:meth:`~cellmaps_imagedownloader.runner.CellmapsImageDownloader.run`
 
         :return: Path to file
         :rtype: str
         """
         return os.path.join(self._outdir,
                             constants.IMAGE_GENE_NODE_ERRORS_FILE)
 
-    def _write_image_gene_node_attrs(self, gene_node_attrs=None,
+    def _write_image_gene_node_attrs(self, gene_node_attrs=None, fold=1,
                                      errors=None):
         """
 
         :param gene_node_attrs:
         :param errors:
         :return:
         """
-        with open(self.get_image_gene_node_attributes_file(), 'w', newline='') as f:
+        with open(self.get_image_gene_node_attributes_file(fold), 'w', newline='') as f:
             writer = csv.DictWriter(f, fieldnames=constants.IMAGE_GENE_NODE_COLS, delimiter='\t')
             writer.writeheader()
             for key in gene_node_attrs:
                 writer.writerow(gene_node_attrs[key])
         if errors is not None:
             with open(self.get_image_gene_node_errors_file(), 'w') as f:
                 for e in errors:
                     f.write(str(e) + '\n')
 
+    def _add_imageurl_to_gene_node_attrs(self, gene_node_attrs=None):
+        """
+        Adds imageurl to **gene_node_attrs** passed in
+
+        :param gene_node_attrs:
+        :type gene_node_attrs: dict
+        """
+        sample_urlmap = self._imageurlgen.get_sample_urlmap()
+        for key in gene_node_attrs:
+            sample = gene_node_attrs[key]
+            image_id = re.sub('^HPA0*|^CAB0*', '', sample['antibody']) + '/' + \
+                       sample['filename']
+            if image_id in sample_urlmap:
+                gene_node_attrs[key][constants.IMAGE_GENE_NODE_IMAGEURL_COL] = sample_urlmap[image_id]
+            else:
+                # this should NOT happen, but just in case
+                logger.error(image_id + ' not in sample urlmap. setting to no image url found')
+                gene_node_attrs[key][constants.IMAGE_GENE_NODE_IMAGEURL_COL] = 'no image url found'
+
     def run(self):
         """
         Downloads images to output directory specified in constructor
         using tsvfile for list of images to download
 
         :raises CellMapsImageDownloaderError: If there is an error
         :return: 0 upon success, otherwise failure
@@ -643,28 +685,30 @@
             self._create_output_directory()
             if self._skip_logging is False:
                 logutils.setup_filelogger(outdir=self._outdir,
                                           handlerprefix='cellmaps_imagedownloader')
                 self._write_task_start_json()
 
             self._create_run_crate()
-            self._register_input_datasets()
+            self._register_samples_dataset()
+            self._register_unique_dataset()
 
             self._register_software()
 
-            # write image attribute data
-            image_gene_node_attrs, errors = self._imagegen.get_gene_node_attributes()
+            exitcode, failed_downloads = self._download_images()
+            # todo need to validate downloaded image data
 
             # write image attribute data
-            self._write_image_gene_node_attrs(image_gene_node_attrs, errors)
+            for fold in [1, 2]:
+                image_gene_node_attrs, errors = self._imagegen.get_gene_node_attributes(fold)
+                self._add_imageurl_to_gene_node_attrs(gene_node_attrs=image_gene_node_attrs)
+                # write image attribute data
+                self._write_image_gene_node_attrs(image_gene_node_attrs, fold, errors)
 
-            self._register_image_gene_node_attrs()
-
-            exitcode = self._download_images()
-            # todo need to validate downloaded image data
+                self._register_image_gene_node_attrs(fold)
 
             # Todo: Right now only registering 2,000 images. need to fix
             self._register_downloaded_images()
 
             self._register_computation()
 
             return exitcode
```

### Comparing `cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/PKG-INFO` & `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cellmaps-imagedownloader
-Version: 0.1.0a5
-Summary: Downloads IF data needed for CM4AI MuSIC pipeline
+Version: 0.1.0a6
+Summary: A tool to download specified image data from the Human Protein Atlas website using CSV file
 Home-page: https://github.com/idekerlab/cellmaps_imagedownloader
-Author: Gege Qian
-Author-email: geqian@ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
 Description: =========================
         cellmaps_imagedownloader
         =========================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_imagedownloader.svg
@@ -52,15 +52,15 @@
         **Or directly from source:**
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_imagedownloader
            cd cellmaps_imagedownloader
            make dist
-           pip install dist/cellmaps_imagedownloadercmd*whl
+           pip install dist/cellmaps_imagedownloader*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_imagedownloader-0.1.0a5/cellmaps_imagedownloader.egg-info/SOURCES.txt` & `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 README.rst
 setup.cfg
 setup.py
 cellmaps_imagedownloader/__init__.py
 cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py
 cellmaps_imagedownloader/exceptions.py
 cellmaps_imagedownloader/gene.py
+cellmaps_imagedownloader/proteinatlas.py
 cellmaps_imagedownloader/runner.py
 cellmaps_imagedownloader.egg-info/PKG-INFO
 cellmaps_imagedownloader.egg-info/SOURCES.txt
 cellmaps_imagedownloader.egg-info/dependency_links.txt
 cellmaps_imagedownloader.egg-info/not-zip-safe
 cellmaps_imagedownloader.egg-info/requires.txt
 cellmaps_imagedownloader.egg-info/top_level.txt
@@ -38,12 +39,15 @@
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 tests/__init__.py
 tests/test_cellmaps_imagedownloadercmd.py
 tests/test_cellmapsimagedownloader.py
 tests/test_genenodegenerator.py
 tests/test_genequery.py
+tests/test_imagedownloadtuplegenerator.py
 tests/test_imagegenenodegenerator.py
 tests/test_integration_cellmaps_downloader.py
 tests/test_multiprocessimagedownloader.py
+tests/test_proteinatlasimageurlreader.py
+tests/test_proteinatlasreader.py
 tests/data/test_single_sample.tsv
 tests/data/test_single_unique.tsv
```

### Comparing `cellmaps_imagedownloader-0.1.0a5/docs/Makefile` & `cellmaps_imagedownloader-0.1.0a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/docs/cellmaps_imagedownloader.rst` & `cellmaps_imagedownloader-0.1.0a6/docs/cellmaps_imagedownloader.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/docs/conf.py` & `cellmaps_imagedownloader-0.1.0a6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/docs/installation.rst` & `cellmaps_imagedownloader-0.1.0a6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/docs/make.bat` & `cellmaps_imagedownloader-0.1.0a6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/docs/newrelease.rst` & `cellmaps_imagedownloader-0.1.0a6/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/docs/pypircfile.rst` & `cellmaps_imagedownloader-0.1.0a6/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/docs/usage.rst` & `cellmaps_imagedownloader-0.1.0a6/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/docs/versioningscheme.rst` & `cellmaps_imagedownloader-0.1.0a6/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/setup.py` & `cellmaps_imagedownloader-0.1.0a6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,25 @@
 import os
 import re
 from setuptools import setup, find_packages
 
 
 with open(os.path.join('cellmaps_imagedownloader', '__init__.py')) as ver_file:
     for line in ver_file:
+        line = line.rstrip()
         if line.startswith('__version__'):
             version=re.sub("'", "", line[line.index("'"):])
+        elif line.startswith('__description__'):
+            desc = re.sub("'", "", line[line.index("'"):])
+        elif line.startswith('__repo_url__'):
+            repo_url = re.sub("'", "", line[line.index("'"):])
+        elif line.startswith('__author__'):
+            author = re.sub("'", "", line[line.index("'"):])
+        elif line.startswith('__email__'):
+            email = re.sub("'", "", line[line.index("'"):])
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
@@ -24,36 +33,36 @@
                 'tqdm']
 
 setup_requirements = [ ]
 
 test_requirements = ['requests_mock']
 
 setup(
-    author="Gege Qian",
-    author_email='geqian@ucsd.edu',
+    author=author,
+    author_email=email,
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
-    description="Downloads IF data needed for CM4AI MuSIC pipeline",
+    description=desc,
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/x-rst',
     include_package_data=True,
     keywords='cellmaps_imagedownloader',
     name='cellmaps_imagedownloader',
     packages=find_packages(include=['cellmaps_imagedownloader']),
     package_dir={'cellmaps_imagedownloader': 'cellmaps_imagedownloader'},
     scripts=['cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py'],
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/idekerlab/cellmaps_imagedownloader',
+    url=repo_url,
     version=version,
     zip_safe=False)
```

### Comparing `cellmaps_imagedownloader-0.1.0a5/tests/test_cellmaps_imagedownloadercmd.py` & `cellmaps_imagedownloader-0.1.0a6/tests/test_cellmaps_imagedownloadercmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/tests/test_genequery.py` & `cellmaps_imagedownloader-0.1.0a6/tests/test_genequery.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/tests/test_integration_cellmaps_downloader.py` & `cellmaps_imagedownloader-0.1.0a6/tests/test_integration_cellmaps_downloader.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a5/tests/test_multiprocessimagedownloader.py` & `cellmaps_imagedownloader-0.1.0a6/tests/test_multiprocessimagedownloader.py`

 * *Files identical despite different names*

