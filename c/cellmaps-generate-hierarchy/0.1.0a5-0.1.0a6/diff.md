# Comparing `tmp/cellmaps_generate_hierarchy-0.1.0a5.tar.gz` & `tmp/cellmaps_generate_hierarchy-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_generate_hierarchy-0.1.0a5.tar", last modified: Tue May 30 23:33:02 2023, max compression
+gzip compressed data, was "dist/cellmaps_generate_hierarchy-0.1.0a6.tar", last modified: Mon Jul 17 19:17:10 2023, max compression
```

## Comparing `cellmaps_generate_hierarchy-0.1.0a5.tar` & `cellmaps_generate_hierarchy-0.1.0a6.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.292047 cellmaps_generate_hierarchy-0.1.0a5/
--rw-r--r--   0 churas     (504) staff       (20)      160 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3761 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 20:13:29.000000 cellmaps_generate_hierarchy-0.1.0a5/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-30 23:33:02.292175 cellmaps_generate_hierarchy-0.1.0a5/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4203 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a5/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.282418 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/
--rw-r--r--   0 churas     (504) staff       (20)      325 2023-05-30 23:32:46.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     5391 2023-05-30 23:32:46.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
--rw-r--r--   0 churas     (504) staff       (20)      151 2023-05-10 16:59:50.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    17184 2023-05-30 23:32:46.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/hierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     3764 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/ppi.py
--rw-r--r--   0 churas     (504) staff       (20)    12203 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.284170 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1429 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       56 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.288662 cellmaps_generate_hierarchy-0.1.0a5/docs/
--rw-r--r--   0 churas     (504) staff       (20)      628 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.277776 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.277860 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.289471 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1294 2023-05-22 23:59:36.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/cellmaps_generate_hierarchy.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6155 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)     1004 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1269 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      481 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      825 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       86 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4460 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      797 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      757 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      410 2023-05-30 23:33:02.292610 cellmaps_generate_hierarchy-0.1.0a5/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2310 2023-05-25 23:23:13.000000 cellmaps_generate_hierarchy-0.1.0a5/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.290914 cellmaps_generate_hierarchy-0.1.0a5/tests/
--rw-r--r--   0 churas     (504) staff       (20)       82 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/__init__.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.291865 cellmaps_generate_hierarchy-0.1.0a5/tests/data/
--rw-r--r--   0 churas     (504) staff       (20)    10232 2023-05-10 19:56:53.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/data/fake_4_node_coembedding.tsv
--rw-r--r--   0 churas     (504) staff       (20)       30 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/data/hidef_output.edges
--rw-r--r--   0 churas     (504) staff       (20)       62 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/data/hidef_output.nodes
--rw-r--r--   0 churas     (504) staff       (20)    10675 2023-05-30 23:32:46.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/test_cdapshierarchygenerator.py
--rw-r--r--   0 churas     (504) staff       (20)     1840 2023-05-19 20:32:56.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/test_cellmaps_generate_hierarchycmd.py
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-05-11 00:02:17.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/test_cellmapsgeneratehierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     1512 2023-05-10 21:34:27.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/test_cosinesimilarityppigenerator.py
--rw-r--r--   0 churas     (504) staff       (20)      842 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/test_integration_cellmaps_generate_hierarchy.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.066891 cellmaps_generate_hierarchy-0.1.0a6/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-12 20:22:02.000000 cellmaps_generate_hierarchy-0.1.0a6/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3761 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 20:13:29.000000 cellmaps_generate_hierarchy-0.1.0a6/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6212 2023-07-17 19:17:10.067054 cellmaps_generate_hierarchy-0.1.0a6/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4098 2023-06-12 20:22:02.000000 cellmaps_generate_hierarchy-0.1.0a6/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.056083 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/
+-rw-r--r--   0 churas     (504) staff       (20)      341 2023-06-12 20:22:02.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     7220 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      151 2023-05-10 16:59:50.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    20579 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/hierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)    25885 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/maturehierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     3877 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/ppi.py
+-rw-r--r--   0 churas     (504) staff       (20)    12203 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.057457 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6212 2023-07-17 19:17:09.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1521 2023-07-17 19:17:10.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:17:09.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:17:09.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       62 2023-07-17 19:17:09.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-07-17 19:17:09.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.062993 cellmaps_generate_hierarchy-0.1.0a6/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      628 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.051189 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.051256 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.063971 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1294 2023-05-22 23:59:36.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/cellmaps_generate_hierarchy.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6155 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1004 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1269 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      481 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      825 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       86 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4460 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      797 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      757 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      133 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/pyproject.toml
+-rw-r--r--   0 churas     (504) staff       (20)      410 2023-07-17 19:17:10.067602 cellmaps_generate_hierarchy-0.1.0a6/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2335 2023-06-08 20:03:18.000000 cellmaps_generate_hierarchy-0.1.0a6/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.065823 cellmaps_generate_hierarchy-0.1.0a6/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       82 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.066647 cellmaps_generate_hierarchy-0.1.0a6/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)    10232 2023-05-10 19:56:53.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/data/fake_4_node_coembedding.tsv
+-rw-r--r--   0 churas     (504) staff       (20)       30 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/data/hidef_output.edges
+-rw-r--r--   0 churas     (504) staff       (20)       62 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/data/hidef_output.nodes
+-rw-r--r--   0 churas     (504) staff       (20)    12745 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_cdapshierarchygenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)     1840 2023-05-19 20:32:56.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_cellmaps_generate_hierarchycmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-05-11 00:02:17.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_cellmapsgeneratehierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     1512 2023-05-10 21:34:27.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_cosinesimilarityppigenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)      842 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_integration_cellmaps_generate_hierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     5638 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_maturehierarchy.py
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/CONTRIBUTING.rst` & `cellmaps_generate_hierarchy-0.1.0a6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/LICENSE` & `cellmaps_generate_hierarchy-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/PKG-INFO` & `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: cellmaps_generate_hierarchy
-Version: 0.1.0a5
+Name: cellmaps-generate-hierarchy
+Version: 0.1.0a6
 Summary: A tool to generate hierarchies from protein to protein interaction networks
 Home-page: https://github.com/idekerlab/cellmaps_generate_hierarchy
-Author: Clara Hu
-Author-email: mhu@ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
 Description: ========================
         CM4AI Generate Hierarchy
         ========================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_generate_hierarchy.svg
@@ -32,23 +32,17 @@
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         * `pandas <https://pypi.org/project/pandas>`__
         * `numpy <https://pypi.org/project/numpy>`__
         * `ndex2 <https://pypi.org/project/ndex2>`__
-        * `HiDeF <https://github.com/fanzheng10/HiDeF>`__
-           HiDeF must be built directly from source which can be done by running the following commands:
+        * `HiDeF <https://pypi.org/project/hidef>`__
+           **Note:** If running HiDeF in parallel on same machine it must be built directly from `source <https://github.com/fanzheng10/HiDeF>`__
         
-          .. code-block:: python
-        
-            git clone https://github.com/fanzheng10/HiDeF.git
-            cd HiDeF
-            make dist
-            pip install dist/hidef*whl
         
         
         
         
         Compatibility
         -------------
         
@@ -58,15 +52,15 @@
         ------------
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_generate_hierarchy
            cd cellmaps_generate_hierarchy
            make dist
-           pip install dist/cellmaps_generate_hierarchycmd*whl
+           pip install dist/cellmaps_generate_hierarchy*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/README.rst` & `cellmaps_generate_hierarchy-0.1.0a6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,17 @@
 ------------
 
 * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
 * `tqdm <https://pypi.org/project/tqdm>`__
 * `pandas <https://pypi.org/project/pandas>`__
 * `numpy <https://pypi.org/project/numpy>`__
 * `ndex2 <https://pypi.org/project/ndex2>`__
-* `HiDeF <https://github.com/fanzheng10/HiDeF>`__
-   HiDeF must be built directly from source which can be done by running the following commands:
+* `HiDeF <https://pypi.org/project/hidef>`__
+   **Note:** If running HiDeF in parallel on same machine it must be built directly from `source <https://github.com/fanzheng10/HiDeF>`__
 
-  .. code-block:: python
-
-    git clone https://github.com/fanzheng10/HiDeF.git
-    cd HiDeF
-    make dist
-    pip install dist/hidef*whl
 
 
 
 
 Compatibility
 -------------
 
@@ -50,15 +44,15 @@
 ------------
 
 .. code-block::
 
    git clone https://github.com/idekerlab/cellmaps_generate_hierarchy
    cd cellmaps_generate_hierarchy
    make dist
-   pip install dist/cellmaps_generate_hierarchycmd*whl
+   pip install dist/cellmaps_generate_hierarchy*whl
 
 
 Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
 
 .. code-block::
 
    make
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/hierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/hierarchy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 import os
+import sys
 import csv
 import logging
 import subprocess
 from datetime import date
 import ndex2
 import cdapsutil
 import cellmaps_generate_hierarchy
@@ -58,33 +59,47 @@
 
     CDAPS_JSON_FILE = 'cdaps.json'
 
     EDGELIST_TSV = '.id.edgelist.tsv'
 
     HIDEF_OUT_PREFIX = 'hidef_output'
 
+    TRANSLATED_HIDEF_OUT_PREFIX = 'hidefnames_output'
+
     CDRES_KEY_NAME = 'communityDetectionResult'
 
     NODE_CX_KEY_NAME = 'nodeAttributesAsCX2'
 
     ATTR_DEC_NAME = 'attributeDeclarations'
 
     PERSISTENCE_COL_NAME = 'HiDeF_persistence'
 
     def __init__(self, hidef_cmd='hidef_finder.py',
                  provenance_utils=ProvenanceUtil(),
+                 refiner=None,
                  author='cellmaps_generate_hierarchy',
                  version=cellmaps_generate_hierarchy.__version__):
         """
-        Constructor
+
+        :param hidef_cmd: HiDeF command line binary
+        :type hidef_cmd: str
+        :param provenance_utils:
+        :param author:
+        :type author: str
+        :param version:
         """
         super().__init__(provenance_utils=provenance_utils,
                          author=author,
                          version=version)
-        self._hidef_cmd = hidef_cmd
+        self._refiner = refiner
+        self._python = sys.executable
+        if os.sep not in hidef_cmd:
+            self._hidef_cmd = os.path.join(os.path.dirname(self._python), hidef_cmd)
+        else:
+            self._hidef_cmd = hidef_cmd
 
     def _get_max_node_id(self, nodes_file):
         """
         Examines the 'nodes_file' passed in and finds the value of
         highest node id.
 
         It is assumed the 'nodes_file' a tab delimited
@@ -247,35 +262,35 @@
         :type out_stream: file like object
         :param outdir:
         :type outdir: str
         :return: None
         """
         nodefile = os.path.join(outdir,
                                 CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX +
-                                '.nodes')
+                                '.pruned.nodes')
         max_node_id = self._get_max_node_id(nodefile)
         cluster_node_map = {}
         persistence_map = {}
         out_stream.write('{"communityDetectionResult": "')
         with open(nodefile, 'r') as csvfile:
             linereader = csv.reader(csvfile, delimiter='\t')
             for row in linereader:
                 max_node_id, cur_node_id = self.update_cluster_node_map(cluster_node_map,
                                                                         row[0],
                                                                         max_node_id)
                 self.update_persistence_map(persistence_map, cur_node_id, row[-1])
                 self.write_members_for_row(out_stream, row,
                                       cur_node_id)
-        edge_file = os.path.join(outdir, CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX + '.edges')
+        edge_file = os.path.join(outdir, CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX + '.pruned.edges')
         self.write_communities(out_stream, edge_file, cluster_node_map)
         self.write_persistence_node_attribute(out_stream, persistence_map)
         out_stream.write('\n')
         return None
 
-    def _run_cmd(self, cmd, cwd=None, timeout=3600):
+    def _run_cmd(self, cmd, cwd=None, timeout=36000):
         """
         Runs command as a command line process
 
         :param cmd_to_run: command to run as list
         :type cmd_to_run: list
         :return: (return code, standard out, standard error)
         :rtype: tuple
@@ -294,44 +309,91 @@
             raise CellmapsGenerateHierarchyError('Process timed out. exit code: ' +
                                                  str(p.returncode) +
                                                  ' stdout: ' + str(out) +
                                                  ' stderr: ' + str(err))
 
         return p.returncode, out, err
 
+    def _get_largest_network(self, networks):
+        """
+        Finds largest network by file size
+
+        :param networks: list of :py:class:`~ndex2.nice_cx_network.NiceCXNetwork` objects
+        :type networks: list
+        :return: Largest network
+        :rtype: :py:class:`~ndex2.nice_cx_network.NiceCXNetwork`
+        """
+        largest_network = None
+        max_file_size = 0
+        for n in networks:
+            file_size = os.path.getsize(n + constants.CX_SUFFIX)
+            if file_size >= max_file_size:
+                largest_network = n
+                max_file_size = file_size
+        return largest_network
+
+    def _get_name_to_id_dict(self, network):
+        """
+
+        :param network:
+        :return:
+        """
+        name_to_id = {}
+        for node_id, node_obj in network.get_nodes():
+            name_to_id[node_obj['n']] = node_id
+        return name_to_id
+
+    def _get_id_to_name_dict(self, network):
+        """
+
+        :param network:
+        :return:
+        """
+        id_to_name = {}
+        for node_id, node_obj in network.get_nodes():
+            id_to_name[node_id] = node_obj['n']
+        return id_to_name
+
     def _create_edgelist_files_for_networks(self, networks):
         """
         Iterates through **networks** prefix paths and loads the
         CX files. Method then creates a PREFIX_PATH
         :py:const:`CDAPSHiDeFHierarchyGenerator.EDGELIST_TSV`
         file for each network and returns those paths as a list
 
         :param networks: Prefix paths of input PPI networks
         :type networks: list
-        :return: (:py:class:`~ndex2.nice_cx_network.NiceCXNetwork`, :py:class:`list`)
+        :return: (largest network path,
+                  :py:class:`~ndex2.nice_cx_network.NiceCXNetwork`,
+                  :py:class:`list`)
         :rtype: tuple
         """
         net_paths = []
-        largest_network = None
-        max_edge_count = 0
+
+        largest_network_path = self._get_largest_network(networks)
+        largest_network = ndex2.create_nice_cx_from_file(largest_network_path + constants.CX_SUFFIX)
+        logger.debug('Largest network name: ' + largest_network.get_name())
+        largest_name_to_id = self._get_name_to_id_dict(largest_network)
+
         for n in networks:
-            logger.debug('Creating NiceCXNetwork object from: ' + n + constants.CX_SUFFIX)
-            net = ndex2.create_nice_cx_from_file(n + constants.CX_SUFFIX)
+            if largest_network_path == n:
+                net = largest_network
+            else:
+                logger.debug('Creating NiceCXNetwork object from: ' + n + constants.CX_SUFFIX)
+                net = ndex2.create_nice_cx_from_file(n + constants.CX_SUFFIX)
             dest_path = n + CDAPSHiDeFHierarchyGenerator.EDGELIST_TSV
             net_paths.append(dest_path)
-            edge_count = 0
             logger.debug('Writing out id edgelist: ' + str(dest_path))
+            id_to_name = self._get_id_to_name_dict(net)
             with open(dest_path, 'w') as f:
                 for edge_id, edge_obj in net.get_edges():
-                    f.write(str(edge_obj['s']) + '\t' + str(edge_obj['t']) + '\n')
-                    edge_count += 1
-
-            # find the largest network by edge count
-            if edge_count >= max_edge_count:
-                largest_network = net
+                    f.write(str(largest_name_to_id[id_to_name[edge_obj['s']]]) +
+                            '\t' +
+                            str(largest_name_to_id[id_to_name[edge_obj['t']]]) +
+                            '\n')
 
                 # register edgelist file with fairscape
                 data_dict = {'name': os.path.basename(dest_path) +
                              ' PPI id edgelist file',
                              'description': 'PPI id edgelist file',
                              'data-format': 'tsv',
                              'author': str(self._author),
@@ -339,15 +401,16 @@
                              'date-published': date.today().strftime('%m-%d-%Y')}
                 dataset_id = self._provenance_utils.register_dataset(os.path.dirname(dest_path),
                                                                      source_file=dest_path,
                                                                      data_dict=data_dict)
                 self._generated_dataset_ids.append(dataset_id)
 
         logger.debug('Largest network name: ' + largest_network.get_name())
-        return largest_network, net_paths
+        return (largest_network_path + constants.CX_SUFFIX,
+                largest_network, net_paths)
 
     def _register_hidef_output_files(self, outdir):
         """
         Register <HIDEF_PREFIX>.nodes and <HIDEF_PREFIX>.edges
         and <HIDEF_PREFIX>.weaver files with FAIRSCAPE
 
         """
@@ -366,14 +429,32 @@
                          'version': str(self._version),
                          'date-published': date.today().strftime('%m-%d-%Y')}
             dataset_id = self._provenance_utils.register_dataset(os.path.dirname(outfile),
                                                                  source_file=outfile,
                                                                  data_dict=data_dict)
             self._generated_dataset_ids.append(dataset_id)
 
+    def _annotate_hierarchy(self, network=None, path=None):
+        """
+        Adds HCX attributes to network as well as sets
+
+        ``prov:wasGeneratedBy`` to the name and version of this tool
+
+        ``prov:wasDerivedFrom`` to FAIRSCAPE dataset id of this rocrate
+
+        :param network: Hierarchy
+        :type network: :py:class:`~ndex2.nice_cx_network.NiceCXNetwork`
+        :param path: Path to largest PPI network in CX or CX2 format
+        :type path: str
+        """
+        network.set_network_attribute(name='prov:wasGeneratedBy',
+                                      values=self._author + ' ' + self._version)
+        network.set_network_attribute(name='prov:wasDerivedFrom',
+                                      values='RO-crate: ' + os.path.dirname(path))
+
     def get_hierarchy(self, networks):
         """
         Runs HiDeF to generate hierarchy and registers resulting output
         files with FAIRSCAPE. To do this the method generates edgelist
         files from the CX files corresponding to the **networks** using
         the internal node ids for edge source and target names. These
         files are written to the same directory as the **networks**
@@ -393,30 +474,38 @@
         :type networks: list
         :raises CellmapsGenerateHierarchyError: If there was an error
         :return: Resulting hierarchy or ``None`` if no hierarchy from HiDeF
         :rtype: :py:class:`~ndex2.nice_cx_network.NiceCXNetwork`
         """
         outdir = os.path.dirname(networks[0])
 
-        largest_net, edgelist_files = self._create_edgelist_files_for_networks(networks)
+        (largest_net_path, largest_net,
+         edgelist_files) = self._create_edgelist_files_for_networks(networks)
 
-        cmd = [self._hidef_cmd, '--g']
+        cmd = [self._python, self._hidef_cmd, '--g']
         cmd.extend(edgelist_files)
-        cmd.extend(['--o', os.path.join(outdir, CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX),
-                    '--alg', 'leiden', '--maxres', '40', '--k', '10',
+        outputprefix = os.path.join(outdir, CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX)
+        cmd.extend(['--o', outputprefix,
+                    '--alg', 'leiden', '--maxres', '80', '--k', '10',
                     '--skipgml'])
 
         exit_code, out, err = self._run_cmd(cmd)
+
         if exit_code != 0:
             logger.error('Cmd failed with exit code: ' + str(exit_code) +
                          ' : ' + str(out) + ' : ' + str(err))
+            raise CellmapsGenerateHierarchyError('Cmd failed with exit code: ' + str(exit_code) +
+                                                 ' : ' + str(out) + ' : ' + str(err))
 
         self._register_hidef_output_files(outdir)
 
         try:
+            if self._refiner is not None:
+                self._refiner.refine_hierarchy(outprefix=outputprefix)
+
             cdaps_out_file = os.path.join(outdir,
                                           CDAPSHiDeFHierarchyGenerator.CDAPS_JSON_FILE)
             with open(cdaps_out_file, 'w') as out_stream:
                 self.convert_hidef_output_to_cdaps(out_stream, outdir)
 
             # register cdaps json file with fairscape
             data_dict = {'name': os.path.basename(cdaps_out_file) +
@@ -428,12 +517,14 @@
                          'date-published': date.today().strftime('%m-%d-%Y')}
             dataset_id = self._provenance_utils.register_dataset(os.path.dirname(cdaps_out_file),
                                                                  source_file=cdaps_out_file,
                                                                  data_dict=data_dict)
             self._generated_dataset_ids.append(dataset_id)
 
             cd = cdapsutil.CommunityDetection(runner=cdapsutil.ExternalResultsRunner())
-            return cd.run_community_detection(largest_net, algorithm=cdaps_out_file)
+            hier = cd.run_community_detection(largest_net, algorithm=cdaps_out_file)
+            self._annotate_hierarchy(network=hier, path=largest_net_path)
+            return hier
 
         except FileNotFoundError as fe:
             logger.error('No output from hidef: ' + str(fe) + '\n')
         return None
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/ppi.py` & `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/ppi.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,16 +37,19 @@
 
     .. code-block::
 
         ID # # # #
 
     Where ID is gene and #'s is embedding vector
     """
+
     def __init__(self, embeddingdir=None,
-                 cutoffs=[0.001, 0.002, 0.005, 0.01, 0.02, 0.05]):
+                 cutoffs=[0.001, 0.002, 0.003, 0.004, 0.005,
+                          0.006, 0.007, 0.008, 0.009, 0.01,
+                          0.02, 0.03, 0.04, 0.05, 0.10]):
         """
         Constructor
         """
         super().__init__()
         if embeddingdir is None:
             raise CellmapsGenerateHierarchyError('embeddingdir is None')
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/runner.py` & `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/runner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/PKG-INFO` & `cellmaps_generate_hierarchy-0.1.0a6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: cellmaps-generate-hierarchy
-Version: 0.1.0a5
+Name: cellmaps_generate_hierarchy
+Version: 0.1.0a6
 Summary: A tool to generate hierarchies from protein to protein interaction networks
 Home-page: https://github.com/idekerlab/cellmaps_generate_hierarchy
-Author: Clara Hu
-Author-email: mhu@ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
 Description: ========================
         CM4AI Generate Hierarchy
         ========================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_generate_hierarchy.svg
@@ -32,23 +32,17 @@
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         * `pandas <https://pypi.org/project/pandas>`__
         * `numpy <https://pypi.org/project/numpy>`__
         * `ndex2 <https://pypi.org/project/ndex2>`__
-        * `HiDeF <https://github.com/fanzheng10/HiDeF>`__
-           HiDeF must be built directly from source which can be done by running the following commands:
+        * `HiDeF <https://pypi.org/project/hidef>`__
+           **Note:** If running HiDeF in parallel on same machine it must be built directly from `source <https://github.com/fanzheng10/HiDeF>`__
         
-          .. code-block:: python
-        
-            git clone https://github.com/fanzheng10/HiDeF.git
-            cd HiDeF
-            make dist
-            pip install dist/hidef*whl
         
         
         
         
         Compatibility
         -------------
         
@@ -58,15 +52,15 @@
         ------------
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_generate_hierarchy
            cd cellmaps_generate_hierarchy
            make dist
-           pip install dist/cellmaps_generate_hierarchycmd*whl
+           pip install dist/cellmaps_generate_hierarchy*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/SOURCES.txt` & `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 cellmaps_generate_hierarchy/__init__.py
 cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
 cellmaps_generate_hierarchy/exceptions.py
 cellmaps_generate_hierarchy/hierarchy.py
+cellmaps_generate_hierarchy/maturehierarchy.py
 cellmaps_generate_hierarchy/ppi.py
 cellmaps_generate_hierarchy/runner.py
 cellmaps_generate_hierarchy.egg-info/PKG-INFO
 cellmaps_generate_hierarchy.egg-info/SOURCES.txt
 cellmaps_generate_hierarchy.egg-info/dependency_links.txt
 cellmaps_generate_hierarchy.egg-info/not-zip-safe
 cellmaps_generate_hierarchy.egg-info/requires.txt
@@ -40,10 +42,11 @@
 docs/_build/html/_static/plus.png
 tests/__init__.py
 tests/test_cdapshierarchygenerator.py
 tests/test_cellmaps_generate_hierarchycmd.py
 tests/test_cellmapsgeneratehierarchy.py
 tests/test_cosinesimilarityppigenerator.py
 tests/test_integration_cellmaps_generate_hierarchy.py
+tests/test_maturehierarchy.py
 tests/data/fake_4_node_coembedding.tsv
 tests/data/hidef_output.edges
 tests/data/hidef_output.nodes
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/docs/Makefile` & `cellmaps_generate_hierarchy-0.1.0a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/docs/cellmaps_generate_hierarchy.rst` & `cellmaps_generate_hierarchy-0.1.0a6/docs/cellmaps_generate_hierarchy.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/docs/conf.py` & `cellmaps_generate_hierarchy-0.1.0a6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/docs/index.rst` & `cellmaps_generate_hierarchy-0.1.0a6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/docs/installation.rst` & `cellmaps_generate_hierarchy-0.1.0a6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/docs/make.bat` & `cellmaps_generate_hierarchy-0.1.0a6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/docs/newrelease.rst` & `cellmaps_generate_hierarchy-0.1.0a6/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/docs/pypircfile.rst` & `cellmaps_generate_hierarchy-0.1.0a6/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/docs/usage.rst` & `cellmaps_generate_hierarchy-0.1.0a6/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/docs/versioningscheme.rst` & `cellmaps_generate_hierarchy-0.1.0a6/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/setup.py` & `cellmaps_generate_hierarchy-0.1.0a6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     history = history_file.read()
 
 requirements = ['cellmaps_utils',
                 'tqdm',
                 'pandas',
                 'numpy',
                 'ndex2>=3.5.1',
-                'cdapsutil']
+                'cdapsutil',
+                'hidef']
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
     author=author,
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/tests/data/fake_4_node_coembedding.tsv` & `cellmaps_generate_hierarchy-0.1.0a6/tests/data/fake_4_node_coembedding.tsv`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/tests/test_cdapshierarchygenerator.py` & `cellmaps_generate_hierarchy-0.1.0a6/tests/test_cdapshierarchygenerator.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import json
 import ndex2
 from io import StringIO
 
 from cellmaps_utils import constants
 import cellmaps_generate_hierarchy
 from cellmaps_generate_hierarchy.hierarchy import CDAPSHiDeFHierarchyGenerator
+from cellmaps_generate_hierarchy.exceptions import CellmapsGenerateHierarchyError
 from cellmaps_generate_hierarchy.hierarchy import CXHierarchyGenerator
 
 
 class TestCDAPSHierarchyGenerator(unittest.TestCase):
     """Tests for `CDAPSHierarchyGenerator`."""
 
     def setUp(self):
@@ -90,17 +91,17 @@
         self.assertEqual({1: 'val',
                           2: '2val'}, persistence_map)
 
     def test_convert_hidef_output_to_cdaps(self):
         temp_dir = tempfile.mkdtemp()
         try:
             shutil.copy(os.path.join(os.path.dirname(__file__), 'data', 'hidef_output.nodes'),
-                        os.path.join(temp_dir, 'hidef_output.nodes'))
+                        os.path.join(temp_dir, 'hidef_output.pruned.nodes'))
             shutil.copy(os.path.join(os.path.dirname(__file__), 'data', 'hidef_output.edges'),
-                        os.path.join(temp_dir, 'hidef_output.edges'))
+                        os.path.join(temp_dir, 'hidef_output.pruned.edges'))
             data = ''
             out_stream = StringIO(data)
             gen = CDAPSHiDeFHierarchyGenerator()
             self.assertIsNone(gen.convert_hidef_output_to_cdaps(out_stream,
                                                                 temp_dir))
 
             res = json.loads(out_stream.getvalue())
@@ -129,31 +130,32 @@
             one_edge_net_file = os.path.join(temp_dir, 'one_edge')
             cx_networks.append(one_edge_net_file)
             with open(one_edge_net_file + constants.CX_SUFFIX, 'w') as f:
                 json.dump(one_edge_net.to_cx(), f)
 
             two_edge_net = ndex2.nice_cx_network.NiceCXNetwork()
             two_edge_net.set_name('two')
-            n_one = two_edge_net.create_node('n3')
-            n_two = two_edge_net.create_node('n4')
+            n_one = two_edge_net.create_node('n1')
+            n_two = two_edge_net.create_node('n2')
             n_three = two_edge_net.create_node('n5')
             two_edge_net.create_edge(edge_source=n_one, edge_target=n_two)
             two_edge_net.create_edge(edge_source=n_two, edge_target=n_three)
             two_edge_net_file = os.path.join(temp_dir, 'two_edge')
             cx_networks.append(two_edge_net_file)
             with open(two_edge_net_file + constants.CX_SUFFIX, 'w') as f:
                 json.dump(two_edge_net.to_cx(), f)
 
             mockprov = MagicMock()
             mockprov.register_dataset = MagicMock()
             mockprov.register_dataset.side_effect = ['XXX', 'YYY']
             gen = CDAPSHiDeFHierarchyGenerator(provenance_utils=mockprov,
                                                author='author',
                                                version='version')
-            largest_network, net_paths = gen._create_edgelist_files_for_networks(cx_networks)
+            (largest_net_path, largest_network, net_paths) = gen._create_edgelist_files_for_networks(cx_networks)
+            self.assertEqual(two_edge_net_file + '.cx', largest_net_path)
             self.assertEqual('two', largest_network.get_name())
             self.assertEqual(2, len(net_paths))
             self.assertTrue(one_edge_net_file +
                             CDAPSHiDeFHierarchyGenerator.EDGELIST_TSV in net_paths)
             self.assertTrue(two_edge_net_file +
                             CDAPSHiDeFHierarchyGenerator.EDGELIST_TSV in net_paths)
 
@@ -219,12 +221,52 @@
                                                                                CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX +
                                                                                '.nodes'),
                                                       data_dict=data_dict)
             self.assertEqual(3, mockprov.register_dataset.call_count)
         finally:
             shutil.rmtree(temp_dir)
 
+    def test_get_hierarchy_hidef_fails(self):
+        temp_dir = tempfile.mkdtemp()
+        try:
+            cx_networks = []
+            one_edge_net = ndex2.nice_cx_network.NiceCXNetwork()
+            one_edge_net.set_name('one')
+            n_one = one_edge_net.create_node('n1')
+            n_two = one_edge_net.create_node('n2')
+            one_edge_net.create_edge(edge_source=n_one, edge_target=n_two)
+            one_edge_net_file = os.path.join(temp_dir, 'one_edge')
+            cx_networks.append(one_edge_net_file)
+            with open(one_edge_net_file + constants.CX_SUFFIX, 'w') as f:
+                json.dump(one_edge_net.to_cx(), f)
+
+            two_edge_net = ndex2.nice_cx_network.NiceCXNetwork()
+            two_edge_net.set_name('two')
+            n_one = two_edge_net.create_node('n1')
+            n_two = two_edge_net.create_node('n2')
+            n_three = two_edge_net.create_node('n5')
+            two_edge_net.create_edge(edge_source=n_one, edge_target=n_two)
+            two_edge_net.create_edge(edge_source=n_two, edge_target=n_three)
+            two_edge_net_file = os.path.join(temp_dir, 'two_edge')
+            cx_networks.append(two_edge_net_file)
+            with open(two_edge_net_file + constants.CX_SUFFIX, 'w') as f:
+                json.dump(two_edge_net.to_cx(), f)
+
+            mockprov = MagicMock()
+            mockprov.register_dataset = MagicMock(return_val='xxx')
+            gen = CDAPSHiDeFHierarchyGenerator(provenance_utils=mockprov,
+                                               author='author',
+                                               version='version')
+
+            gen.get_hierarchy(cx_networks)
+            self.fail('Expected exception')
+        except CellmapsGenerateHierarchyError as e:
+            self.assertTrue('Cmd failed with exit code: 1' in str(e))
+
+        finally:
+            shutil.rmtree(temp_dir)
+
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/tests/test_cellmaps_generate_hierarchycmd.py` & `cellmaps_generate_hierarchy-0.1.0a6/tests/test_cellmaps_generate_hierarchycmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/tests/test_cellmapsgeneratehierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a6/tests/test_cellmapsgeneratehierarchy.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/tests/test_cosinesimilarityppigenerator.py` & `cellmaps_generate_hierarchy-0.1.0a6/tests/test_cosinesimilarityppigenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a5/tests/test_integration_cellmaps_generate_hierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a6/tests/test_integration_cellmaps_generate_hierarchy.py`

 * *Files identical despite different names*

