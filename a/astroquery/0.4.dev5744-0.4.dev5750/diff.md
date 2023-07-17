# Comparing `tmp/astroquery-0.4.dev5744.tar.gz` & `tmp/astroquery-0.4.dev5750.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/astroquery-0.4.dev5744.tar", last modified: Tue Oct  8 20:45:32 2019, max compression
+gzip compressed data, was "dist/astroquery-0.4.dev5750.tar", last modified: Thu Oct 10 04:47:58 2019, max compression
```

## Comparing `astroquery-0.4.dev5744.tar` & `astroquery-0.4.dev5750.tar`

### file list

```diff
@@ -1,1087 +1,1091 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19118 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/CHANGES.rst
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/CITATION -> astroquery/CITATION
--rw-rw-r--   0 travis    (2000) travis    (2000)     1497 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/LICENSE.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      421 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    11377 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    37494 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/ah_bootstrap.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18166 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1491 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/LICENSE.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2587 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    37494 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/ah_bootstrap.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1836 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2940 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/_dummy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11722 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/_test_compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19785 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/build_ext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1454 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/build_py.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10935 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/build_sphinx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      486 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/install.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      512 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/install_lib.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/register.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3033 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/src/compiler.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1364 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/compat/
--rw-rw-r--   0 travis    (2000) travis    (2000)      368 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/compat/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1647 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7922 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/distutils_helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/
--rw-rw-r--   0 travis    (2000) travis    (2000)      589 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5398 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/autodoc_enhancements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16490 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/automodapi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27764 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/automodsumm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4148 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/smart_resolver.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7140 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/numpydoc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      194 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/numpydoc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19206 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15160 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape_sphinx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11395 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/numpydoc/numpydoc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6465 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/git_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3145 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/openmp_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27888 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/setup_helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/
--rw-rw-r--   0 travis    (2000) travis    (2000)      437 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11873 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/conf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3193 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5940 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/local/
--rw-rw-r--   0 travis    (2000) travis    (2000)      562 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1638 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      658 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv
--rw-rw-r--   0 travis    (2000) travis    (2000)     2820 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/globaltoc.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3433 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/localtoc.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/searchbox.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5201 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1725 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    32988 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1884 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    12067 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css
--rw-rw-r--   0 travis    (2000) travis    (2000)     2769 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     4971 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      192 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/theme.conf
--rw-rw-r--   0 travis    (2000) travis    (2000)      515 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27125 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      569 2019-10-08 20:45:12.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10035 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/version_helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3946 2019-10-08 20:45:12.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3278 2019-10-08 20:45:12.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-08 20:45:12.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-08 20:45:12.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-10-08 20:45:12.000000 astroquery-0.4.dev5744/astropy_helpers/astropy_helpers.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astropy_helpers/licenses/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1644 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2505 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5959 2019-10-08 20:41:37.000000 astroquery-0.4.dev5744/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1330 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/CITATION
--rw-rw-r--   0 travis    (2000) travis    (2000)      992 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2023 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/_astropy_init.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/alfalfa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      494 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alfalfa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6620 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alfalfa/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/alfalfa/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alfalfa/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/alfalfa/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4226 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alfalfa/tests/data/alfalfa_cat_small.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    83520 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alfalfa/tests/data/alfalfa_sp.fits
--rw-rw-r--   0 travis    (2000) travis    (2000)      291 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alfalfa/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2442 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alfalfa/tests/test_alfalfa.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/alma/
--rw-rw-r--   0 travis    (2000) travis    (2000)      863 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47339 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/alma/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    36513 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/data/cycle0_delivery_asdm_mapping.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      264 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/alma/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11891 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/data_list_page.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      418 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/downloadRequest519752156script.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      376 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/downloadRequest786572566script.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)     4306 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/downloadRequest786978956script.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)     2686 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/downloadRequest787632764script.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/empty.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    39698 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/etacar_query.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2759 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/initial_response.html
--rw-rw-r--   0 travis    (2000) travis    (2000)  2319422 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/m83_March25_2015.votable.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    42792 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/ngc4945.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    42990 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/querypage.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    13491 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/request_786572566.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    53200 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/request_786978956.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    69518 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/request_787632764.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    15293 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/request_801926122.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    11891 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/staging_submission.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/data/summary_519752156.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      376 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7972 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/test_alma.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13316 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/test_alma_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3583 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/tests/test_alma_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22712 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/alma/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/
--rw-rw-r--   0 travis    (2000) travis    (2000)      853 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17909 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    37440 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/test-source-list.fit
--rw-rw-r--   0 travis    (2000) travis    (2000)    17280 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/test-wcs-sol.fit
--rw-rw-r--   0 travis    (2000) travis    (2000)    42485 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/thumbnail-image.fit.gz
--rw-rw-r--   0 travis    (2000) travis    (2000)    11520 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/thumbnail-wcs-sol-from-photutils.fit
--rw-rw-r--   0 travis    (2000) travis    (2000)    17280 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/thumbnail-wcs-sol.fit
--rw-rw-r--   0 travis    (2000) travis    (2000)      374 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6898 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/test_astrometry_net.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astrometry_net/tests/test_astrometry_net_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5605 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/astroquery.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/atomic/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2603 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/atomic/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15742 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/atomic/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      154 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/atomic/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/atomic/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/atomic/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/atomic/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45949 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/atomic/tests/data/default_params_result.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/atomic/tests/data/empty_results.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2951 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/atomic/tests/test_atomic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3302 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/atomic/tests/test_atomic_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      482 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/atomic/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/besancon/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1300 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15502 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7428 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/data/1376235131.430670.resu
--rw-rw-r--   0 travis    (2000) travis    (2000)     7428 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/data/besancon_test.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8106 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/data/besancon_test2.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2465 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/data/default_params.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      466 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/data/query_return.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     6787 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/data/query_return.iframe.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      337 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3872 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/besancon/tests/test_besancon.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/cadc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      935 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29901 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      645 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/DummyJob.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4486 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/DummyTapHandler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3821 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/data/datalink_result.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/data/job_1.vot
--rw-rw-r--   0 travis    (2000) travis    (2000)    51840 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/data/query_images.fits
--rw-rw-r--   0 travis    (2000) travis    (2000)     4591 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/data/tap_caps.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      598 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15988 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/test_cadctap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10981 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cadc/tests/test_cadctap_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/cds/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1365 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18113 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cds/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/cds/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cds/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/cds/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cds/tests/data/hips_from_saada_alasky.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      223 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cds/tests/data/properties.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      135 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cds/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5153 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cds/tests/test_mocserver.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3171 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cds/tests/test_mocserver_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3052 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/conftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/cosmosim/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cosmosim/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58419 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cosmosim/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/cosmosim/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cosmosim/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/cosmosim/tests/test_cosmosim.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/esa/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/
--rw-rw-r--   0 travis    (2000) travis    (2000)      951 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15358 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      226 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/data/F05I0602M.tar
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/data/J6FL25S4Q.tar
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/data/X0MC5101T.tar
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/data/metadata.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/data/region.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/data/target.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2712 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/dummy_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3469 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/dummy_tap_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      515 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5331 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esa/hubble/tests/test_esa_hubble.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/esasky/
--rw-rw-r--   0 travis    (2000) travis    (2000)      680 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esasky/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37868 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esasky/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/esasky/tests/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esasky/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/esasky/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    28700 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esasky/tests/data/catalogs.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    16100 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esasky/tests/data/observations.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      555 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esasky/tests/setup_package.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1722 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esasky/tests/test_esasky.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3960 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/esasky/tests/test_esasky_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/eso/
--rw-rw-r--   0 travis    (2000) travis    (2000)      721 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45553 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/eso/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    39108 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/47cae7cb7578c2a4f0461b4897e6a05a747d3b79aad09a25168c0463.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)    29615 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/862b6db5bf174fb89ee7ddc42d0fcd49d864388bc3c0dc6f6f64744b.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/a77820a9fdbaa8ca10322e0832595e3ce59b9b28241ade00bd846ce6.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)    35621 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/amber_query_form.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    10143 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/amber_sgra_query.tbl
--rw-rw-r--   0 travis    (2000) travis    (2000)    26370 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/c3931c90b484ef51fb10ad6370d9e5af99de668e116460c36fe1d1c5.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)    27132 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/da4b7c06e277275f197d8681bf5fdc0ecd556ed07e6aac8cbf0249d2.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)    25415 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/de77b0a24235373d6bbf8487ba825fcd634768f43da682614d202ffc.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)    29128 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/e2c39d36193cdb16ce871845157c1e50ff539cf8122d87a8282854b9.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)      383 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/efafb320926e82995df2dc4e2ea745de75c51ea90b7ed52bc6569105.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)    25361 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/main_query_form.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/main_sgra_query.tbl
--rw-rw-r--   0 travis    (2000) travis    (2000)    50742 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/vvv_sgra_form.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    14321 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/data/vvv_sgra_survey_response.tbl
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3190 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/test_eso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8017 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/eso/tests/test_eso_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2207 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/
--rw-rw-r--   0 travis    (2000) travis    (2000)      688 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3770 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/data/exoplanet_orbit_database_units.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4114 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/exoplanet_orbit_database.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      313 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      133 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6355 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/tests/data/exoplanet_orbit_database.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     4841 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/tests/test_exoplanet_orbit_database.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/fermi/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1022 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/fermi/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5291 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/fermi/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      245 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/fermi/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/fermi/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/fermi/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/fermi/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6705 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/fermi/tests/data/query_result_m31.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     8490 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/fermi/tests/data/result_page_m31.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2503 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/fermi/tests/test_fermi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/fermi/tests/test_fermi_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/gaia/
--rw-rw-r--   0 travis    (2000) travis    (2000)      968 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gaia/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23093 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gaia/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/gaia/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13160 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gaia/tests/DummyTapHandler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      284 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gaia/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/gaia/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gaia/tests/data/job_1.vot
--rw-rw-r--   0 travis    (2000) travis    (2000)      509 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gaia/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24624 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gaia/tests/test_gaiatap.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/gama/
--rw-rw-r--   0 travis    (2000) travis    (2000)      287 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gama/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2284 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gama/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/gama/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gama/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/gama/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11520 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gama/tests/data/GAMA_HzVs28.fits
--rw-rw-r--   0 travis    (2000) travis    (2000)    48879 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gama/tests/data/query_result.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gama/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1008 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gama/tests/test_gama.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      662 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/gama/tests/test_gama_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/heasarc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1255 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/heasarc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13184 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/heasarc/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/heasarc/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/heasarc/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      290 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/heasarc/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/heasarc/tests/test_heasarc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2167 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/heasarc/tests/test_heasarc_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/hitran/
--rw-rw-r--   0 travis    (2000) travis    (2000)      867 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/hitran/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11868 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/hitran/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/hitran/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5303 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/hitran/data/readme.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      357 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/hitran/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/hitran/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/hitran/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/hitran/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19764 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/hitran/tests/data/H2O.data
--rw-rw-r--   0 travis    (2000) travis    (2000)     1949 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/hitran/tests/test_hitran.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/hitran/tests/test_hitran_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4716 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/hitran/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ibe/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1271 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16715 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    34515 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/data/columns.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      844 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/data/datasets.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    50778 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/data/field_id.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      907 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/data/missions.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    50600 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/data/pos.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1308 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/data/tables.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      287 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3077 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/test_ibe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      794 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ibe/tests/test_ibe_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/imcce/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2555 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30225 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5238 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype1.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)     7294 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype2.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)     4806 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype3.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)     4807 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype4.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)     7453 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype5.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)     6244 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype6.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)    35514 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/data/skybot_query.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)      259 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4550 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/test_miriade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      703 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/test_miriade_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4565 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/test_skybot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1176 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/imcce/tests/test_skybot_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/irsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      994 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21068 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/irsa/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/irsa/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4171 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa/tests/data/Box.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     4308 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa/tests/data/Cone.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     4307 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa/tests/data/Cone_coord.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     7775 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa/tests/data/Polygon.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6208 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa/tests/test_irsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2074 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa/tests/test_irsa_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/
--rw-rw-r--   0 travis    (2000) travis    (2000)      961 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40935 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/dust-error.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     4377 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/dust_ext_detail.tbl
--rw-rw-r--   0 travis    (2000) travis    (2000)     2573 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/dustm101.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/dustm31.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2569 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/dustm81.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)   331200 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/test.fits
--rw-rw-r--   0 travis    (2000) travis    (2000)      381 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15511 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/test_irsa_dust.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7285 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/tests/test_irsa_dust_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2980 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/irsa_dust/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9018 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65635 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7361 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/tests/data/ceres_elements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    15088 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/tests/data/ceres_ephemerides.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6823 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/tests/data/ceres_vectors.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    28929 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/tests/data/no_H.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8416 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/tests/test_jplhorizons.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15091 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplhorizons/tests/test_jplhorizons_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1607 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16553 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20313 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/67P.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)    53829 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/apophis.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)     7044 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/ceres.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)     7029 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/ceres_missing_value.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)    38098 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/phaethon.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)      315 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3496 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/test_jplsbdb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplsbdb/tests/test_jplsbdb_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/jplspec/
--rw-rw-r--   0 travis    (2000) travis    (2000)      727 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10228 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/jplspec/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    31527 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/data/catdir.cat
--rw-rw-r--   0 travis    (2000) travis    (2000)      932 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/lookup_table.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      454 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/jplspec/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/jplspec/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      681 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/tests/data/CO.data
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/tests/data/CO_6.data
--rw-rw-r--   0 travis    (2000) travis    (2000)    17016 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/tests/data/multi.data
--rw-rw-r--   0 travis    (2000) travis    (2000)     3939 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/tests/test_jplspec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/jplspec/tests/test_jplspec_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/lamda/
--rw-rw-r--   0 travis    (2000) travis    (2000)      701 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lamda/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14121 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lamda/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/lamda/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lamda/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/lamda/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    25560 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lamda/tests/data/co.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      244 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lamda/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lamda/tests/test_lamda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      466 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lamda/tests/test_lamda_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4951 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lamda/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/lcogt/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1098 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lcogt/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17299 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lcogt/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/lcogt/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lcogt/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/lcogt/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4171 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lcogt/tests/data/Box.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     4308 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lcogt/tests/data/Cone.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     4307 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lcogt/tests/data/Cone_coord.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     7775 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lcogt/tests/data/Polygon.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      244 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lcogt/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6349 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lcogt/tests/test_lcogt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2683 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/lcogt/tests/test_lcogt_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/magpis/
--rw-rw-r--   0 travis    (2000) travis    (2000)      838 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/magpis/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4910 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/magpis/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/magpis/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/magpis/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/magpis/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)   365760 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/magpis/tests/data/image.fits
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/magpis/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2343 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/magpis/tests/test_magpis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      822 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/magpis/tests/test_magpis_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/mast/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1249 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    93700 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6730 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/fpl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13515 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tesscut.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/mast/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3904 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/advSearch.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    12466 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/advSearchPos.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   260927 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/astrocut_107.27_-70.0_5x5.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)      537 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/bundleResponse.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    18958 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/caom.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    12347 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/columnsconfig.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      221 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/countsResp.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    15794 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/dd.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1936 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/ddcolumns.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   674902 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/ddcolumns_filtered.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    35770 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/hsc.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    11755 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/matchid.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   225915 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/missions.extjs
--rw-rw-r--   0 travis    (2000) travis    (2000)     8185 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/panstarrs.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    12359 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/products.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/resolver.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    13369 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/spectra.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       86 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/tess_sector.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    15817 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/tic.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6807 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/ticcolumns.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   423717 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/data/ticcolumns_filtered.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      236 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22004 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/test_mast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26157 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mast/tests/test_mast_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/mpc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56316 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      324 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9296 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/1994XG_ephemeris_500-a-t.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    10133 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/1994XG_ephemeris_G37-a-t.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2556 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_500-G-t.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3076 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_500-a-c.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3075 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_500-a-s.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3075 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_500-a-t.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3615 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_500-s-t.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3903 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_G37-a-t.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      702 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/ObsCodes.html
--rw-rw-r--   0 travis    (2000) travis    (2000)   337798 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/mpc_obs.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/data/testfail_ephemeris_500-a-t.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    16944 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/test_mpc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4707 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/mpc/tests/test_mpc_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nasa_ads/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1030 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_ads/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4066 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_ads/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nasa_ads/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_ads/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nasa_ads/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      744 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_ads/tests/data/test_text.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_ads/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_ads/tests/test_nasaads.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      388 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_ads/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/
--rw-rw-r--   0 travis    (2000) travis    (2000)      670 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1599 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/data/exoplanet_nexsci_units.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4988 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/nasa_exoplanet_archive.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      311 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/tests/data/nasa_exoplanet_archive.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     5038 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/tests/test_nasa_exoplanet_archive_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ned/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2566 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28522 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ned/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    44661 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/data/keywords_dict.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ned/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      862 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/error.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     7550 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/image_extract.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    13031 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_diameters.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    11033 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_iau_format.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    72000 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_images.fits
--rw-rw-r--   0 travis    (2000) travis    (2000)     6577 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_near_name.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)   126513 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_near_position.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    40517 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_notes.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     5183 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_object.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)   277494 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_photometry.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     8352 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_positions.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     8704 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_redshifts.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    14494 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_refcode.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     7509 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/data/query_references.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     9913 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/test_ned.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3307 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ned/tests/test_ned_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nist/
--rw-rw-r--   0 travis    (2000) travis    (2000)      634 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nist/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7775 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nist/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nist/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nist/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nist/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24444 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nist/tests/data/nist_out.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nist/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1740 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nist/tests/test_nist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1173 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nist/tests/test_nist_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nrao/
--rw-rw-r--   0 travis    (2000) travis    (2000)      742 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nrao/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19954 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nrao/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nrao/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nrao/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nrao/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)   263122 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nrao/tests/data/archive_html.html
--rw-rw-r--   0 travis    (2000) travis    (2000)   793497 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nrao/tests/data/votable.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nrao/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4278 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nrao/tests/test_nrao.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2189 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nrao/tests/test_nrao_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nvas/
--rw-rw-r--   0 travis    (2000) travis    (2000)      777 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nvas/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9887 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nvas/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nvas/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nvas/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/nvas/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    66240 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nvas/tests/data/image.imfits
--rw-rw-r--   0 travis    (2000) travis    (2000)    16956 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nvas/tests/data/image_results.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nvas/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4404 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nvas/tests/test_nvas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      918 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/nvas/tests/test_nvas_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/oac/
--rw-rw-r--   0 travis    (2000) travis    (2000)      934 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/oac/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19861 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/oac/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/oac/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/oac/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/oac/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    34404 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/oac/tests/data/photometry_csv.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    41357 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/oac/tests/data/photometry_json.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    46287 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/oac/tests/data/single_spectrum_csv.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   157121 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/oac/tests/data/spectra_json.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      290 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/oac/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3191 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/oac/tests/test_oac.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2890 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/oac/tests/test_oac_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ogle/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1061 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ogle/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7627 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ogle/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ogle/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ogle/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ogle/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      197 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ogle/tests/data/gal_0_3.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ogle/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1716 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ogle/tests/test_ogle.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/
--rw-rw-r--   0 travis    (2000) travis    (2000)      280 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2374 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/oec_query.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)   244625 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/tests/data/systems.xml.gz
--rw-rw-r--   0 travis    (2000) travis    (2000)      383 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      735 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/tests/test_open_exoplanet_catalogue_local.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      489 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/tests/test_open_exoplanet_catalogue_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9006 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16704 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/query.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/sdss/
--rw-rw-r--   0 travis    (2000) travis    (2000)      854 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46643 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/sdss/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)   115564 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/data/PhotoObjAll_dr12.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    46061 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/data/SpecObjAll_dr12.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3201 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/field_names.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/sdss/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/sdss/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2880 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/tests/data/emptyfile.fits
--rw-rw-r--   0 travis    (2000) travis    (2000)     1163 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/tests/data/xid_im.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      206 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/tests/data/xid_sp.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13504 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/tests/test_sdss.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6746 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sdss/tests/test_sdss_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      187 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/sha/
--rw-rw-r--   0 travis    (2000) travis    (2000)      446 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sha/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8261 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sha/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/sha/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sha/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/sha/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    95040 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sha/tests/data/img.fits
--rw-rw-r--   0 travis    (2000) travis    (2000)     3377 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sha/tests/data/nid_t.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   374026 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sha/tests/data/pid_t.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    20311 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sha/tests/data/pos_t.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5276 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sha/tests/data/rqk_t.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sha/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2202 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/sha/tests/test_sha.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/simbad/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1101 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40364 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/simbad/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7947 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/data/votable_fields_dict.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      503 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/data/votable_fields_notes.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1602 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/get_votable_fields.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      960 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3165 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/m1.data
--rw-rw-r--   0 travis    (2000) travis    (2000)      838 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_bibcode.data
--rw-rw-r--   0 travis    (2000) travis    (2000)     3843 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_bibobj.data
--rw-rw-r--   0 travis    (2000) travis    (2000)    20797 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_cat.data
--rw-rw-r--   0 travis    (2000) travis    (2000)    14181 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_coo.data
--rw-rw-r--   0 travis    (2000) travis    (2000)     1130 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_error.data
--rw-rw-r--   0 travis    (2000) travis    (2000)     3165 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_id.data
--rw-rw-r--   0 travis    (2000) travis    (2000)      932 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_objectids.data
--rw-rw-r--   0 travis    (2000) travis    (2000)     1977 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_sample.data
--rw-rw-r--   0 travis    (2000) travis    (2000)     4548 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_sample_region.data
--rw-rw-r--   0 travis    (2000) travis    (2000)    17911 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/test_simbad.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8057 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/simbad/tests/test_simbad_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/skyview/
--rw-rw-r--   0 travis    (2000) travis    (2000)      466 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/skyview/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14126 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/skyview/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      336 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/skyview/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/skyview/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/skyview/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/skyview/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)   122244 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/skyview/tests/data/query_page.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    32703 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/skyview/tests/data/results.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3616 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/skyview/tests/data/survey_dict.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2963 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/skyview/tests/test_skyview.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1722 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/skyview/tests/test_skyview_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/solarsystem/
--rw-rw-r--   0 travis    (2000) travis    (2000)      247 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/solarsystem/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/solarsystem/imcce/
--rw-rw-r--   0 travis    (2000) travis    (2000)      242 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/solarsystem/imcce/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/solarsystem/imcce/miriade/
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/solarsystem/imcce/miriade/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/solarsystem/imcce/skybot/
--rw-rw-r--   0 travis    (2000) travis    (2000)      236 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/solarsystem/imcce/skybot/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/solarsystem/jpl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      235 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/solarsystem/jpl/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/solarsystem/jpl/horizons/
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/solarsystem/jpl/horizons/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/solarsystem/jpl/sbdb/
--rw-rw-r--   0 travis    (2000) travis    (2000)      226 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/solarsystem/jpl/sbdb/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/solarsystem/mpc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/solarsystem/mpc/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/splatalogue/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1106 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1286 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/build_species_table.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21208 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/splatalogue/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    56822 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/data/species.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/load_species_table.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      409 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1827 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/slap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      439 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/splatalogue/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/splatalogue/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1037 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/tests/data/CO_colons.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     6119 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/tests/test_splatalogue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/splatalogue/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/template_module/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1078 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/template_module/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13780 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/template_module/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/template_module/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/template_module/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/template_module/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/template_module/tests/data/dummy.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)      520 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/template_module/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3115 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/template_module/tests/test_module.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      488 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/template_module/tests/test_module_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      768 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/tests/coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)      201 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      424 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/tests/test_internet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1284 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/tests/test_resume.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ukidss/
--rw-rw-r--   0 travis    (2000) travis    (2000)      925 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2529 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2303 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/data/error.html
--rw-rw-r--   0 travis    (2000) travis    (2000)   385920 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/data/image.fits
--rw-rw-r--   0 travis    (2000) travis    (2000)     1098 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/data/image_results.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    13757 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/data/vo_results.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4985 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/data/votable.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      336 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5745 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/test_ukidss.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2270 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/ukidss/tests/test_ukidss_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1018 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/class_or_instance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15084 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/commons.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8399 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1271 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/docstr_chompers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4217 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/download_file_list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2623 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/process_asyncs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1945 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/progressbar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6260 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/schema.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2271 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/system_tools.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      547 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/conn/
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/conn/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    25239 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/conn/tapconn.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1624 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/DummyConn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5329 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/DummyConnHandler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1862 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/DummyResponse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      424 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6649 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/test_conn.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    81617 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/gui/
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/gui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3911 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/gui/login.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1489 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/filter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      915 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/group.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    17476 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/job.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/modelutils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      952 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/shared_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      752 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/shared_to_item.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1091 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/tapcolumn.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1274 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/taptable.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/tests/data/result_1.vot
--rw-rw-r--   0 travis    (2000) travis    (2000)      468 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3911 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/tests/test_job.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      612 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/model/user.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5824 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/taputils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/tests/data/job_1.vot
--rw-rw-r--   0 travis    (2000) travis    (2000)      573 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/tests/data/jobs_list.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1123 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/tests/data/test_table1.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1931 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/tests/data/test_tables.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      729 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35694 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/tests/test_tap.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3732 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/groupSaxParser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2823 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/jobListSaxParser.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4431 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/jobSaxParser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3840 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/sharedItemsSaxParser.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6292 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tableSaxParser.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10867 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/data/test_job_results.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1790 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/data/test_jobs_async.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      646 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/data/test_jobs_list.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1931 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/data/test_tables.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      516 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3758 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/test_xmlparser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1724 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/testing_tools.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/utils/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      384 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tests/test_url_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14141 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1603 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/utils/url_helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vamdc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      575 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vamdc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3802 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vamdc/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1601 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vamdc/load_species_table.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vamdc/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vamdc/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      510 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vamdc/tests/setup_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      588 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vamdc/tests/test_vamdc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      763 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vamdc/tests/test_vamdc_remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7358 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vizier/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1488 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33047 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vizier/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3364 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/data/inverse_dict.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2171 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/data/keywords_dict.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      628 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vizier/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vizier/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8019 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/tests/data/afgl2591_iram.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     9834 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/tests/data/find_kangapj70683.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    20706 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/tests/data/kang2010.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)   443070 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/tests/data/viz.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/tests/test_vizier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5449 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vizier/tests/test_vizier_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1242 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16847 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/conesearch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7804 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1133 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      207 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/data/basic.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      251 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/data/conesearch_error1.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      300 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/data/conesearch_error2.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      339 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/data/conesearch_error3.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      310 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/data/conesearch_error4.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     9009 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/test_conesearch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7031 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/test_vos_catalog.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1486 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/data/conesearch_urls.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      710 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/inspect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      408 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/conesearch_error.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/conesearch_exception.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3344 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/conesearch_good.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/conesearch_warn.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      355 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/listcats1.out
--rw-rw-r--   0 travis    (2000) travis    (2000)       97 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/listcats2.out
--rw-rw-r--   0 travis    (2000) travis    (2000)     2875 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/printcat.out
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/tally.out
--rw-rw-r--   0 travis    (2000) travis    (2000)     3844 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/vao_conesearch_sites_121107_subset.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2641 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/test_inpect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3114 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/test_validate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2961 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tstquery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11356 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/validate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2609 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/vo_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28184 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vo_conesearch/vos_catalog.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      928 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2909 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vsa/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/vsa/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vsa/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2871 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/vsa/tests/test_vista_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/wfau/
--rw-rw-r--   0 travis    (2000) travis    (2000)      597 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/wfau/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37041 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/wfau/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/xmatch/
--rw-rw-r--   0 travis    (2000) travis    (2000)      558 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/xmatch/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7891 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/xmatch/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      245 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/xmatch/setup_package.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/xmatch/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/xmatch/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/astroquery/xmatch/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      140 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/xmatch/tests/data/posList.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      301 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/xmatch/tests/data/poslist_duplicates.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1688 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/xmatch/tests/data/query_res.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   275304 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/xmatch/tests/data/tables.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     4295 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/xmatch/tests/test_xmatch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4439 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/astroquery/xmatch/tests/test_xmatch_remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4581 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/_templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/_templates/autosummary/
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/_templates/autosummary/base.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      251 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      252 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/_templates/autosummary/module.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/alfalfa/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1550 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/alfalfa/alfalfa.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/alma/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7629 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/alma/alma.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     8783 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/api.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/astrometry_net/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12990 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/astrometry_net/astrometry_net.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/atomic/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2171 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/atomic/atomic.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/besancon/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5752 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/besancon/besancon.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/cadc/
--rw-rw-r--   0 travis    (2000) travis    (2000)    25091 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/cadc/cadc.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/cds/
--rw-rw-r--   0 travis    (2000) travis    (2000)   140621 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/cds/HST_union.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   131787 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/cds/MOC_GALEXGR6_AIS_FUV.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    44330 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/cds/cds.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     7588 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/conf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/cosmosim/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19150 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/cosmosim/cosmosim.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/demos/
--rw-rw-r--   0 travis    (2000) travis    (2000)   518906 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/demos/Astroquery_DotAstro_Demo.ipynb
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/esa/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4679 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/esa/hubble.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/esasky/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9965 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/esasky/esasky.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/eso/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16639 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/eso/eso.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/exoplanet_orbit_database/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2290 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/exoplanet_orbit_database/exoplanet_orbit_database.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/fermi/
--rw-rw-r--   0 travis    (2000) travis    (2000)      995 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/fermi/fermi.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/gaia/
--rw-rw-r--   0 travis    (2000) travis    (2000)    27623 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gaia/gaia.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/gallery-examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1538 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/example10_mast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      930 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/example1_vizier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      717 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/example2_simbad.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      216 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/example3_simbad.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      738 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/example4_simbad.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      252 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/example5_oec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/example6_alma.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10578 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/example7_alma.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      793 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/example8_eso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1965 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/example9_skyview_vizier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      380 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery-examples/run_examples.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2464 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gallery.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/gama/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3986 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/gama/gama.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/heasarc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8906 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/heasarc/heasarc.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/hitran/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1349 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/hitran/hitran.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/ibe/
--rw-rw-r--   0 travis    (2000) travis    (2000)      993 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/ibe/ibe.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/imcce/
--rw-rw-r--   0 travis    (2000) travis    (2000)    26921 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/imcce/imcce.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     9593 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/index.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/irsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12157 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/irsa/irsa.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     9213 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/irsa/irsa_dust.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/jplhorizons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24374 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/jplhorizons/jplhorizons.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/jplsbdb/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11843 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/jplsbdb/jplsbdb.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/jplspec/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/jplspec/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)    37257 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/jplspec/images/docplot_curvefit.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    25216 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/jplspec/images/docplot_jplspec.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    11376 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/jplspec/jplspec.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/lamda/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1456 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/lamda/lamda.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/license.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/magpis/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2502 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/magpis/magpis.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4513 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)     1222 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/make_doctests.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:31.000000 astroquery-0.4.dev5744/docs/mast/
--rw-rw-r--   0 travis    (2000) travis    (2000)    55480 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/mast/mast.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/mpc/
--rw-rw-r--   0 travis    (2000) travis    (2000)    26623 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/mpc/mpc.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/nasa_ads/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2068 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/nasa_ads/nasa_ads.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/nasa_exoplanet_archive/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2324 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/nasa_exoplanet_archive/nasa_exoplanet_archive.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/ned/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13635 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/ned/ned.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/nist/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7683 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/nist/nist.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/nrao/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4405 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/nrao/nrao.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/nvas/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4683 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/nvas/nvas.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/oac/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5805 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/oac/oac.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/ogle/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1600 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/ogle/ogle.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/open_exoplanet_catalogue/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4548 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/open_exoplanet_catalogue/open_exoplanet_catalogue.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/query.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1912 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/release_notice_v0.2.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/sdss/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2792 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/sdss/sdss.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/sha/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2410 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/sha/sha.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/simbad/
--rw-rw-r--   0 travis    (2000) travis    (2000)    33218 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/simbad/simbad.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/skyview/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9614 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/skyview/skyview.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/solarsystem/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/solarsystem/imcce/
--rw-rw-r--   0 travis    (2000) travis    (2000)      727 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/solarsystem/imcce/imcce.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/solarsystem/jpl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      708 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/solarsystem/jpl/jpl.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/solarsystem/mpc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      663 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/solarsystem/mpc/mpc.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      689 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/solarsystem/solarsystem.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/splatalogue/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12302 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/splatalogue/splatalogue.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/template.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3399 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/testing.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/ukidss/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12666 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/ukidss/ukidss.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24555 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/utils/tap.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      330 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/utils.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/vamdc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1344 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vamdc/vamdc.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/vizier/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14072 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vizier/vizier.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/vo_conesearch/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24804 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vo_conesearch/client.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/vo_conesearch/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21397 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vo_conesearch/images/astroquery_vo_flowchart.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    35668 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vo_conesearch/images/client_predict_search_n.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    28522 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vo_conesearch/images/client_predict_search_t.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    24576 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vo_conesearch/images/validator_html_1.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    61145 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vo_conesearch/images/validator_html_2.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    31796 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vo_conesearch/images/validator_html_3.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    53922 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vo_conesearch/images/validator_html_4.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    13539 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vo_conesearch/validator.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     8979 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vo_conesearch/vo_conesearch.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/vsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      567 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/vsa/vsa.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/wfau/
--rw-rw-r--   0 travis    (2000) travis    (2000)      481 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/wfau/wfau.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/docs/xmatch/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2786 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/docs/xmatch/xmatch.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 20:45:32.000000 astroquery-0.4.dev5744/licenses/
--rw-rw-r--   0 travis    (2000) travis    (2000)      257 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/licenses/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/licenses/SCHEMA.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2809 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4838 2019-10-08 20:41:36.000000 astroquery-0.4.dev5744/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19152 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/CHANGES.rst
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/CITATION -> astroquery/CITATION
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1497 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/LICENSE.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      421 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11369 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37494 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/ah_bootstrap.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18166 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/CHANGES.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1491 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/LICENSE.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2587 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37494 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/ah_bootstrap.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1836 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2940 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/_dummy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11722 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/_test_compat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19785 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/build_ext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1454 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/build_py.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10935 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/build_sphinx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      486 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/install.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      512 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/install_lib.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/register.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/src/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3033 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/src/compiler.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1364 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/compat/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      368 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/compat/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1647 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7922 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/distutils_helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      589 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5398 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/autodoc_enhancements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16490 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/automodapi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27764 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/automodsumm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4148 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/smart_resolver.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7140 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/numpydoc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      194 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/numpydoc/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19206 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15160 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape_sphinx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11395 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/numpydoc/numpydoc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6465 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/git_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3145 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/openmp_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27888 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/setup_helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      437 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11873 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/conf.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3193 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5940 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/local/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      562 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1638 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      658 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2820 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/globaltoc.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3433 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)       34 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/localtoc.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/searchbox.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5201 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1725 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32988 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1884 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12067 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2769 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4971 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)      192 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/theme.conf
+-rw-rw-r--   0 travis    (2000) travis    (2000)      515 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27125 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      569 2019-10-10 04:47:37.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10035 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/version_helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3946 2019-10-10 04:47:37.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3278 2019-10-10 04:47:37.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-10 04:47:37.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-10 04:47:37.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-10-10 04:47:37.000000 astroquery-0.4.dev5750/astropy_helpers/astropy_helpers.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astropy_helpers/licenses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1644 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2505 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5959 2019-10-10 04:44:03.000000 astroquery-0.4.dev5750/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1330 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/CITATION
+-rw-rw-r--   0 travis    (2000) travis    (2000)      992 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2023 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/_astropy_init.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/alfalfa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      494 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alfalfa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6620 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alfalfa/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/alfalfa/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alfalfa/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/alfalfa/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4226 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alfalfa/tests/data/alfalfa_cat_small.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    83520 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alfalfa/tests/data/alfalfa_sp.fits
+-rw-rw-r--   0 travis    (2000) travis    (2000)      291 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alfalfa/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2442 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alfalfa/tests/test_alfalfa.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/alma/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      863 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47339 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/alma/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36513 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/data/cycle0_delivery_asdm_mapping.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      264 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/alma/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11891 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/data_list_page.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      418 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/downloadRequest519752156script.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      376 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/downloadRequest786572566script.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4306 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/downloadRequest786978956script.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2686 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/downloadRequest787632764script.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/empty.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39698 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/etacar_query.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2759 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/initial_response.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)  2319422 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/m83_March25_2015.votable.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42792 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/ngc4945.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42990 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/querypage.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13491 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/request_786572566.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53200 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/request_786978956.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69518 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/request_787632764.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15293 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/request_801926122.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11891 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/staging_submission.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/data/summary_519752156.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      376 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7972 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/test_alma.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13316 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/test_alma_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3583 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/tests/test_alma_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22712 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/alma/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      853 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17909 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37440 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/test-source-list.fit
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17280 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/test-wcs-sol.fit
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42485 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/thumbnail-image.fit.gz
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11520 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/thumbnail-wcs-sol-from-photutils.fit
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17280 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/thumbnail-wcs-sol.fit
+-rw-rw-r--   0 travis    (2000) travis    (2000)      374 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6898 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/test_astrometry_net.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astrometry_net/tests/test_astrometry_net_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5605 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/astroquery.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/atomic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2603 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/atomic/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15742 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/atomic/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      154 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/atomic/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/atomic/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/atomic/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/atomic/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45949 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/atomic/tests/data/default_params_result.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      432 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/atomic/tests/data/empty_results.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2951 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/atomic/tests/test_atomic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3302 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/atomic/tests/test_atomic_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      482 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/atomic/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/besancon/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1300 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15502 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7428 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/data/1376235131.430670.resu
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7428 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/data/besancon_test.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8106 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/data/besancon_test2.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2465 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/data/default_params.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      466 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/data/query_return.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6787 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/data/query_return.iframe.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      337 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3872 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/besancon/tests/test_besancon.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/cadc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      935 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29901 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      645 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/DummyJob.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4486 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/DummyTapHandler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3821 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/data/datalink_result.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/data/job_1.vot
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51840 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/data/query_images.fits
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4591 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/data/tap_caps.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      598 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15988 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/test_cadctap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10981 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cadc/tests/test_cadctap_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/cds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1365 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18113 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cds/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/cds/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cds/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/cds/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cds/tests/data/hips_from_saada_alasky.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      223 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cds/tests/data/properties.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      135 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cds/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5153 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cds/tests/test_mocserver.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3171 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cds/tests/test_mocserver_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3052 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/conftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/cosmosim/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cosmosim/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58419 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cosmosim/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/cosmosim/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cosmosim/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/cosmosim/tests/test_cosmosim.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/esa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      951 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15358 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      226 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/data/F05I0602M.tar
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/data/J6FL25S4Q.tar
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/data/X0MC5101T.tar
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/data/metadata.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/data/region.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/data/target.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2712 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/dummy_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3469 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/dummy_tap_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      515 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5331 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esa/hubble/tests/test_esa_hubble.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/esasky/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      680 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esasky/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37868 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esasky/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/esasky/tests/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esasky/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/esasky/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28700 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esasky/tests/data/catalogs.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16100 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esasky/tests/data/observations.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      555 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esasky/tests/setup_package.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1722 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esasky/tests/test_esasky.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3960 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/esasky/tests/test_esasky_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/eso/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      721 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45553 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/eso/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39108 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/47cae7cb7578c2a4f0461b4897e6a05a747d3b79aad09a25168c0463.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29615 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/862b6db5bf174fb89ee7ddc42d0fcd49d864388bc3c0dc6f6f64744b.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)      463 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/a77820a9fdbaa8ca10322e0832595e3ce59b9b28241ade00bd846ce6.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35621 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/amber_query_form.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10143 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/amber_sgra_query.tbl
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26370 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/c3931c90b484ef51fb10ad6370d9e5af99de668e116460c36fe1d1c5.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27132 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/da4b7c06e277275f197d8681bf5fdc0ecd556ed07e6aac8cbf0249d2.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25415 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/de77b0a24235373d6bbf8487ba825fcd634768f43da682614d202ffc.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29128 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/e2c39d36193cdb16ce871845157c1e50ff539cf8122d87a8282854b9.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)      383 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/efafb320926e82995df2dc4e2ea745de75c51ea90b7ed52bc6569105.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25361 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/main_query_form.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/main_sgra_query.tbl
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50742 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/vvv_sgra_form.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14321 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/data/vvv_sgra_survey_response.tbl
+-rw-rw-r--   0 travis    (2000) travis    (2000)      334 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3190 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/test_eso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8017 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/eso/tests/test_eso_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2207 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/exceptions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      688 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3770 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/data/exoplanet_orbit_database_units.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4114 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/exoplanet_orbit_database.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      313 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      133 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6355 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/tests/data/exoplanet_orbit_database.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4841 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/tests/test_exoplanet_orbit_database.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/fermi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1022 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/fermi/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5291 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/fermi/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      245 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/fermi/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/fermi/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/fermi/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/fermi/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6705 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/fermi/tests/data/query_result_m31.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8490 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/fermi/tests/data/result_page_m31.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2503 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/fermi/tests/test_fermi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/fermi/tests/test_fermi_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/gaia/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      968 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gaia/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23093 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gaia/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/gaia/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13160 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gaia/tests/DummyTapHandler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      284 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gaia/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/gaia/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gaia/tests/data/job_1.vot
+-rw-rw-r--   0 travis    (2000) travis    (2000)      509 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gaia/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24624 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gaia/tests/test_gaiatap.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/gama/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      287 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gama/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2284 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gama/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/gama/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gama/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/gama/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11520 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gama/tests/data/GAMA_HzVs28.fits
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48879 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gama/tests/data/query_result.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      289 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gama/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1008 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gama/tests/test_gama.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      662 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/gama/tests/test_gama_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/heasarc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1255 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/heasarc/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13184 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/heasarc/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/heasarc/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/heasarc/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      290 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/heasarc/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/heasarc/tests/test_heasarc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2167 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/heasarc/tests/test_heasarc_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/hitran/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      867 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/hitran/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11868 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/hitran/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/hitran/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5303 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/hitran/data/readme.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      357 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/hitran/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/hitran/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/hitran/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/hitran/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19764 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/hitran/tests/data/H2O.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1949 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/hitran/tests/test_hitran.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/hitran/tests/test_hitran_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4716 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/hitran/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ibe/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1271 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16715 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34515 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/data/columns.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      844 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/data/datasets.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50778 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/data/field_id.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      907 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/data/missions.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50600 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/data/pos.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1308 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/data/tables.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      287 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3077 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/test_ibe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      794 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ibe/tests/test_ibe_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/imcce/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2555 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30225 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5238 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype1.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7294 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype2.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4806 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype3.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4807 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype4.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7453 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype5.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6244 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype6.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35514 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/data/skybot_query.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)      259 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4550 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/test_miriade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      703 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/test_miriade_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4565 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/test_skybot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1176 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/imcce/tests/test_skybot_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/irsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      994 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21068 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/irsa/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/irsa/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4171 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa/tests/data/Box.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4308 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa/tests/data/Cone.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4307 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa/tests/data/Cone_coord.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7775 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa/tests/data/Polygon.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      243 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6208 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa/tests/test_irsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2074 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa/tests/test_irsa_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      961 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40935 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      116 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/dust-error.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4377 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/dust_ext_detail.tbl
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2573 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/dustm101.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/dustm31.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2569 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/dustm81.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)   331200 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/test.fits
+-rw-rw-r--   0 travis    (2000) travis    (2000)      381 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15511 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/test_irsa_dust.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7285 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/tests/test_irsa_dust_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2980 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/irsa_dust/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9018 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65635 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7361 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/tests/data/ceres_elements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15088 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/tests/data/ceres_ephemerides.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6823 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/tests/data/ceres_vectors.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28929 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/tests/data/no_H.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8416 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/tests/test_jplhorizons.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15091 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplhorizons/tests/test_jplhorizons_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1607 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16553 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20313 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/67P.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53829 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/apophis.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7044 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/ceres.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7029 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/ceres_missing_value.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38098 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/phaethon.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)      315 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3496 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/test_jplsbdb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplsbdb/tests/test_jplsbdb_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/jplspec/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      727 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10228 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/jplspec/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31527 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/data/catdir.cat
+-rw-rw-r--   0 travis    (2000) travis    (2000)      932 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/lookup_table.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      454 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/jplspec/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/jplspec/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      681 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/tests/data/CO.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/tests/data/CO_6.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17016 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/tests/data/multi.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3939 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/tests/test_jplspec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/jplspec/tests/test_jplspec_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/lamda/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      701 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lamda/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14121 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lamda/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/lamda/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lamda/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/lamda/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25560 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lamda/tests/data/co.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      244 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lamda/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lamda/tests/test_lamda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      466 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lamda/tests/test_lamda_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4951 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lamda/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/lcogt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1098 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lcogt/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17299 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lcogt/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/lcogt/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lcogt/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/lcogt/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4171 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lcogt/tests/data/Box.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4308 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lcogt/tests/data/Cone.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4307 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lcogt/tests/data/Cone_coord.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7775 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lcogt/tests/data/Polygon.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      244 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lcogt/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6349 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lcogt/tests/test_lcogt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2683 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/lcogt/tests/test_lcogt_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/magpis/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      838 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/magpis/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4910 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/magpis/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/magpis/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/magpis/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/magpis/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   365760 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/magpis/tests/data/image.fits
+-rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/magpis/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2343 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/magpis/tests/test_magpis.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      822 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/magpis/tests/test_magpis_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/mast/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1249 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    93700 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6730 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/fpl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13515 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tesscut.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/mast/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3904 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/advSearch.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12466 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/advSearchPos.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   260927 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/astrocut_107.27_-70.0_5x5.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)      537 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/bundleResponse.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18958 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/caom.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12347 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/columnsconfig.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      221 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/countsResp.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15794 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/dd.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1936 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/ddcolumns.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   674902 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/ddcolumns_filtered.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35770 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/hsc.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11755 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/matchid.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   225915 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/missions.extjs
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8185 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/panstarrs.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12359 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/products.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/resolver.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13369 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/spectra.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       86 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/tess_sector.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15817 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/tic.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6807 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/ticcolumns.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   423717 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/data/ticcolumns_filtered.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      236 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22004 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/test_mast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26157 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mast/tests/test_mast_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/mpc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56316 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      324 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9296 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/1994XG_ephemeris_500-a-t.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10133 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/1994XG_ephemeris_G37-a-t.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2556 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_500-G-t.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3076 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_500-a-c.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3075 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_500-a-s.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3075 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_500-a-t.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3615 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_500-s-t.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3903 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_G37-a-t.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      702 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/ObsCodes.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)   337798 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/mpc_obs.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/data/testfail_ephemeris_500-a-t.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16944 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/test_mpc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4707 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/mpc/tests/test_mpc_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nasa_ads/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1030 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_ads/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4066 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_ads/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nasa_ads/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_ads/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nasa_ads/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      744 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_ads/tests/data/test_text.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_ads/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_ads/tests/test_nasaads.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      388 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_ads/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      670 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1599 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/data/exoplanet_nexsci_units.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4988 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/nasa_exoplanet_archive.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      311 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/tests/data/nasa_exoplanet_archive.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5038 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/tests/test_nasa_exoplanet_archive_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ned/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2566 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28522 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ned/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44661 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/data/keywords_dict.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ned/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      862 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/error.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7550 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/image_extract.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13031 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_diameters.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11033 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_iau_format.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72000 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_images.fits
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6577 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_near_name.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)   126513 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_near_position.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40517 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_notes.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5183 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_object.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)   277494 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_photometry.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8352 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_positions.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8704 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_redshifts.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14494 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_refcode.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7509 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/data/query_references.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9913 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/test_ned.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3307 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ned/tests/test_ned_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nist/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      634 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nist/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7775 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nist/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nist/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nist/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nist/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24444 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nist/tests/data/nist_out.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      239 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nist/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1740 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nist/tests/test_nist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1173 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nist/tests/test_nist_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nrao/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      742 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nrao/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19954 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nrao/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nrao/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nrao/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nrao/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   263122 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nrao/tests/data/archive_html.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)   793497 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nrao/tests/data/votable.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      289 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nrao/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4278 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nrao/tests/test_nrao.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2189 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nrao/tests/test_nrao_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nvas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      777 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nvas/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9887 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nvas/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nvas/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nvas/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/nvas/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66240 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nvas/tests/data/image.imfits
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16956 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nvas/tests/data/image_results.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nvas/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4404 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nvas/tests/test_nvas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      918 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/nvas/tests/test_nvas_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/oac/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      934 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/oac/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19861 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/oac/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/oac/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/oac/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/oac/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34404 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/oac/tests/data/photometry_csv.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41357 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/oac/tests/data/photometry_json.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46287 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/oac/tests/data/single_spectrum_csv.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)   157121 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/oac/tests/data/spectra_json.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      290 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/oac/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3191 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/oac/tests/test_oac.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2890 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/oac/tests/test_oac_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ogle/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1061 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ogle/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7627 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ogle/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ogle/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ogle/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ogle/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      197 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ogle/tests/data/gal_0_3.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      239 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ogle/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1716 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ogle/tests/test_ogle.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      280 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2374 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/oec_query.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   244625 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/tests/data/systems.xml.gz
+-rw-rw-r--   0 travis    (2000) travis    (2000)      383 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      735 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/tests/test_open_exoplanet_catalogue_local.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      489 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/tests/test_open_exoplanet_catalogue_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9006 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16704 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/query.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/sdss/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      854 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46643 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/sdss/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115564 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/data/PhotoObjAll_dr12.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46061 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/data/SpecObjAll_dr12.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3201 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/field_names.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/sdss/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/sdss/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2880 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/tests/data/emptyfile.fits
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1163 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/tests/data/xid_im.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      206 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/tests/data/xid_sp.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13504 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/tests/test_sdss.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6746 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sdss/tests/test_sdss_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      187 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/sha/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      446 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sha/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8261 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sha/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/sha/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sha/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/sha/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95040 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sha/tests/data/img.fits
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3377 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sha/tests/data/nid_t.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)   374026 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sha/tests/data/pid_t.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20311 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sha/tests/data/pos_t.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5276 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sha/tests/data/rqk_t.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sha/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2202 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/sha/tests/test_sha.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/simbad/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1101 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40364 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/simbad/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7947 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/data/votable_fields_dict.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      503 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/data/votable_fields_notes.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1602 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/get_votable_fields.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      960 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3165 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/m1.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)      838 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_bibcode.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3843 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_bibobj.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20797 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_cat.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14181 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_coo.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1130 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_error.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3165 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_id.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)      932 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_objectids.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1977 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_sample.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4548 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_sample_region.data
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17911 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/test_simbad.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8057 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/simbad/tests/test_simbad_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/skyview/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      466 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/skyview/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14126 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/skyview/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      336 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/skyview/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/skyview/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/skyview/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/skyview/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   122244 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/skyview/tests/data/query_page.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32703 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/skyview/tests/data/results.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3616 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/skyview/tests/data/survey_dict.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2963 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/skyview/tests/test_skyview.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1722 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/skyview/tests/test_skyview_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/solarsystem/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      247 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/solarsystem/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/solarsystem/imcce/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      242 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/solarsystem/imcce/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/solarsystem/imcce/miriade/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      240 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/solarsystem/imcce/miriade/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/solarsystem/imcce/skybot/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      236 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/solarsystem/imcce/skybot/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/solarsystem/jpl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      235 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/solarsystem/jpl/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/solarsystem/jpl/horizons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/solarsystem/jpl/horizons/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/solarsystem/jpl/sbdb/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      226 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/solarsystem/jpl/sbdb/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/solarsystem/mpc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      208 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/solarsystem/mpc/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/splatalogue/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1106 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1286 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/build_species_table.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21208 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/splatalogue/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56822 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/data/species.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/load_species_table.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      409 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1827 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/slap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      439 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/splatalogue/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/splatalogue/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1037 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/tests/data/CO_colons.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6119 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/tests/test_splatalogue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/tests/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/splatalogue/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/template_module/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1078 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/template_module/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13780 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/template_module/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/template_module/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/template_module/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/template_module/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       92 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/template_module/tests/data/dummy.dat
+-rw-rw-r--   0 travis    (2000) travis    (2000)      520 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/template_module/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3115 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/template_module/tests/test_module.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      488 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/template_module/tests/test_module_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      768 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/tests/coveragerc
+-rw-rw-r--   0 travis    (2000) travis    (2000)      201 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      424 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/tests/test_internet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1284 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/tests/test_resume.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ukidss/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      925 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2529 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2303 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/data/error.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)   385920 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/data/image.fits
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1098 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/data/image_results.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13757 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/data/vo_results.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4985 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/data/votable.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      336 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5745 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/test_ukidss.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2270 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/ukidss/tests/test_ukidss_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      402 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1018 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/class_or_instance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15084 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/commons.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8399 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1271 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/docstr_chompers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4217 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/download_file_list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2623 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/process_asyncs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1945 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/progressbar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6260 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/schema.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2271 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/system_tools.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      547 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/conn/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/conn/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    25239 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/conn/tapconn.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1624 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/DummyConn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5329 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/DummyConnHandler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1862 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/DummyResponse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      424 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6649 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/test_conn.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    81617 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/gui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/gui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3911 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/gui/login.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1489 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/filter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      915 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/group.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    17476 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/modelutils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      952 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/shared_item.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      752 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/shared_to_item.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1091 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/tapcolumn.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1274 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/taptable.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/tests/data/result_1.vot
+-rw-rw-r--   0 travis    (2000) travis    (2000)      468 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3911 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/tests/test_job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      612 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/model/user.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5824 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/taputils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/tests/data/job_1.vot
+-rw-rw-r--   0 travis    (2000) travis    (2000)      573 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/tests/data/jobs_list.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1123 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/tests/data/test_table1.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1931 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/tests/data/test_tables.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      729 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35694 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/tests/test_tap.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3732 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/groupSaxParser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2823 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/jobListSaxParser.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4431 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/jobSaxParser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3840 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/sharedItemsSaxParser.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6292 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tableSaxParser.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10867 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/data/test_job_results.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1790 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/data/test_jobs_async.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      646 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/data/test_jobs_list.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1931 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/data/test_tables.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      516 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3758 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/test_xmlparser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1724 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/testing_tools.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/utils/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2142 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tests/test_timer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      384 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tests/test_url_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14141 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/tests/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10840 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/timer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1603 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/utils/url_helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vamdc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      575 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vamdc/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3802 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vamdc/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1601 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vamdc/load_species_table.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vamdc/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vamdc/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      510 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vamdc/tests/setup_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      588 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vamdc/tests/test_vamdc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      763 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vamdc/tests/test_vamdc_remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7358 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vizier/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1488 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33047 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vizier/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3364 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/data/inverse_dict.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2171 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/data/keywords_dict.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      628 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vizier/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vizier/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8019 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/tests/data/afgl2591_iram.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9834 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/tests/data/find_kangapj70683.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20706 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/tests/data/kang2010.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)   443070 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/tests/data/viz.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/tests/test_vizier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5449 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vizier/tests/test_vizier_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1242 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16847 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/conesearch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7804 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1133 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      207 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/data/basic.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      251 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/data/conesearch_error1.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      300 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/data/conesearch_error2.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      339 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/data/conesearch_error3.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      310 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/data/conesearch_error4.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9009 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/test_conesearch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7031 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/test_vos_catalog.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1486 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/data/conesearch_urls.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      710 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/inspect.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      408 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/conesearch_error.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/conesearch_exception.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3344 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/conesearch_good.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/conesearch_warn.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      355 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/listcats1.out
+-rw-rw-r--   0 travis    (2000) travis    (2000)       97 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/listcats2.out
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2875 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/printcat.out
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/tally.out
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3844 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/vao_conesearch_sites_121107_subset.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2641 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/test_inpect.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3114 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/test_validate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2961 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tstquery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11351 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/validate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2609 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/vo_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28184 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vo_conesearch/vos_catalog.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      928 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2909 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vsa/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/vsa/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vsa/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2871 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/vsa/tests/test_vista_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/wfau/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      597 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/wfau/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37041 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/wfau/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/xmatch/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      558 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/xmatch/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7891 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/xmatch/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      245 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/xmatch/setup_package.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/xmatch/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/xmatch/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/astroquery/xmatch/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      140 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/xmatch/tests/data/posList.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      301 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/xmatch/tests/data/poslist_duplicates.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1688 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/xmatch/tests/data/query_res.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)   275304 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/xmatch/tests/data/tables.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4295 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/xmatch/tests/test_xmatch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4439 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/astroquery/xmatch/tests/test_xmatch_remote.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4581 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/Makefile
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/_static/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28453 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/_static/timer_prediction_pow10.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/_templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/_templates/autosummary/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      250 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/_templates/autosummary/base.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      251 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      252 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/_templates/autosummary/module.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/alfalfa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1550 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/alfalfa/alfalfa.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/alma/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7629 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/alma/alma.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8783 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/api.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/astrometry_net/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12990 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/astrometry_net/astrometry_net.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/atomic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2171 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/atomic/atomic.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/besancon/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5752 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/besancon/besancon.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/cadc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25091 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/cadc/cadc.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/cds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   140621 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/cds/HST_union.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   131787 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/cds/MOC_GALEXGR6_AIS_FUV.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44330 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/cds/cds.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7588 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/conf.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/cosmosim/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19150 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/cosmosim/cosmosim.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/demos/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   518906 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/demos/Astroquery_DotAstro_Demo.ipynb
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/esa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4679 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/esa/hubble.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/esasky/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9965 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/esasky/esasky.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/eso/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16639 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/eso/eso.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/exoplanet_orbit_database/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2290 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/exoplanet_orbit_database/exoplanet_orbit_database.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/fermi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      995 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/fermi/fermi.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/gaia/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27623 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gaia/gaia.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/gallery-examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1538 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/example10_mast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      930 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/example1_vizier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      717 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/example2_simbad.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      216 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/example3_simbad.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      738 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/example4_simbad.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      252 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/example5_oec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/example6_alma.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10578 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/example7_alma.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      793 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/example8_eso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1965 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/example9_skyview_vizier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      380 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery-examples/run_examples.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2464 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gallery.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/gama/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3986 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/gama/gama.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/heasarc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8906 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/heasarc/heasarc.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/hitran/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1349 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/hitran/hitran.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/ibe/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      993 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/ibe/ibe.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/imcce/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26921 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/imcce/imcce.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9585 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/index.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/irsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12157 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/irsa/irsa.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9213 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/irsa/irsa_dust.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/jplhorizons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24374 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/jplhorizons/jplhorizons.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:57.000000 astroquery-0.4.dev5750/docs/jplsbdb/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11843 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/jplsbdb/jplsbdb.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/jplspec/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/jplspec/images/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37257 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/jplspec/images/docplot_curvefit.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25216 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/jplspec/images/docplot_jplspec.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11376 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/jplspec/jplspec.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/lamda/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1456 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/lamda/lamda.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/license.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/magpis/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2502 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/magpis/magpis.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4513 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1222 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/make_doctests.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/mast/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55480 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/mast/mast.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/mpc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26623 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/mpc/mpc.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/nasa_ads/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2068 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/nasa_ads/nasa_ads.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/nasa_exoplanet_archive/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2324 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/nasa_exoplanet_archive/nasa_exoplanet_archive.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/ned/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13635 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/ned/ned.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/nist/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7683 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/nist/nist.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/nrao/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4405 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/nrao/nrao.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/nvas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4683 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/nvas/nvas.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/oac/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5805 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/oac/oac.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/ogle/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1600 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/ogle/ogle.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/open_exoplanet_catalogue/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4548 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/open_exoplanet_catalogue/open_exoplanet_catalogue.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      250 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/query.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1912 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/release_notice_v0.2.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/sdss/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2792 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/sdss/sdss.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/sha/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2410 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/sha/sha.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/simbad/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33218 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/simbad/simbad.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/skyview/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9614 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/skyview/skyview.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/solarsystem/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/solarsystem/imcce/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      727 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/solarsystem/imcce/imcce.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/solarsystem/jpl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      708 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/solarsystem/jpl/jpl.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/solarsystem/mpc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      663 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/solarsystem/mpc/mpc.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      689 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/solarsystem/solarsystem.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/splatalogue/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12302 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/splatalogue/splatalogue.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/template.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3399 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/testing.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/ukidss/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12666 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/ukidss/ukidss.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24555 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/utils/tap.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      398 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/utils.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/vamdc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1344 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vamdc/vamdc.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/vizier/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14072 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vizier/vizier.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/vo_conesearch/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24804 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vo_conesearch/client.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/vo_conesearch/images/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21397 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vo_conesearch/images/astroquery_vo_flowchart.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35668 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vo_conesearch/images/client_predict_search_n.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28522 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vo_conesearch/images/client_predict_search_t.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24576 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vo_conesearch/images/validator_html_1.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61145 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vo_conesearch/images/validator_html_2.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31796 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vo_conesearch/images/validator_html_3.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53922 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vo_conesearch/images/validator_html_4.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13539 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vo_conesearch/validator.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8979 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vo_conesearch/vo_conesearch.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/vsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      567 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/vsa/vsa.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/wfau/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/wfau/wfau.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/docs/xmatch/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2786 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/docs/xmatch/xmatch.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-10 04:47:58.000000 astroquery-0.4.dev5750/licenses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      257 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/licenses/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/licenses/SCHEMA.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2809 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4838 2019-10-10 04:44:02.000000 astroquery-0.4.dev5750/setup.py
```

### Comparing `astroquery-0.4.dev5744/CHANGES.rst` & `astroquery-0.4.dev5750/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,16 @@
 
 ukidss
 ^^^^^^
 
 utils
 ^^^^^
 
+- Added timer functions. [#1508]
+
 vamdc
 ^^^^^
 
 vizier
 ^^^^^^
 
 vo_conesearch
```

### Comparing `astroquery-0.4.dev5744/LICENSE.rst` & `astroquery-0.4.dev5750/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/README.rst` & `astroquery-0.4.dev5750/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
        MAIN_ID          RA           DEC      ... COO_QUAL COO_WAVELENGTH     COO_BIBCODE
     ------------- ------------- ------------- ... -------- -------------- -------------------
     * tet01 Ori C 05 35 16.4637 -05 23 22.848 ...        A              O 2007A&A...474..653V
 
 Installation and Requirements
 -----------------------------
 
-Astroquery works with Python 2.7 and 3.5 or later.
+Astroquery works with Python 3.6 or later.
 As an `astropy`_ affiliate, astroquery requires `astropy`_ version 2.0 or later.
 
 astroquery uses the `requests <http://docs.python-requests.org/en/latest/>`_
 module to communicate with the internet.  `BeautifulSoup
 <http://www.crummy.com/software/BeautifulSoup/>`_ and `html5lib'
 <https://html5lib.readthedocs.io/en/latest/>`_ are needed for HTML parsing for
 some services.  The `keyring <https://pypi.python.org/pypi/keyring>`_ module is
```

### Comparing `astroquery-0.4.dev5744/ah_bootstrap.py` & `astroquery-0.4.dev5750/ah_bootstrap.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/CHANGES.rst` & `astroquery-0.4.dev5750/astropy_helpers/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/LICENSE.rst` & `astroquery-0.4.dev5750/astropy_helpers/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/README.rst` & `astroquery-0.4.dev5750/astropy_helpers/README.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/ah_bootstrap.py` & `astroquery-0.4.dev5750/astropy_helpers/ah_bootstrap.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/__init__.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/_dummy.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/_dummy.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/_test_compat.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/_test_compat.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/build_ext.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/build_ext.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/build_py.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/build_py.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/build_sphinx.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/build_sphinx.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/install_lib.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/install_lib.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/register.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/register.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/src/compiler.c` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/src/compiler.c`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/commands/test.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/commands/test.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/conftest.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/conftest.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/distutils_helpers.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/distutils_helpers.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/__init__.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/autodoc_enhancements.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/autodoc_enhancements.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/automodapi.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/automodapi.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/automodsumm.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/automodsumm.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/smart_resolver.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/smart_resolver.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/automodapi/utils.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/automodapi/utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape_sphinx.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/numpydoc/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/extern/numpydoc/numpydoc.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/extern/numpydoc/numpydoc.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/git_helpers.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/git_helpers.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/openmp_helpers.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/openmp_helpers.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/setup_helpers.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/conf.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/ext/changelog_links.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/ext/doctest.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/ext/edit_on_github.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.inv`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/local/python2_local_links.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.inv`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/local/python3_local_links.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/layout.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout.svg`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_linkout_20.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.ico`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo.svg`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/astropy_logo_32.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/bootstrap-astropy.css`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/copybutton.js`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/sphinx/themes/bootstrap-astropy/static/sidebar.js`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/test_helpers.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/test_helpers.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/utils.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/version.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Autogenerated by Astropy-affiliated package astropy_helpers's setup.py on 2019-10-08 20:45:12 UTC
+# Autogenerated by Astropy-affiliated package astropy_helpers's setup.py on 2019-10-10 04:47:37 UTC
 from __future__ import unicode_literals
 import datetime
 
 version = "2.0.10"
 githash = "fd80be7cf8698e2350a919ef7fc89871db0ba580"
 
 
 major = 2
 minor = 0
 bugfix = 10
 
 release = True
-timestamp = datetime.datetime(2019, 10, 8, 20, 45, 12)
+timestamp = datetime.datetime(2019, 10, 10, 4, 47, 37)
 debug = False
 
 astropy_helpers_version = ""
 
 try:
     from ._compiler import compiler
 except ImportError:
```

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers/version_helpers.py` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers/version_helpers.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers.egg-info/PKG-INFO` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt` & `astroquery-0.4.dev5750/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst` & `astroquery-0.4.dev5750/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst` & `astroquery-0.4.dev5750/astropy_helpers/licenses/LICENSE_COPYBUTTON.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst` & `astroquery-0.4.dev5750/astropy_helpers/licenses/LICENSE_NUMPYDOC.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/CITATION` & `astroquery-0.4.dev5750/astroquery/CITATION`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/__init__.py` & `astroquery-0.4.dev5750/astroquery/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/_astropy_init.py` & `astroquery-0.4.dev5750/astroquery/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alfalfa/core.py` & `astroquery-0.4.dev5750/astroquery/alfalfa/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alfalfa/tests/data/alfalfa_cat_small.txt` & `astroquery-0.4.dev5750/astroquery/alfalfa/tests/data/alfalfa_cat_small.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alfalfa/tests/data/alfalfa_sp.fits` & `astroquery-0.4.dev5750/astroquery/alfalfa/tests/data/alfalfa_sp.fits`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alfalfa/tests/test_alfalfa.py` & `astroquery-0.4.dev5750/astroquery/alfalfa/tests/test_alfalfa.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/__init__.py` & `astroquery-0.4.dev5750/astroquery/alma/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/core.py` & `astroquery-0.4.dev5750/astroquery/alma/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/data/cycle0_delivery_asdm_mapping.txt` & `astroquery-0.4.dev5750/astroquery/alma/data/cycle0_delivery_asdm_mapping.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/data_list_page.html` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/data_list_page.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/downloadRequest786978956script.sh` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/downloadRequest786978956script.sh`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/downloadRequest787632764script.sh` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/downloadRequest787632764script.sh`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/etacar_query.xml` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/etacar_query.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/initial_response.html` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/initial_response.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/m83_March25_2015.votable.xml` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/m83_March25_2015.votable.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/ngc4945.xml` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/ngc4945.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/querypage.html` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/querypage.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/request_786572566.html` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/request_786572566.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/request_786978956.html` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/request_786978956.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/request_787632764.html` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/request_787632764.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/request_801926122.html` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/request_801926122.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/staging_submission.html` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/staging_submission.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/data/summary_519752156.json` & `astroquery-0.4.dev5750/astroquery/alma/tests/data/summary_519752156.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/test_alma.py` & `astroquery-0.4.dev5750/astroquery/alma/tests/test_alma.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/test_alma_remote.py` & `astroquery-0.4.dev5750/astroquery/alma/tests/test_alma_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/tests/test_alma_utils.py` & `astroquery-0.4.dev5750/astroquery/alma/tests/test_alma_utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/alma/utils.py` & `astroquery-0.4.dev5750/astroquery/alma/utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/astrometry_net/__init__.py` & `astroquery-0.4.dev5750/astroquery/astrometry_net/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/astrometry_net/core.py` & `astroquery-0.4.dev5750/astroquery/astrometry_net/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/test-source-list.fit` & `astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/test-source-list.fit`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/test-wcs-sol.fit` & `astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/test-wcs-sol.fit`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/thumbnail-image.fit.gz` & `astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/thumbnail-image.fit.gz`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/thumbnail-wcs-sol-from-photutils.fit` & `astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/thumbnail-wcs-sol-from-photutils.fit`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/astrometry_net/tests/data/thumbnail-wcs-sol.fit` & `astroquery-0.4.dev5750/astroquery/astrometry_net/tests/data/thumbnail-wcs-sol.fit`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/astrometry_net/tests/test_astrometry_net.py` & `astroquery-0.4.dev5750/astroquery/astrometry_net/tests/test_astrometry_net.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/astrometry_net/tests/test_astrometry_net_remote.py` & `astroquery-0.4.dev5750/astroquery/astrometry_net/tests/test_astrometry_net_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/astroquery.cfg` & `astroquery-0.4.dev5750/astroquery/astroquery.cfg`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/atomic/__init__.py` & `astroquery-0.4.dev5750/astroquery/atomic/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/atomic/core.py` & `astroquery-0.4.dev5750/astroquery/atomic/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/atomic/tests/data/default_params_result.html` & `astroquery-0.4.dev5750/astroquery/atomic/tests/data/default_params_result.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/atomic/tests/test_atomic.py` & `astroquery-0.4.dev5750/astroquery/atomic/tests/test_atomic.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/atomic/tests/test_atomic_remote.py` & `astroquery-0.4.dev5750/astroquery/atomic/tests/test_atomic_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/besancon/__init__.py` & `astroquery-0.4.dev5750/astroquery/besancon/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/besancon/core.py` & `astroquery-0.4.dev5750/astroquery/besancon/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/besancon/tests/data/1376235131.430670.resu` & `astroquery-0.4.dev5750/astroquery/besancon/tests/data/1376235131.430670.resu`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/besancon/tests/data/besancon_test.txt` & `astroquery-0.4.dev5750/astroquery/besancon/tests/data/besancon_test.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/besancon/tests/data/besancon_test2.txt` & `astroquery-0.4.dev5750/astroquery/besancon/tests/data/besancon_test2.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/besancon/tests/data/default_params.txt` & `astroquery-0.4.dev5750/astroquery/besancon/tests/data/default_params.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/besancon/tests/data/query_return.iframe.html` & `astroquery-0.4.dev5750/astroquery/besancon/tests/data/query_return.iframe.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/besancon/tests/test_besancon.py` & `astroquery-0.4.dev5750/astroquery/besancon/tests/test_besancon.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/__init__.py` & `astroquery-0.4.dev5750/astroquery/cadc/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/core.py` & `astroquery-0.4.dev5750/astroquery/cadc/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/tests/DummyJob.py` & `astroquery-0.4.dev5750/astroquery/cadc/tests/DummyJob.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/tests/DummyTapHandler.py` & `astroquery-0.4.dev5750/astroquery/cadc/tests/DummyTapHandler.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/tests/data/datalink_result.xml` & `astroquery-0.4.dev5750/astroquery/cadc/tests/data/datalink_result.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/tests/data/job_1.vot` & `astroquery-0.4.dev5750/astroquery/cadc/tests/data/job_1.vot`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/tests/data/query_images.fits` & `astroquery-0.4.dev5750/astroquery/cadc/tests/data/query_images.fits`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/tests/data/tap_caps.xml` & `astroquery-0.4.dev5750/astroquery/cadc/tests/data/tap_caps.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/tests/setup_package.py` & `astroquery-0.4.dev5750/astroquery/cadc/tests/setup_package.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/tests/test_cadctap.py` & `astroquery-0.4.dev5750/astroquery/cadc/tests/test_cadctap.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cadc/tests/test_cadctap_remote.py` & `astroquery-0.4.dev5750/astroquery/cadc/tests/test_cadctap_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cds/__init__.py` & `astroquery-0.4.dev5750/astroquery/cds/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cds/core.py` & `astroquery-0.4.dev5750/astroquery/cds/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cds/tests/test_mocserver.py` & `astroquery-0.4.dev5750/astroquery/cds/tests/test_mocserver.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cds/tests/test_mocserver_remote.py` & `astroquery-0.4.dev5750/astroquery/cds/tests/test_mocserver_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/conftest.py` & `astroquery-0.4.dev5750/astroquery/conftest.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cosmosim/__init__.py` & `astroquery-0.4.dev5750/astroquery/cosmosim/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/cosmosim/core.py` & `astroquery-0.4.dev5750/astroquery/cosmosim/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esa/hubble/__init__.py` & `astroquery-0.4.dev5750/astroquery/esa/hubble/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esa/hubble/core.py` & `astroquery-0.4.dev5750/astroquery/esa/hubble/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esa/hubble/tests/dummy_handler.py` & `astroquery-0.4.dev5750/astroquery/esa/hubble/tests/dummy_handler.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esa/hubble/tests/dummy_tap_handler.py` & `astroquery-0.4.dev5750/astroquery/esa/hubble/tests/dummy_tap_handler.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esa/hubble/tests/setup_package.py` & `astroquery-0.4.dev5750/astroquery/esa/hubble/tests/setup_package.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esa/hubble/tests/test_esa_hubble.py` & `astroquery-0.4.dev5750/astroquery/esa/hubble/tests/test_esa_hubble.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esasky/__init__.py` & `astroquery-0.4.dev5750/astroquery/esasky/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esasky/core.py` & `astroquery-0.4.dev5750/astroquery/esasky/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esasky/tests/data/catalogs.txt` & `astroquery-0.4.dev5750/astroquery/esasky/tests/data/catalogs.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esasky/tests/data/observations.txt` & `astroquery-0.4.dev5750/astroquery/esasky/tests/data/observations.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esasky/tests/setup_package.py` & `astroquery-0.4.dev5750/astroquery/esasky/tests/setup_package.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esasky/tests/test_esasky.py` & `astroquery-0.4.dev5750/astroquery/esasky/tests/test_esasky.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/esasky/tests/test_esasky_remote.py` & `astroquery-0.4.dev5750/astroquery/esasky/tests/test_esasky_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/__init__.py` & `astroquery-0.4.dev5750/astroquery/eso/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/core.py` & `astroquery-0.4.dev5750/astroquery/eso/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/47cae7cb7578c2a4f0461b4897e6a05a747d3b79aad09a25168c0463.pickle` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/47cae7cb7578c2a4f0461b4897e6a05a747d3b79aad09a25168c0463.pickle`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/862b6db5bf174fb89ee7ddc42d0fcd49d864388bc3c0dc6f6f64744b.pickle` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/862b6db5bf174fb89ee7ddc42d0fcd49d864388bc3c0dc6f6f64744b.pickle`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/amber_query_form.html` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/amber_query_form.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/amber_sgra_query.tbl` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/amber_sgra_query.tbl`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/c3931c90b484ef51fb10ad6370d9e5af99de668e116460c36fe1d1c5.pickle` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/c3931c90b484ef51fb10ad6370d9e5af99de668e116460c36fe1d1c5.pickle`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/da4b7c06e277275f197d8681bf5fdc0ecd556ed07e6aac8cbf0249d2.pickle` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/da4b7c06e277275f197d8681bf5fdc0ecd556ed07e6aac8cbf0249d2.pickle`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/de77b0a24235373d6bbf8487ba825fcd634768f43da682614d202ffc.pickle` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/de77b0a24235373d6bbf8487ba825fcd634768f43da682614d202ffc.pickle`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/e2c39d36193cdb16ce871845157c1e50ff539cf8122d87a8282854b9.pickle` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/e2c39d36193cdb16ce871845157c1e50ff539cf8122d87a8282854b9.pickle`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/main_query_form.html` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/main_query_form.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/main_sgra_query.tbl` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/main_sgra_query.tbl`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/vvv_sgra_form.html` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/vvv_sgra_form.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/data/vvv_sgra_survey_response.tbl` & `astroquery-0.4.dev5750/astroquery/eso/tests/data/vvv_sgra_survey_response.tbl`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/test_eso.py` & `astroquery-0.4.dev5750/astroquery/eso/tests/test_eso.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/eso/tests/test_eso_remote.py` & `astroquery-0.4.dev5750/astroquery/eso/tests/test_eso_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/exceptions.py` & `astroquery-0.4.dev5750/astroquery/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/__init__.py` & `astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/data/exoplanet_orbit_database_units.json` & `astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/data/exoplanet_orbit_database_units.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/exoplanet_orbit_database.py` & `astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/exoplanet_orbit_database.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/tests/data/exoplanet_orbit_database.csv` & `astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/tests/data/exoplanet_orbit_database.csv`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/exoplanet_orbit_database/tests/test_exoplanet_orbit_database.py` & `astroquery-0.4.dev5750/astroquery/exoplanet_orbit_database/tests/test_exoplanet_orbit_database.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/fermi/__init__.py` & `astroquery-0.4.dev5750/astroquery/fermi/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/fermi/core.py` & `astroquery-0.4.dev5750/astroquery/fermi/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/fermi/tests/data/query_result_m31.html` & `astroquery-0.4.dev5750/astroquery/fermi/tests/data/query_result_m31.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/fermi/tests/data/result_page_m31.html` & `astroquery-0.4.dev5750/astroquery/fermi/tests/data/result_page_m31.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/fermi/tests/test_fermi.py` & `astroquery-0.4.dev5750/astroquery/fermi/tests/test_fermi.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/fermi/tests/test_fermi_remote.py` & `astroquery-0.4.dev5750/astroquery/fermi/tests/test_fermi_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/gaia/__init__.py` & `astroquery-0.4.dev5750/astroquery/gaia/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/gaia/core.py` & `astroquery-0.4.dev5750/astroquery/gaia/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/gaia/tests/DummyTapHandler.py` & `astroquery-0.4.dev5750/astroquery/gaia/tests/DummyTapHandler.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/gaia/tests/data/job_1.vot` & `astroquery-0.4.dev5750/astroquery/gaia/tests/data/job_1.vot`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/gaia/tests/test_gaiatap.py` & `astroquery-0.4.dev5750/astroquery/gaia/tests/test_gaiatap.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/gama/core.py` & `astroquery-0.4.dev5750/astroquery/gama/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/gama/tests/data/GAMA_HzVs28.fits` & `astroquery-0.4.dev5750/astroquery/gama/tests/data/GAMA_HzVs28.fits`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/gama/tests/data/query_result.html` & `astroquery-0.4.dev5750/astroquery/gama/tests/data/query_result.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/gama/tests/test_gama.py` & `astroquery-0.4.dev5750/astroquery/gama/tests/test_gama.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/gama/tests/test_gama_remote.py` & `astroquery-0.4.dev5750/astroquery/gama/tests/test_gama_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/heasarc/__init__.py` & `astroquery-0.4.dev5750/astroquery/heasarc/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/heasarc/core.py` & `astroquery-0.4.dev5750/astroquery/heasarc/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/heasarc/tests/test_heasarc_remote.py` & `astroquery-0.4.dev5750/astroquery/heasarc/tests/test_heasarc_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/hitran/__init__.py` & `astroquery-0.4.dev5750/astroquery/hitran/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/hitran/core.py` & `astroquery-0.4.dev5750/astroquery/hitran/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/hitran/data/readme.txt` & `astroquery-0.4.dev5750/astroquery/hitran/data/readme.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/hitran/tests/data/H2O.data` & `astroquery-0.4.dev5750/astroquery/hitran/tests/data/H2O.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/hitran/tests/test_hitran.py` & `astroquery-0.4.dev5750/astroquery/hitran/tests/test_hitran.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/hitran/tests/test_hitran_remote.py` & `astroquery-0.4.dev5750/astroquery/hitran/tests/test_hitran_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/hitran/utils.py` & `astroquery-0.4.dev5750/astroquery/hitran/utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ibe/__init__.py` & `astroquery-0.4.dev5750/astroquery/ibe/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ibe/core.py` & `astroquery-0.4.dev5750/astroquery/ibe/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ibe/tests/data/columns.txt` & `astroquery-0.4.dev5750/astroquery/ibe/tests/data/columns.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ibe/tests/data/datasets.html` & `astroquery-0.4.dev5750/astroquery/ibe/tests/data/datasets.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ibe/tests/data/field_id.txt` & `astroquery-0.4.dev5750/astroquery/ibe/tests/data/field_id.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ibe/tests/data/missions.html` & `astroquery-0.4.dev5750/astroquery/ibe/tests/data/missions.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ibe/tests/data/pos.txt` & `astroquery-0.4.dev5750/astroquery/ibe/tests/data/pos.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ibe/tests/data/tables.html` & `astroquery-0.4.dev5750/astroquery/ibe/tests/data/tables.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ibe/tests/test_ibe.py` & `astroquery-0.4.dev5750/astroquery/ibe/tests/test_ibe.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ibe/tests/test_ibe_remote.py` & `astroquery-0.4.dev5750/astroquery/ibe/tests/test_ibe_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/__init__.py` & `astroquery-0.4.dev5750/astroquery/imcce/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/core.py` & `astroquery-0.4.dev5750/astroquery/imcce/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype1.dat` & `astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype1.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype2.dat` & `astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype2.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype3.dat` & `astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype3.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype4.dat` & `astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype4.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype5.dat` & `astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype5.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/data/3552_coordtype6.dat` & `astroquery-0.4.dev5750/astroquery/imcce/tests/data/3552_coordtype6.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/data/skybot_query.dat` & `astroquery-0.4.dev5750/astroquery/imcce/tests/data/skybot_query.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/test_miriade.py` & `astroquery-0.4.dev5750/astroquery/imcce/tests/test_miriade.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/test_miriade_remote.py` & `astroquery-0.4.dev5750/astroquery/imcce/tests/test_miriade_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/test_skybot.py` & `astroquery-0.4.dev5750/astroquery/imcce/tests/test_skybot.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/imcce/tests/test_skybot_remote.py` & `astroquery-0.4.dev5750/astroquery/imcce/tests/test_skybot_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa/__init__.py` & `astroquery-0.4.dev5750/astroquery/irsa/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa/core.py` & `astroquery-0.4.dev5750/astroquery/irsa/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa/tests/data/Box.xml` & `astroquery-0.4.dev5750/astroquery/irsa/tests/data/Box.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa/tests/data/Cone.xml` & `astroquery-0.4.dev5750/astroquery/irsa/tests/data/Cone.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa/tests/data/Cone_coord.xml` & `astroquery-0.4.dev5750/astroquery/irsa/tests/data/Cone_coord.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa/tests/data/Polygon.xml` & `astroquery-0.4.dev5750/astroquery/irsa/tests/data/Polygon.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa/tests/test_irsa.py` & `astroquery-0.4.dev5750/astroquery/irsa/tests/test_irsa.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa/tests/test_irsa_remote.py` & `astroquery-0.4.dev5750/astroquery/irsa/tests/test_irsa_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa_dust/__init__.py` & `astroquery-0.4.dev5750/astroquery/irsa_dust/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa_dust/core.py` & `astroquery-0.4.dev5750/astroquery/irsa_dust/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/dust_ext_detail.tbl` & `astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/dust_ext_detail.tbl`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/dustm101.xml` & `astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/dustm101.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/dustm31.xml` & `astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/dustm31.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/dustm81.xml` & `astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/dustm81.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa_dust/tests/data/test.fits` & `astroquery-0.4.dev5750/astroquery/irsa_dust/tests/data/test.fits`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa_dust/tests/test_irsa_dust.py` & `astroquery-0.4.dev5750/astroquery/irsa_dust/tests/test_irsa_dust.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa_dust/tests/test_irsa_dust_remote.py` & `astroquery-0.4.dev5750/astroquery/irsa_dust/tests/test_irsa_dust_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/irsa_dust/utils.py` & `astroquery-0.4.dev5750/astroquery/irsa_dust/utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplhorizons/__init__.py` & `astroquery-0.4.dev5750/astroquery/jplhorizons/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplhorizons/core.py` & `astroquery-0.4.dev5750/astroquery/jplhorizons/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplhorizons/tests/data/ceres_elements.txt` & `astroquery-0.4.dev5750/astroquery/jplhorizons/tests/data/ceres_elements.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplhorizons/tests/data/ceres_ephemerides.txt` & `astroquery-0.4.dev5750/astroquery/jplhorizons/tests/data/ceres_ephemerides.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplhorizons/tests/data/ceres_vectors.txt` & `astroquery-0.4.dev5750/astroquery/jplhorizons/tests/data/ceres_vectors.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplhorizons/tests/data/no_H.txt` & `astroquery-0.4.dev5750/astroquery/jplhorizons/tests/data/no_H.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplhorizons/tests/test_jplhorizons.py` & `astroquery-0.4.dev5750/astroquery/jplhorizons/tests/test_jplhorizons.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplhorizons/tests/test_jplhorizons_remote.py` & `astroquery-0.4.dev5750/astroquery/jplhorizons/tests/test_jplhorizons_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplsbdb/__init__.py` & `astroquery-0.4.dev5750/astroquery/jplsbdb/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplsbdb/core.py` & `astroquery-0.4.dev5750/astroquery/jplsbdb/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/67P.dat` & `astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/67P.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/apophis.dat` & `astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/apophis.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/ceres.dat` & `astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/ceres.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/ceres_missing_value.dat` & `astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/ceres_missing_value.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplsbdb/tests/data/phaethon.dat` & `astroquery-0.4.dev5750/astroquery/jplsbdb/tests/data/phaethon.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplsbdb/tests/test_jplsbdb.py` & `astroquery-0.4.dev5750/astroquery/jplsbdb/tests/test_jplsbdb.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplsbdb/tests/test_jplsbdb_remote.py` & `astroquery-0.4.dev5750/astroquery/jplsbdb/tests/test_jplsbdb_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplspec/__init__.py` & `astroquery-0.4.dev5750/astroquery/jplspec/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplspec/core.py` & `astroquery-0.4.dev5750/astroquery/jplspec/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplspec/data/catdir.cat` & `astroquery-0.4.dev5750/astroquery/jplspec/data/catdir.cat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplspec/lookup_table.py` & `astroquery-0.4.dev5750/astroquery/jplspec/lookup_table.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplspec/tests/data/CO.data` & `astroquery-0.4.dev5750/astroquery/jplspec/tests/data/CO.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplspec/tests/data/CO_6.data` & `astroquery-0.4.dev5750/astroquery/jplspec/tests/data/CO_6.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplspec/tests/data/multi.data` & `astroquery-0.4.dev5750/astroquery/jplspec/tests/data/multi.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplspec/tests/test_jplspec.py` & `astroquery-0.4.dev5750/astroquery/jplspec/tests/test_jplspec.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/jplspec/tests/test_jplspec_remote.py` & `astroquery-0.4.dev5750/astroquery/jplspec/tests/test_jplspec_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lamda/__init__.py` & `astroquery-0.4.dev5750/astroquery/lamda/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lamda/core.py` & `astroquery-0.4.dev5750/astroquery/lamda/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lamda/tests/data/co.txt` & `astroquery-0.4.dev5750/astroquery/lamda/tests/data/co.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lamda/tests/test_lamda.py` & `astroquery-0.4.dev5750/astroquery/lamda/tests/test_lamda.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lamda/utils.py` & `astroquery-0.4.dev5750/astroquery/lamda/utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lcogt/__init__.py` & `astroquery-0.4.dev5750/astroquery/lcogt/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lcogt/core.py` & `astroquery-0.4.dev5750/astroquery/lcogt/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lcogt/tests/data/Box.xml` & `astroquery-0.4.dev5750/astroquery/lcogt/tests/data/Box.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lcogt/tests/data/Cone.xml` & `astroquery-0.4.dev5750/astroquery/lcogt/tests/data/Cone.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lcogt/tests/data/Cone_coord.xml` & `astroquery-0.4.dev5750/astroquery/lcogt/tests/data/Cone_coord.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lcogt/tests/data/Polygon.xml` & `astroquery-0.4.dev5750/astroquery/lcogt/tests/data/Polygon.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lcogt/tests/test_lcogt.py` & `astroquery-0.4.dev5750/astroquery/lcogt/tests/test_lcogt.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/lcogt/tests/test_lcogt_remote.py` & `astroquery-0.4.dev5750/astroquery/lcogt/tests/test_lcogt_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/magpis/__init__.py` & `astroquery-0.4.dev5750/astroquery/magpis/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/magpis/core.py` & `astroquery-0.4.dev5750/astroquery/magpis/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/magpis/tests/data/image.fits` & `astroquery-0.4.dev5750/astroquery/magpis/tests/data/image.fits`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/magpis/tests/test_magpis.py` & `astroquery-0.4.dev5750/astroquery/magpis/tests/test_magpis.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/magpis/tests/test_magpis_remote.py` & `astroquery-0.4.dev5750/astroquery/magpis/tests/test_magpis_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/__init__.py` & `astroquery-0.4.dev5750/astroquery/mast/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/core.py` & `astroquery-0.4.dev5750/astroquery/mast/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/fpl.py` & `astroquery-0.4.dev5750/astroquery/mast/fpl.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tesscut.py` & `astroquery-0.4.dev5750/astroquery/mast/tesscut.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/advSearch.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/advSearch.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/advSearchPos.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/advSearchPos.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/astrocut_107.27_-70.0_5x5.zip` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/astrocut_107.27_-70.0_5x5.zip`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/bundleResponse.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/bundleResponse.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/caom.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/caom.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/columnsconfig.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/columnsconfig.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/dd.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/dd.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/ddcolumns.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/ddcolumns.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/ddcolumns_filtered.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/ddcolumns_filtered.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/hsc.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/hsc.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/matchid.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/matchid.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/missions.extjs` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/missions.extjs`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/panstarrs.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/panstarrs.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/products.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/products.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/spectra.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/spectra.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/tic.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/tic.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/ticcolumns.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/ticcolumns.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/data/ticcolumns_filtered.json` & `astroquery-0.4.dev5750/astroquery/mast/tests/data/ticcolumns_filtered.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/test_mast.py` & `astroquery-0.4.dev5750/astroquery/mast/tests/test_mast.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mast/tests/test_mast_remote.py` & `astroquery-0.4.dev5750/astroquery/mast/tests/test_mast_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/__init__.py` & `astroquery-0.4.dev5750/astroquery/mpc/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/core.py` & `astroquery-0.4.dev5750/astroquery/mpc/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/data/1994XG_ephemeris_500-a-t.html` & `astroquery-0.4.dev5750/astroquery/mpc/tests/data/1994XG_ephemeris_500-a-t.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/data/1994XG_ephemeris_G37-a-t.html` & `astroquery-0.4.dev5750/astroquery/mpc/tests/data/1994XG_ephemeris_G37-a-t.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_500-G-t.html` & `astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_500-G-t.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_500-a-c.html` & `astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_500-a-c.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_500-a-s.html` & `astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_500-a-s.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_500-a-t.html` & `astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_500-a-t.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_500-s-t.html` & `astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_500-s-t.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/data/2P_ephemeris_G37-a-t.html` & `astroquery-0.4.dev5750/astroquery/mpc/tests/data/2P_ephemeris_G37-a-t.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/data/ObsCodes.html` & `astroquery-0.4.dev5750/astroquery/mpc/tests/data/ObsCodes.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/data/mpc_obs.dat` & `astroquery-0.4.dev5750/astroquery/mpc/tests/data/mpc_obs.dat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/test_mpc.py` & `astroquery-0.4.dev5750/astroquery/mpc/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/mpc/tests/test_mpc_remote.py` & `astroquery-0.4.dev5750/astroquery/mpc/tests/test_mpc_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nasa_ads/__init__.py` & `astroquery-0.4.dev5750/astroquery/nasa_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nasa_ads/core.py` & `astroquery-0.4.dev5750/astroquery/nasa_ads/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nasa_ads/tests/data/test_text.txt` & `astroquery-0.4.dev5750/astroquery/nasa_ads/tests/data/test_text.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nasa_ads/tests/test_nasaads.py` & `astroquery-0.4.dev5750/astroquery/nasa_ads/tests/test_nasaads.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/__init__.py` & `astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/data/exoplanet_nexsci_units.json` & `astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/data/exoplanet_nexsci_units.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/nasa_exoplanet_archive.py` & `astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/nasa_exoplanet_archive.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/tests/data/nasa_exoplanet_archive.csv` & `astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/tests/data/nasa_exoplanet_archive.csv`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nasa_exoplanet_archive/tests/test_nasa_exoplanet_archive_remote.py` & `astroquery-0.4.dev5750/astroquery/nasa_exoplanet_archive/tests/test_nasa_exoplanet_archive_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/__init__.py` & `astroquery-0.4.dev5750/astroquery/ned/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/core.py` & `astroquery-0.4.dev5750/astroquery/ned/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/data/keywords_dict.json` & `astroquery-0.4.dev5750/astroquery/ned/data/keywords_dict.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/error.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/error.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/image_extract.html` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/image_extract.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_diameters.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_diameters.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_iau_format.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_iau_format.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_images.fits` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_images.fits`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_near_name.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_near_name.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_near_position.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_near_position.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_notes.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_notes.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_object.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_object.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_photometry.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_photometry.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_positions.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_positions.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_redshifts.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_redshifts.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_refcode.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_refcode.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/data/query_references.xml` & `astroquery-0.4.dev5750/astroquery/ned/tests/data/query_references.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/test_ned.py` & `astroquery-0.4.dev5750/astroquery/ned/tests/test_ned.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ned/tests/test_ned_remote.py` & `astroquery-0.4.dev5750/astroquery/ned/tests/test_ned_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nist/__init__.py` & `astroquery-0.4.dev5750/astroquery/nist/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nist/core.py` & `astroquery-0.4.dev5750/astroquery/nist/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nist/tests/data/nist_out.html` & `astroquery-0.4.dev5750/astroquery/nist/tests/data/nist_out.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nist/tests/test_nist.py` & `astroquery-0.4.dev5750/astroquery/nist/tests/test_nist.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nist/tests/test_nist_remote.py` & `astroquery-0.4.dev5750/astroquery/nist/tests/test_nist_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nrao/__init__.py` & `astroquery-0.4.dev5750/astroquery/nrao/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nrao/core.py` & `astroquery-0.4.dev5750/astroquery/nrao/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nrao/tests/data/archive_html.html` & `astroquery-0.4.dev5750/astroquery/nrao/tests/data/archive_html.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nrao/tests/data/votable.xml` & `astroquery-0.4.dev5750/astroquery/nrao/tests/data/votable.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nrao/tests/test_nrao.py` & `astroquery-0.4.dev5750/astroquery/nrao/tests/test_nrao.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nrao/tests/test_nrao_remote.py` & `astroquery-0.4.dev5750/astroquery/nrao/tests/test_nrao_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nvas/__init__.py` & `astroquery-0.4.dev5750/astroquery/nvas/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nvas/core.py` & `astroquery-0.4.dev5750/astroquery/nvas/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nvas/tests/data/image.imfits` & `astroquery-0.4.dev5750/astroquery/nvas/tests/data/image.imfits`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nvas/tests/data/image_results.html` & `astroquery-0.4.dev5750/astroquery/nvas/tests/data/image_results.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nvas/tests/test_nvas.py` & `astroquery-0.4.dev5750/astroquery/nvas/tests/test_nvas.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/nvas/tests/test_nvas_remote.py` & `astroquery-0.4.dev5750/astroquery/nvas/tests/test_nvas_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/oac/__init__.py` & `astroquery-0.4.dev5750/astroquery/oac/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/oac/core.py` & `astroquery-0.4.dev5750/astroquery/oac/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/oac/tests/data/photometry_csv.txt` & `astroquery-0.4.dev5750/astroquery/oac/tests/data/photometry_csv.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/oac/tests/data/photometry_json.txt` & `astroquery-0.4.dev5750/astroquery/oac/tests/data/photometry_json.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/oac/tests/data/single_spectrum_csv.txt` & `astroquery-0.4.dev5750/astroquery/oac/tests/data/single_spectrum_csv.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/oac/tests/data/spectra_json.txt` & `astroquery-0.4.dev5750/astroquery/oac/tests/data/spectra_json.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/oac/tests/test_oac.py` & `astroquery-0.4.dev5750/astroquery/oac/tests/test_oac.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/oac/tests/test_oac_remote.py` & `astroquery-0.4.dev5750/astroquery/oac/tests/test_oac_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ogle/__init__.py` & `astroquery-0.4.dev5750/astroquery/ogle/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ogle/core.py` & `astroquery-0.4.dev5750/astroquery/ogle/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ogle/tests/test_ogle.py` & `astroquery-0.4.dev5750/astroquery/ogle/tests/test_ogle.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/oec_query.py` & `astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/oec_query.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/tests/data/systems.xml.gz` & `astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/tests/data/systems.xml.gz`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/tests/test_open_exoplanet_catalogue_local.py` & `astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/tests/test_open_exoplanet_catalogue_local.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/open_exoplanet_catalogue/utils.py` & `astroquery-0.4.dev5750/astroquery/open_exoplanet_catalogue/utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/query.py` & `astroquery-0.4.dev5750/astroquery/query.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sdss/__init__.py` & `astroquery-0.4.dev5750/astroquery/sdss/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sdss/core.py` & `astroquery-0.4.dev5750/astroquery/sdss/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sdss/data/PhotoObjAll_dr12.json` & `astroquery-0.4.dev5750/astroquery/sdss/data/PhotoObjAll_dr12.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sdss/data/SpecObjAll_dr12.json` & `astroquery-0.4.dev5750/astroquery/sdss/data/SpecObjAll_dr12.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sdss/field_names.py` & `astroquery-0.4.dev5750/astroquery/sdss/field_names.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sdss/tests/data/emptyfile.fits` & `astroquery-0.4.dev5750/astroquery/sdss/tests/data/emptyfile.fits`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sdss/tests/data/xid_im.txt` & `astroquery-0.4.dev5750/astroquery/sdss/tests/data/xid_im.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sdss/tests/test_sdss.py` & `astroquery-0.4.dev5750/astroquery/sdss/tests/test_sdss.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sdss/tests/test_sdss_remote.py` & `astroquery-0.4.dev5750/astroquery/sdss/tests/test_sdss_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sha/core.py` & `astroquery-0.4.dev5750/astroquery/sha/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sha/tests/data/img.fits` & `astroquery-0.4.dev5750/astroquery/sha/tests/data/img.fits`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sha/tests/data/nid_t.txt` & `astroquery-0.4.dev5750/astroquery/sha/tests/data/nid_t.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sha/tests/data/pid_t.txt` & `astroquery-0.4.dev5750/astroquery/sha/tests/data/pid_t.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sha/tests/data/pos_t.txt` & `astroquery-0.4.dev5750/astroquery/sha/tests/data/pos_t.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sha/tests/data/rqk_t.txt` & `astroquery-0.4.dev5750/astroquery/sha/tests/data/rqk_t.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/sha/tests/test_sha.py` & `astroquery-0.4.dev5750/astroquery/sha/tests/test_sha.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/__init__.py` & `astroquery-0.4.dev5750/astroquery/simbad/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/core.py` & `astroquery-0.4.dev5750/astroquery/simbad/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/data/votable_fields_dict.json` & `astroquery-0.4.dev5750/astroquery/simbad/data/votable_fields_dict.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/get_votable_fields.py` & `astroquery-0.4.dev5750/astroquery/simbad/get_votable_fields.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/setup_package.py` & `astroquery-0.4.dev5750/astroquery/simbad/setup_package.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/data/m1.data` & `astroquery-0.4.dev5750/astroquery/simbad/tests/data/m1.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_bibcode.data` & `astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_bibcode.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_bibobj.data` & `astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_bibobj.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_cat.data` & `astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_cat.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_coo.data` & `astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_coo.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_error.data` & `astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_error.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_id.data` & `astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_id.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_objectids.data` & `astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_objectids.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_sample.data` & `astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_sample.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/data/query_sample_region.data` & `astroquery-0.4.dev5750/astroquery/simbad/tests/data/query_sample_region.data`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/test_simbad.py` & `astroquery-0.4.dev5750/astroquery/simbad/tests/test_simbad.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/simbad/tests/test_simbad_remote.py` & `astroquery-0.4.dev5750/astroquery/simbad/tests/test_simbad_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/skyview/core.py` & `astroquery-0.4.dev5750/astroquery/skyview/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/skyview/tests/data/query_page.html` & `astroquery-0.4.dev5750/astroquery/skyview/tests/data/query_page.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/skyview/tests/data/results.html` & `astroquery-0.4.dev5750/astroquery/skyview/tests/data/results.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/skyview/tests/data/survey_dict.json` & `astroquery-0.4.dev5750/astroquery/skyview/tests/data/survey_dict.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/skyview/tests/test_skyview.py` & `astroquery-0.4.dev5750/astroquery/skyview/tests/test_skyview.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/skyview/tests/test_skyview_remote.py` & `astroquery-0.4.dev5750/astroquery/skyview/tests/test_skyview_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/splatalogue/__init__.py` & `astroquery-0.4.dev5750/astroquery/splatalogue/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/splatalogue/build_species_table.py` & `astroquery-0.4.dev5750/astroquery/splatalogue/build_species_table.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/splatalogue/core.py` & `astroquery-0.4.dev5750/astroquery/splatalogue/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/splatalogue/data/species.json` & `astroquery-0.4.dev5750/astroquery/splatalogue/data/species.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/splatalogue/load_species_table.py` & `astroquery-0.4.dev5750/astroquery/splatalogue/load_species_table.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/splatalogue/slap.py` & `astroquery-0.4.dev5750/astroquery/splatalogue/slap.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/splatalogue/tests/data/CO_colons.csv` & `astroquery-0.4.dev5750/astroquery/splatalogue/tests/data/CO_colons.csv`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/splatalogue/tests/test_splatalogue.py` & `astroquery-0.4.dev5750/astroquery/splatalogue/tests/test_splatalogue.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/splatalogue/tests/test_utils.py` & `astroquery-0.4.dev5750/astroquery/splatalogue/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/splatalogue/utils.py` & `astroquery-0.4.dev5750/astroquery/splatalogue/utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/template_module/__init__.py` & `astroquery-0.4.dev5750/astroquery/template_module/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/template_module/core.py` & `astroquery-0.4.dev5750/astroquery/template_module/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/template_module/tests/setup_package.py` & `astroquery-0.4.dev5750/astroquery/template_module/tests/setup_package.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/template_module/tests/test_module.py` & `astroquery-0.4.dev5750/astroquery/template_module/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/tests/coveragerc` & `astroquery-0.4.dev5750/astroquery/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/tests/test_resume.py` & `astroquery-0.4.dev5750/astroquery/tests/test_resume.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ukidss/__init__.py` & `astroquery-0.4.dev5750/astroquery/ukidss/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ukidss/core.py` & `astroquery-0.4.dev5750/astroquery/ukidss/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ukidss/tests/data/error.html` & `astroquery-0.4.dev5750/astroquery/ukidss/tests/data/error.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ukidss/tests/data/image.fits` & `astroquery-0.4.dev5750/astroquery/ukidss/tests/data/image.fits`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ukidss/tests/data/image_results.html` & `astroquery-0.4.dev5750/astroquery/ukidss/tests/data/image_results.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ukidss/tests/data/vo_results.html` & `astroquery-0.4.dev5750/astroquery/ukidss/tests/data/vo_results.html`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ukidss/tests/data/votable.xml` & `astroquery-0.4.dev5750/astroquery/ukidss/tests/data/votable.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ukidss/tests/test_ukidss.py` & `astroquery-0.4.dev5750/astroquery/ukidss/tests/test_ukidss.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/ukidss/tests/test_ukidss_remote.py` & `astroquery-0.4.dev5750/astroquery/ukidss/tests/test_ukidss_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/class_or_instance.py` & `astroquery-0.4.dev5750/astroquery/utils/class_or_instance.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/commons.py` & `astroquery-0.4.dev5750/astroquery/utils/commons.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/decorators.py` & `astroquery-0.4.dev5750/astroquery/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/docstr_chompers.py` & `astroquery-0.4.dev5750/astroquery/utils/docstr_chompers.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/download_file_list.py` & `astroquery-0.4.dev5750/astroquery/utils/download_file_list.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/process_asyncs.py` & `astroquery-0.4.dev5750/astroquery/utils/process_asyncs.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/progressbar.py` & `astroquery-0.4.dev5750/astroquery/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/schema.py` & `astroquery-0.4.dev5750/astroquery/utils/schema.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/system_tools.py` & `astroquery-0.4.dev5750/astroquery/utils/system_tools.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/__init__.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/conn/tapconn.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/conn/tapconn.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/DummyConn.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/DummyConn.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/DummyConnHandler.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/DummyConnHandler.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/DummyResponse.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/DummyResponse.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/conn/tests/test_conn.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/conn/tests/test_conn.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/core.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/gui/login.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/gui/login.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/filter.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/filter.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/group.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/group.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/job.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/job.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/modelutils.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/modelutils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/shared_item.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/shared_item.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/shared_to_item.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/shared_to_item.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/tapcolumn.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/tapcolumn.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/taptable.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/taptable.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/tests/data/result_1.vot` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/tests/data/result_1.vot`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/tests/test_job.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/model/user.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/model/user.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/taputils.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/taputils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/tests/data/job_1.vot` & `astroquery-0.4.dev5750/astroquery/utils/tap/tests/data/job_1.vot`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/tests/data/jobs_list.xml` & `astroquery-0.4.dev5750/astroquery/utils/tap/tests/data/jobs_list.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/tests/data/test_table1.xml` & `astroquery-0.4.dev5750/astroquery/utils/tap/tests/data/test_table1.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/tests/data/test_tables.xml` & `astroquery-0.4.dev5750/astroquery/utils/tap/tests/data/test_tables.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/tests/setup_package.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/tests/setup_package.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/tests/test_tap.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/tests/test_tap.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/groupSaxParser.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/groupSaxParser.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/jobListSaxParser.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/jobListSaxParser.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/jobSaxParser.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/jobSaxParser.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/sharedItemsSaxParser.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/sharedItemsSaxParser.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tableSaxParser.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tableSaxParser.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/data/test_job_results.xml` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/data/test_job_results.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/data/test_jobs_async.xml` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/data/test_jobs_async.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/data/test_jobs_list.xml` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/data/test_jobs_list.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/data/test_tables.xml` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/data/test_tables.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/setup_package.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/setup_package.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/tests/test_xmlparser.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/tests/test_xmlparser.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tap/xmlparser/utils.py` & `astroquery-0.4.dev5750/astroquery/utils/tap/xmlparser/utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/testing_tools.py` & `astroquery-0.4.dev5750/astroquery/utils/testing_tools.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/tests/test_utils.py` & `astroquery-0.4.dev5750/astroquery/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/utils/url_helpers.py` & `astroquery-0.4.dev5750/astroquery/utils/url_helpers.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vamdc/__init__.py` & `astroquery-0.4.dev5750/astroquery/vamdc/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vamdc/core.py` & `astroquery-0.4.dev5750/astroquery/vamdc/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vamdc/load_species_table.py` & `astroquery-0.4.dev5750/astroquery/vamdc/load_species_table.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vamdc/tests/test_vamdc.py` & `astroquery-0.4.dev5750/astroquery/vamdc/tests/test_vamdc.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vamdc/tests/test_vamdc_remote.py` & `astroquery-0.4.dev5750/astroquery/vamdc/tests/test_vamdc_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/version.py` & `astroquery-0.4.dev5750/astroquery/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Autogenerated by Astropy-affiliated package astroquery's setup.py on 2019-10-08 20:45:31 UTC
+# Autogenerated by Astropy-affiliated package astroquery's setup.py on 2019-10-10 04:47:57 UTC
 from __future__ import unicode_literals
 import datetime
 
 
 import locale
 import os
 import subprocess
@@ -183,16 +183,16 @@
 
         current_dir = os.path.dirname(current_dir)
 
     return None
 
 
 _packagename = "astroquery"
-_last_generated_version = "0.4.dev5744"
-_last_githash = "a733169f06cf4530b24ce2005001fd5299616e0e"
+_last_generated_version = "0.4.dev5750"
+_last_githash = "e7d94e01aa6cde786a8e21bb481835a9993ac0d4"
 
 # Determine where the source code for this module
 # lives.  If __file__ is not a filesystem path then
 # it is assumed not to live in a git repo at all.
 if _get_repo_path(__file__, levels=len(_packagename.split('.'))):
     version = update_git_devstr(_last_generated_version, path=__file__)
     githash = get_git_devstr(sha=True, show_warning=False,
@@ -205,15 +205,15 @@
 
 
 major = 0
 minor = 4
 bugfix = 0
 
 release = False
-timestamp = datetime.datetime(2019, 10, 8, 20, 45, 31)
+timestamp = datetime.datetime(2019, 10, 10, 4, 47, 57)
 debug = False
 
 astropy_helpers_version = "2.0.10"
 
 try:
     from ._compiler import compiler
 except ImportError:
```

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/__init__.py` & `astroquery-0.4.dev5750/astroquery/vizier/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/core.py` & `astroquery-0.4.dev5750/astroquery/vizier/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/data/inverse_dict.json` & `astroquery-0.4.dev5750/astroquery/vizier/data/inverse_dict.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/data/keywords_dict.json` & `astroquery-0.4.dev5750/astroquery/vizier/data/keywords_dict.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/setup_package.py` & `astroquery-0.4.dev5750/astroquery/vizier/setup_package.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/tests/data/afgl2591_iram.xml` & `astroquery-0.4.dev5750/astroquery/vizier/tests/data/afgl2591_iram.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/tests/data/find_kangapj70683.xml` & `astroquery-0.4.dev5750/astroquery/vizier/tests/data/find_kangapj70683.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/tests/data/kang2010.xml` & `astroquery-0.4.dev5750/astroquery/vizier/tests/data/kang2010.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/tests/data/viz.xml` & `astroquery-0.4.dev5750/astroquery/vizier/tests/data/viz.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/tests/test_vizier.py` & `astroquery-0.4.dev5750/astroquery/vizier/tests/test_vizier.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vizier/tests/test_vizier_remote.py` & `astroquery-0.4.dev5750/astroquery/vizier/tests/test_vizier_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/__init__.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/conesearch.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/conesearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 # THIRD-PARTY
 import numpy as np
 
 # ASTROPY
 from astropy.io.votable.exceptions import vo_warn, W25
 from astropy.utils.console import color_print
-from astropy.utils.timer import timefunc, RunTimePredictor
 from astropy.utils.exceptions import AstropyUserWarning
 
 # LOCAL
 from . import vos_catalog
 from .vo_async import AsyncBase
 from .core import ConeSearchClass, _validate_sr
 from .exceptions import ConeSearchError, VOSError
+from ..utils.timer import timefunc, RunTimePredictor
 
 # Import configurable items declared in __init__.py
 from . import conf
 
 __all__ = ['AsyncConeSearch', 'conesearch', 'AsyncSearchAll', 'search_all',
            'list_catalogs', 'predict_search', 'conesearch_timer']
 
@@ -371,15 +371,15 @@
 
 def predict_search(url, *args, **kwargs):
     """
     Predict the run time needed and the number of objects
     for a Cone Search for the given access URL, position, and
     radius.
 
-    Run time prediction uses `astropy.utils.timer.RunTimePredictor`.
+    Run time prediction uses `astroquery.utils.timer.RunTimePredictor`.
     Baseline searches are done with starting and ending radii at
     0.05 and 0.5 of the given radius, respectively.
 
     Extrapolation on good data uses least-square straight line fitting,
     assuming linear increase of search time and number of objects
     with radius, which might not be accurate for some cases. If
     there are less than 3 data points in the fit, it fails.
@@ -504,15 +504,15 @@
 
     return t_est, n_est
 
 
 @timefunc(1)
 def conesearch_timer(*args, **kwargs):
     """
-    Time a single Cone Search using `astropy.utils.timer.timefunc`
+    Time a single Cone Search using `astroquery.utils.timer.timefunc`
     with a single try and a verbose timer.
 
     Parameters
     ----------
     args, kwargs
         See :func:`conesearch`.
```

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/core.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/exceptions.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/test_conesearch.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/test_conesearch.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/tests/test_vos_catalog.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/tests/test_vos_catalog.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/__init__.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/data/conesearch_urls.txt` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/data/conesearch_urls.txt`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/exceptions.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/inspect.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/inspect.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/conesearch_good.json` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/conesearch_good.json`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/printcat.out` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/printcat.out`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/data/vao_conesearch_sites_121107_subset.xml` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/data/vao_conesearch_sites_121107_subset.xml`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/test_inpect.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/test_inpect.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tests/test_validate.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/tstquery.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/tstquery.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/validator/validate.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/validator/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 # ASTROPY
 from astropy.io import votable
 from astropy.io.votable.exceptions import E19
 from astropy.io.votable.validator import html, result
 from astropy.logger import log
 from astropy.utils import data
 from astropy.utils.exceptions import AstropyUserWarning
-from astropy.utils.timer import timefunc
 from astropy.utils.xml.unescaper import unescape_all
 
 # LOCAL
 from .tstquery import parse_cs
 from .exceptions import (ValidationMultiprocessingError,
                          InvalidValidationAttribute)
 from ..exceptions import VOSError
 from ..vos_catalog import VOSDatabase, vo_tab_parse
+from ...utils.timer import timefunc
 
 # Import configurable items declared in __init__.py
 from . import conf
 
 __all__ = ['check_conesearch_sites']
```

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/vo_async.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/vo_async.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vo_conesearch/vos_catalog.py` & `astroquery-0.4.dev5750/astroquery/vo_conesearch/vos_catalog.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vsa/__init__.py` & `astroquery-0.4.dev5750/astroquery/vsa/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vsa/core.py` & `astroquery-0.4.dev5750/astroquery/vsa/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/vsa/tests/test_vista_remote.py` & `astroquery-0.4.dev5750/astroquery/vsa/tests/test_vista_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/wfau/__init__.py` & `astroquery-0.4.dev5750/astroquery/wfau/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/wfau/core.py` & `astroquery-0.4.dev5750/astroquery/wfau/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/xmatch/__init__.py` & `astroquery-0.4.dev5750/astroquery/xmatch/__init__.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/xmatch/core.py` & `astroquery-0.4.dev5750/astroquery/xmatch/core.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/xmatch/tests/data/query_res.csv` & `astroquery-0.4.dev5750/astroquery/xmatch/tests/data/query_res.csv`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/xmatch/tests/data/tables.csv` & `astroquery-0.4.dev5750/astroquery/xmatch/tests/data/tables.csv`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/xmatch/tests/test_xmatch.py` & `astroquery-0.4.dev5750/astroquery/xmatch/tests/test_xmatch.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/astroquery/xmatch/tests/test_xmatch_remote.py` & `astroquery-0.4.dev5750/astroquery/xmatch/tests/test_xmatch_remote.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/Makefile` & `astroquery-0.4.dev5750/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/alfalfa/alfalfa.rst` & `astroquery-0.4.dev5750/docs/alfalfa/alfalfa.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/alma/alma.rst` & `astroquery-0.4.dev5750/docs/alma/alma.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/api.rst` & `astroquery-0.4.dev5750/docs/api.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/astrometry_net/astrometry_net.rst` & `astroquery-0.4.dev5750/docs/astrometry_net/astrometry_net.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/atomic/atomic.rst` & `astroquery-0.4.dev5750/docs/atomic/atomic.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/besancon/besancon.rst` & `astroquery-0.4.dev5750/docs/besancon/besancon.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/cadc/cadc.rst` & `astroquery-0.4.dev5750/docs/cadc/cadc.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/cds/HST_union.png` & `astroquery-0.4.dev5750/docs/cds/HST_union.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/cds/MOC_GALEXGR6_AIS_FUV.png` & `astroquery-0.4.dev5750/docs/cds/MOC_GALEXGR6_AIS_FUV.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/cds/cds.rst` & `astroquery-0.4.dev5750/docs/cds/cds.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/conf.py` & `astroquery-0.4.dev5750/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/cosmosim/cosmosim.rst` & `astroquery-0.4.dev5750/docs/cosmosim/cosmosim.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/demos/Astroquery_DotAstro_Demo.ipynb` & `astroquery-0.4.dev5750/docs/demos/Astroquery_DotAstro_Demo.ipynb`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/esa/hubble.rst` & `astroquery-0.4.dev5750/docs/esa/hubble.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/esasky/esasky.rst` & `astroquery-0.4.dev5750/docs/esasky/esasky.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/eso/eso.rst` & `astroquery-0.4.dev5750/docs/eso/eso.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/exoplanet_orbit_database/exoplanet_orbit_database.rst` & `astroquery-0.4.dev5750/docs/exoplanet_orbit_database/exoplanet_orbit_database.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/fermi/fermi.rst` & `astroquery-0.4.dev5750/docs/fermi/fermi.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gaia/gaia.rst` & `astroquery-0.4.dev5750/docs/gaia/gaia.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gallery-examples/example10_mast.py` & `astroquery-0.4.dev5750/docs/gallery-examples/example10_mast.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gallery-examples/example1_vizier.py` & `astroquery-0.4.dev5750/docs/gallery-examples/example1_vizier.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gallery-examples/example2_simbad.py` & `astroquery-0.4.dev5750/docs/gallery-examples/example2_simbad.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gallery-examples/example4_simbad.py` & `astroquery-0.4.dev5750/docs/gallery-examples/example4_simbad.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gallery-examples/example6_alma.py` & `astroquery-0.4.dev5750/docs/gallery-examples/example6_alma.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gallery-examples/example7_alma.py` & `astroquery-0.4.dev5750/docs/gallery-examples/example7_alma.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gallery-examples/example8_eso.py` & `astroquery-0.4.dev5750/docs/gallery-examples/example8_eso.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gallery-examples/example9_skyview_vizier.py` & `astroquery-0.4.dev5750/docs/gallery-examples/example9_skyview_vizier.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gallery.rst` & `astroquery-0.4.dev5750/docs/gallery.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/gama/gama.rst` & `astroquery-0.4.dev5750/docs/gama/gama.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/heasarc/heasarc.rst` & `astroquery-0.4.dev5750/docs/heasarc/heasarc.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/hitran/hitran.rst` & `astroquery-0.4.dev5750/docs/hitran/hitran.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/ibe/ibe.rst` & `astroquery-0.4.dev5750/docs/ibe/ibe.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/imcce/imcce.rst` & `astroquery-0.4.dev5750/docs/imcce/imcce.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/index.rst` & `astroquery-0.4.dev5750/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -60,19 +60,19 @@
     $ cd astroquery
     $ python setup.py install
 
 
 Requirements
 ------------
 
-Astroquery works with Python 2.7 and 3.5 or later.
+Astroquery works with Python 3.6 or later.
 
 The following packages are required for astroquery installation & use:
 
-* `numpy <http://www.numpy.org>`_ >= 1.12
+* `numpy <http://www.numpy.org>`_ >= 1.14
 * `astropy <http://www.astropy.org>`__ (>=2.0)
 * `requests <http://docs.python-requests.org/en/latest/>`_
 * `keyring <https://pypi.python.org/pypi/keyring>`_
 * `Beautiful Soup <https://www.crummy.com/software/BeautifulSoup/>`_
 * `html5lib <https://pypi.python.org/pypi/html5lib>`_
 * `six <http://pypi.python.org/pypi/six/>`_
```

### Comparing `astroquery-0.4.dev5744/docs/irsa/irsa.rst` & `astroquery-0.4.dev5750/docs/irsa/irsa.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/irsa/irsa_dust.rst` & `astroquery-0.4.dev5750/docs/irsa/irsa_dust.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/jplhorizons/jplhorizons.rst` & `astroquery-0.4.dev5750/docs/jplhorizons/jplhorizons.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/jplsbdb/jplsbdb.rst` & `astroquery-0.4.dev5750/docs/jplsbdb/jplsbdb.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/jplspec/images/docplot_curvefit.png` & `astroquery-0.4.dev5750/docs/jplspec/images/docplot_curvefit.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/jplspec/images/docplot_jplspec.png` & `astroquery-0.4.dev5750/docs/jplspec/images/docplot_jplspec.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/jplspec/jplspec.rst` & `astroquery-0.4.dev5750/docs/jplspec/jplspec.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/lamda/lamda.rst` & `astroquery-0.4.dev5750/docs/lamda/lamda.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/magpis/magpis.rst` & `astroquery-0.4.dev5750/docs/magpis/magpis.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/make.bat` & `astroquery-0.4.dev5750/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/make_doctests.py` & `astroquery-0.4.dev5750/docs/make_doctests.py`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/mast/mast.rst` & `astroquery-0.4.dev5750/docs/mast/mast.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/mpc/mpc.rst` & `astroquery-0.4.dev5750/docs/mpc/mpc.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/nasa_ads/nasa_ads.rst` & `astroquery-0.4.dev5750/docs/nasa_ads/nasa_ads.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/nasa_exoplanet_archive/nasa_exoplanet_archive.rst` & `astroquery-0.4.dev5750/docs/nasa_exoplanet_archive/nasa_exoplanet_archive.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/ned/ned.rst` & `astroquery-0.4.dev5750/docs/ned/ned.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/nist/nist.rst` & `astroquery-0.4.dev5750/docs/nist/nist.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/nrao/nrao.rst` & `astroquery-0.4.dev5750/docs/nrao/nrao.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/nvas/nvas.rst` & `astroquery-0.4.dev5750/docs/nvas/nvas.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/oac/oac.rst` & `astroquery-0.4.dev5750/docs/oac/oac.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/ogle/ogle.rst` & `astroquery-0.4.dev5750/docs/ogle/ogle.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/open_exoplanet_catalogue/open_exoplanet_catalogue.rst` & `astroquery-0.4.dev5750/docs/open_exoplanet_catalogue/open_exoplanet_catalogue.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/release_notice_v0.2.rst` & `astroquery-0.4.dev5750/docs/release_notice_v0.2.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/sdss/sdss.rst` & `astroquery-0.4.dev5750/docs/sdss/sdss.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/sha/sha.rst` & `astroquery-0.4.dev5750/docs/sha/sha.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/simbad/simbad.rst` & `astroquery-0.4.dev5750/docs/simbad/simbad.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/skyview/skyview.rst` & `astroquery-0.4.dev5750/docs/skyview/skyview.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/solarsystem/imcce/imcce.rst` & `astroquery-0.4.dev5750/docs/solarsystem/imcce/imcce.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/solarsystem/jpl/jpl.rst` & `astroquery-0.4.dev5750/docs/solarsystem/jpl/jpl.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/solarsystem/mpc/mpc.rst` & `astroquery-0.4.dev5750/docs/solarsystem/mpc/mpc.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/solarsystem/solarsystem.rst` & `astroquery-0.4.dev5750/docs/solarsystem/solarsystem.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/splatalogue/splatalogue.rst` & `astroquery-0.4.dev5750/docs/splatalogue/splatalogue.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/testing.rst` & `astroquery-0.4.dev5750/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/ukidss/ukidss.rst` & `astroquery-0.4.dev5750/docs/ukidss/ukidss.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/utils/tap.rst` & `astroquery-0.4.dev5750/docs/utils/tap.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vamdc/vamdc.rst` & `astroquery-0.4.dev5750/docs/vamdc/vamdc.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vizier/vizier.rst` & `astroquery-0.4.dev5750/docs/vizier/vizier.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vo_conesearch/client.rst` & `astroquery-0.4.dev5750/docs/vo_conesearch/client.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vo_conesearch/images/astroquery_vo_flowchart.png` & `astroquery-0.4.dev5750/docs/vo_conesearch/images/astroquery_vo_flowchart.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vo_conesearch/images/client_predict_search_n.png` & `astroquery-0.4.dev5750/docs/vo_conesearch/images/client_predict_search_n.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vo_conesearch/images/client_predict_search_t.png` & `astroquery-0.4.dev5750/docs/vo_conesearch/images/client_predict_search_t.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vo_conesearch/images/validator_html_1.png` & `astroquery-0.4.dev5750/docs/vo_conesearch/images/validator_html_1.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vo_conesearch/images/validator_html_2.png` & `astroquery-0.4.dev5750/docs/vo_conesearch/images/validator_html_2.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vo_conesearch/images/validator_html_3.png` & `astroquery-0.4.dev5750/docs/vo_conesearch/images/validator_html_3.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vo_conesearch/images/validator_html_4.png` & `astroquery-0.4.dev5750/docs/vo_conesearch/images/validator_html_4.png`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vo_conesearch/validator.rst` & `astroquery-0.4.dev5750/docs/vo_conesearch/validator.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vo_conesearch/vo_conesearch.rst` & `astroquery-0.4.dev5750/docs/vo_conesearch/vo_conesearch.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/vsa/vsa.rst` & `astroquery-0.4.dev5750/docs/vsa/vsa.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/docs/xmatch/xmatch.rst` & `astroquery-0.4.dev5750/docs/xmatch/xmatch.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/licenses/SCHEMA.rst` & `astroquery-0.4.dev5750/licenses/SCHEMA.rst`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/setup.cfg` & `astroquery-0.4.dev5750/setup.cfg`

 * *Files identical despite different names*

### Comparing `astroquery-0.4.dev5744/setup.py` & `astroquery-0.4.dev5750/setup.py`

 * *Files identical despite different names*

