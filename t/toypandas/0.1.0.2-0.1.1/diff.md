# Comparing `tmp/toypandas-0.1.0.2.tar.gz` & `tmp/toypandas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toypandas-0.1.0.2.tar", last modified: Fri Jul 14 13:08:21 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `toypandas-0.1.0.2.tar` & `toypandas-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,52 @@
-drwxr-xr-x   0 danieletraversaro   (501) staff       (20)        0 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/
--rw-r--r--   0 danieletraversaro   (501) staff       (20)      285 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/PKG-INFO
-drwxr-xr-x   0 danieletraversaro   (501) staff       (20)        0 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas/
--rw-r--r--   0 danieletraversaro   (501) staff       (20)     9725 2023-07-14 12:05:35.000000 toypandas-0.1.0.2/ToyPandas/toypandas.py
-drwxr-xr-x   0 danieletraversaro   (501) staff       (20)        0 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/
--rw-r--r--   0 danieletraversaro   (501) staff       (20)      285 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/PKG-INFO
--rw-r--r--   0 danieletraversaro   (501) staff       (20)      382 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/SOURCES.txt
--rw-r--r--   0 danieletraversaro   (501) staff       (20)       37 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/requires.txt
--rw-r--r--   0 danieletraversaro   (501) staff       (20)       10 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/top_level.txt
--rw-r--r--   0 danieletraversaro   (501) staff       (20)        1 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/dependency_links.txt
--rw-r--r--   0 danieletraversaro   (501) staff       (20)      364 2023-07-14 13:08:04.000000 toypandas-0.1.0.2/setup.py
--rw-r--r--   0 danieletraversaro   (501) staff       (20)       59 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/setup.cfg
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 toypandas-0.1.1/Makefile
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 toypandas-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0  2504919 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/autoapi/index.doctree
+-rw-r--r--   0        0        0    18039 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/autoapi/toypandas/index.doctree
+-rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/autoapi/toypandas/dataframe/index.doctree
+-rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/autoapi/toypandas/locating/index.doctree
+-rw-r--r--   0        0        0    36717 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/autoapi/toypandas/series/index.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/index.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/py-modindex.html
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/search.html
+-rw-r--r--   0        0        0     8556 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/autoapi/index.rst.txt
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/autoapi/toypandas/index.rst.txt
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/autoapi/toypandas/dataframe/index.rst.txt
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/autoapi/toypandas/locating/index.rst.txt
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/autoapi/toypandas/series/index.rst.txt
+-rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/graphviz.css
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/autoapi/index.html
+-rw-r--r--   0        0        0    10118 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/autoapi/toypandas/index.html
+-rw-r--r--   0        0        0    17261 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/autoapi/toypandas/dataframe/index.html
+-rw-r--r--   0        0        0     6486 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/autoapi/toypandas/locating/index.html
+-rw-r--r--   0        0        0    16913 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/autoapi/toypandas/series/index.html
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 toypandas-0.1.1/src/toypandas/__init__.py
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 toypandas-0.1.1/src/toypandas/dataframe.py
+-rw-r--r--   0        0        0     5767 2020-02-02 00:00:00.000000 toypandas-0.1.1/src/toypandas/series.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toypandas-0.1.1/LICENSE
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 toypandas-0.1.1/README.md
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 toypandas-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 toypandas-0.1.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

