# Comparing `tmp/dkist_processing_vbi-1.4.1.tar.gz` & `tmp/dkist_processing_vbi-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_vbi-1.4.1.tar", last modified: Tue Jul 11 22:51:52 2023, max compression
+gzip compressed data, was "dkist_processing_vbi-1.4.2.tar", last modified: Mon Jul 17 21:54:28 2023, max compression
```

## Comparing `dkist_processing_vbi-1.4.1.tar` & `dkist_processing_vbi-1.4.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.926884 dkist_processing_vbi-1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    10437 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6298 2023-07-11 22:51:52.926884 dkist_processing_vbi-1.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5696 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3425 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.918884 dkist_processing_vbi-1.4.1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.918884 dkist_processing_vbi-1.4.1/dkist_processing_vbi/
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.922884 dkist_processing_vbi-1.4.1/dkist_processing_vbi/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/models/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.922884 dkist_processing_vbi-1.4.1/dkist_processing_vbi/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6939 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/parsers/mosaic_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     1144 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.922884 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3008 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4436 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)     6462 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/gain.py
--rw-rw-rw-   0 root         (0) root         (0)    13834 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.922884 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2135 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)     2665 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2185 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/process_summit_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     5607 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5013 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.926884 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9497 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    12936 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/grogu_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2437 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4708 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_gain.py
--rw-rw-rw-   0 root         (0) root         (0)     3704 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10051 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    12628 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_parse_l0.py
--rw-rw-rw-   0 root         (0) root         (0)     5518 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_parse_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     8313 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_process_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6722 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_vbi_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     4746 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.926884 dkist_processing_vbi-1.4.1/dkist_processing_vbi/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2966 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi/workflows/summit_data_processing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.922884 dkist_processing_vbi-1.4.1/dkist_processing_vbi.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6298 2023-07-11 22:51:52.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2574 2023-07-11 22:51:52.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-11 22:51:52.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-07-11 22:51:52.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-11 22:51:52.000000 dkist_processing_vbi-1.4.1/dkist_processing_vbi.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.926884 dkist_processing_vbi-1.4.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/docs/l0_to_l1_vbi_no-speckle.rst
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/docs/l0_to_l1_vbi_summit-calibrated.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:51:52.926884 dkist_processing_vbi-1.4.1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1569 2023-07-11 22:51:52.926884 dkist_processing_vbi-1.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-11 22:51:47.000000 dkist_processing_vbi-1.4.1/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.429391 dkist_processing_vbi-1.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    10686 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6298 2023-07-17 21:54:28.429391 dkist_processing_vbi-1.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5696 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3425 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.425391 dkist_processing_vbi-1.4.2/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.425391 dkist_processing_vbi-1.4.2/dkist_processing_vbi/
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.425391 dkist_processing_vbi-1.4.2/dkist_processing_vbi/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/models/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.425391 dkist_processing_vbi-1.4.2/dkist_processing_vbi/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6939 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/parsers/mosaic_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.429391 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3008 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4436 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    13834 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.429391 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)     2665 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2185 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/process_summit_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     5607 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5013 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.429391 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9497 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    12936 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/grogu_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2437 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4708 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_gain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10051 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    12628 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_parse_l0.py
+-rw-rw-rw-   0 root         (0) root         (0)     5518 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_parse_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     8313 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_process_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6722 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_vbi_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     4746 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.429391 dkist_processing_vbi-1.4.2/dkist_processing_vbi/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2966 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi/workflows/summit_data_processing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.425391 dkist_processing_vbi-1.4.2/dkist_processing_vbi.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6298 2023-07-17 21:54:28.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2574 2023-07-17 21:54:28.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-17 21:54:28.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-07-17 21:54:28.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-17 21:54:28.000000 dkist_processing_vbi-1.4.2/dkist_processing_vbi.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.429391 dkist_processing_vbi-1.4.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/docs/l0_to_l1_vbi_no-speckle.rst
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/docs/l0_to_l1_vbi_summit-calibrated.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:54:28.429391 dkist_processing_vbi-1.4.2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2023-07-17 21:54:28.433391 dkist_processing_vbi-1.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-17 21:54:22.000000 dkist_processing_vbi-1.4.2/towncrier_science.toml
```

### Comparing `dkist_processing_vbi-1.4.1/.gitignore` & `dkist_processing_vbi-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/.pre-commit-config.yaml` & `dkist_processing_vbi-1.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/CHANGELOG.rst` & `dkist_processing_vbi-1.4.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v1.4.2 (2023-07-17)
+===================
+
+Misc
+----
+
+- Update dkist-processing-common and the dkist-header-validator to propagate dependency breakages in PyYAML < 6.0. (`#49 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/49>`__)
+
+
 v1.4.1 (2023-07-11)
 ===================
 
 Misc
 ----
 
 - Update dkist-processing-common to upgrade Airflow to 2.6.3.
```

### Comparing `dkist_processing_vbi-1.4.1/PKG-INFO` & `dkist_processing_vbi-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_vbi
-Version: 1.4.1
+Version: 1.4.2
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_vbi-1.4.1/README.rst` & `dkist_processing_vbi-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/bitbucket-pipelines.yml` & `dkist_processing_vbi-1.4.2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/check_changelog_updated.sh` & `dkist_processing_vbi-1.4.2/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/models/constants.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/models/filter.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/models/filter.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/models/tags.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/parsers/mosaic_repeats.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/parsers/mosaic_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/parsers/vbi_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/parsers/vbi_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/assemble_movie.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/dark.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/gain.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/make_movie_frames.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/parse.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/process_summit_processed.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/process_summit_processed.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/quality_metrics.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/science.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/vbi_base.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tasks/write_l1.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/conftest.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/grogu_test.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/grogu_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_assemble_movie.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_dark.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_gain.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_intermediate_loaders.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_make_movie_frames.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_parse_l0.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_parse_l0.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_parse_summit.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_parse_summit.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_process_summit.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_process_summit.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_quality_metrics.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_science.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_vbi_base.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_vbi_constants.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_vbi_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/tests/test_write_l1.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/workflows/l0_processing.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi/workflows/summit_data_processing.py` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi/workflows/summit_data_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi.egg-info/PKG-INFO` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-vbi
-Version: 1.4.1
+Version: 1.4.2
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi.egg-info/SOURCES.txt` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/dkist_processing_vbi.egg-info/requires.txt` & `dkist_processing_vbi-1.4.2/dkist_processing_vbi.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-dkist-processing-common==4.0.1
+dkist-processing-common==4.0.2
 dkist-processing-math==2.0.0
-dkist-header-validator==3.0.5
+dkist-header-validator==4.0.0
 dkist-fits-specifications==3.6.0
 astropy==5.3.0
 numpy==1.24.3
 sunpy==5.0.0
 scipy==1.11.0
 pillow==9.5.0
 moviepy==1.0.3
```

### Comparing `dkist_processing_vbi-1.4.1/docs/Makefile` & `dkist_processing_vbi-1.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/docs/conf.py` & `dkist_processing_vbi-1.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/docs/l0_to_l1_vbi_no-speckle.rst` & `dkist_processing_vbi-1.4.2/docs/l0_to_l1_vbi_no-speckle.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/docs/l0_to_l1_vbi_summit-calibrated.rst` & `dkist_processing_vbi-1.4.2/docs/l0_to_l1_vbi_summit-calibrated.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/docs/make.bat` & `dkist_processing_vbi-1.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/licenses/LICENSE.rst` & `dkist_processing_vbi-1.4.2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/pyproject.toml` & `dkist_processing_vbi-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.4.1/setup.cfg` & `dkist_processing_vbi-1.4.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 4.0.1
+	dkist-processing-common == 4.0.2
 	dkist-processing-math == 2.0.0
-	dkist-header-validator == 3.0.5
+	dkist-header-validator == 4.0.0
 	dkist-fits-specifications == 3.6.0
 	astropy == 5.3.0
 	numpy == 1.24.3
 	sunpy == 5.0.0
 	scipy == 1.11.0
 	pillow == 9.5.0
 	moviepy == 1.0.3
```

