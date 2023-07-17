# Comparing `tmp/invenio-github-1.0.0b1.tar.gz` & `tmp/invenio-github-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-github-1.0.0b1.tar", last modified: Mon Jul  3 13:23:32 2023, max compression
+gzip compressed data, was "dist/invenio-github-1.0.0b2.tar", last modified: Mon Jul 17 09:34:13 2023, max compression
```

## Comparing `invenio-github-1.0.0b1.tar` & `invenio-github-1.0.0b2.tar`

### file list

```diff
@@ -1,117 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/.lgtm
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1134 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4311 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/RELEASE-NOTES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/babel.ini
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10752 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21716 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/invenio_github/init.js
--rw-r--r--   0 runner    (1001) docker     (122)     3733 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/invenio_github/view.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/less/github/
--rw-r--r--   0 runner    (1001) docker     (122)     3013 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/less/github/github.scss
--rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3498 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     8658 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     4777 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/receivers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/helpers.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     3702 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (122)     5597 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
--rw-r--r--   0 runner    (1001) docker     (122)    10522 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/views/
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/views/badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/views/github.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4311 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2500 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8804 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    21853 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_invenio_github.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3608 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     3713 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/.lgtm
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4517 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/RELEASE-NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10752 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22856 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/assets/semantic-ui/js/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/assets/semantic-ui/js/invenio_github/index.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/helpers.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6503 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
+-rw-r--r--   0 runner    (1001) docker     (122)    15043 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/views/badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8193 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/views/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4517 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2356 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21853 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_invenio_github.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3693 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_webhook.py
```

### Comparing `invenio-github-1.0.0b1/.editorconfig` & `invenio-github-1.0.0b2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/.tx/config` & `invenio-github-1.0.0b2/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/AUTHORS.rst` & `invenio-github-1.0.0b2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/CHANGES.rst` & `invenio-github-1.0.0b2/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,20 @@
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
 Changes
 =======
 
+Version v1.0.0b2 (released 2023-07-17)
+
+- global: restrain extension behind feature flag
+- api: add record serialization
+- handlers: fix hooks serialization
+
 Version v1.0.0b1 (released 2023-07-03)
 
 - Initial beta release.
 
 Version v1.0.0a28 (released 2022-10-24)
 
 - Initial public release.
```

### Comparing `invenio-github-1.0.0b1/CONTRIBUTING.rst` & `invenio-github-1.0.0b2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/LICENSE` & `invenio-github-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/MANIFEST.in` & `invenio-github-1.0.0b2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/PKG-INFO` & `invenio-github-1.0.0b2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,20 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.0b2 (released 2023-07-17)
+        
+        - global: restrain extension behind feature flag
+        - api: add record serialization
+        - handlers: fix hooks serialization
+        
         Version v1.0.0b1 (released 2023-07-03)
         
         - Initial beta release.
         
         Version v1.0.0a28 (released 2022-10-24)
         
         - Initial public release.
```

### Comparing `invenio-github-1.0.0b1/README.rst` & `invenio-github-1.0.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/RELEASE-NOTES.rst` & `invenio-github-1.0.0b2/RELEASE-NOTES.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/babel.ini` & `invenio-github-1.0.0b2/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/Makefile` & `invenio-github-1.0.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/api.rst` & `invenio-github-1.0.0b2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/authors.rst` & `invenio-github-1.0.0b2/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/changes.rst` & `invenio-github-1.0.0b2/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/conf.py` & `invenio-github-1.0.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/contributing.rst` & `invenio-github-1.0.0b2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/index.rst` & `invenio-github-1.0.0b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/installation.rst` & `invenio-github-1.0.0b2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/license.rst` & `invenio-github-1.0.0b2/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/make.bat` & `invenio-github-1.0.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/docs/usage.rst` & `invenio-github-1.0.0b2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/__init__.py` & `invenio-github-1.0.0b2/invenio_github/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
 from .ext import InvenioGitHub
 
-__version__ = "1.0.0b1"
+__version__ = "1.0.0b2"
 
 __all__ = ("__version__", "InvenioGitHub")
```

### Comparing `invenio-github-1.0.0b1/invenio_github/api.py` & `invenio-github-1.0.0b2/invenio_github/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
 import json
 from contextlib import contextmanager
+from copy import deepcopy
 
 import github3
 import humanize
 import requests
 from flask import current_app
 from invenio_access.permissions import authenticated_user
 from invenio_access.utils import get_identity
@@ -38,23 +39,25 @@
 from invenio_oauthclient.handlers import token_getter
 from invenio_oauthclient.models import RemoteAccount, RemoteToken
 from invenio_oauthclient.proxies import current_oauthclient
 from sqlalchemy.orm.exc import NoResultFound
 from werkzeug.local import LocalProxy
 from werkzeug.utils import cached_property
 
+from invenio_github.models import Release, ReleaseStatus, Repository
+from invenio_github.proxies import current_github
+from invenio_github.tasks import sync_hooks as sync_hooks_task
+from invenio_github.utils import iso_utcnow, parse_timestamp, utcnow
+
 from .errors import (
     RemoteAccountDataNotSet,
     RemoteAccountNotFound,
     RepositoryAccessError,
     RepositoryNotFoundError,
 )
-from .models import ReleaseStatus, Repository
-from .tasks import sync_hooks as sync_hooks_task
-from .utils import iso_utcnow, parse_timestamp, utcnow
 
 
 def check_repo_access_permissions(repo, user_id, repo_id, repo_name):
     """Checks permissions from user on repo."""
     if repo and repo.user_id and repo.user_id != int(user_id):
         raise RepositoryAccessError(user=user_id, repo=repo_name, repo_id=repo_id)
 
@@ -69,18 +72,20 @@
     @cached_property
     def api(self):
         """Return an authenticated GitHub API."""
         return github3.login(token=self.access_token)
 
     @cached_property
     def access_token(self):
-        """Return OAuth access token."""
-        if self.user_id:
-            return RemoteToken.get(self.user_id, self.remote.consumer_key).access_token
-        return self.remote.get_request_token()[0]
+        """Return OAuth access token's value."""
+        token = RemoteToken.get(self.user_id, self.remote.consumer_key)
+        if not token:
+            # The token is not yet in DB, it is retrieved from the request session.
+            return self.remote.get_request_token()[0]
+        return token.access_token
 
     @property
     def session_token(self):
         """Return OAuth session token."""
         session_token = None
         if self.user_id is not None:
             session_token = token_getter(self.remote)
@@ -158,51 +163,49 @@
 
         .. note::
 
             Syncing happens from GitHub's direction only. This means that we
             consider the information on GitHub as valid, and we overwrite our
             own state based on this information.
         """
-        active_repos = {}
-        github_repos = {
-            repo.id: repo
-            for repo in self.api.repositories()
-            if repo.permissions["admin"]
-        }
-        for gh_repo_id, gh_repo in github_repos.items():
-            active_repos[gh_repo_id] = {
-                "id": gh_repo_id,
-                "full_name": gh_repo.full_name,
-                "description": gh_repo.description,
-                "default_branch": gh_repo.default_branch,
-            }
+        github_repos = {}
+        for repo in self.api.repositories():
+            if repo.permissions["admin"]:
+                github_repos[repo.id] = {
+                    "id": repo.id,
+                    "full_name": repo.full_name,
+                    "description": repo.description,
+                    "default_branch": repo.default_branch,
+                }
 
         if hooks:
-            self._sync_hooks(list(active_repos.keys()), asynchronous=async_hooks)
+            self._sync_hooks(list(github_repos.keys()), asynchronous=async_hooks)
 
         # Update changed names for repositories stored in DB
         db_repos = Repository.query.filter(
             Repository.user_id == self.user_id,
         )
 
         for repo in db_repos:
-            if gh_repo and repo.name != gh_repo.full_name:
-                repo.name = gh_repo.full_name
+            gh_repo = github_repos.get(repo.github_id)
+            if gh_repo and repo.name != gh_repo["full_name"]:
+                repo.name = gh_repo["full_name"]
                 db.session.add(repo)
 
         # Remove ownership from repositories that the user has no longer
         # 'admin' permissions, or have been deleted.
         Repository.query.filter(
             Repository.user_id == self.user_id,
+            ~Repository.github_id.in_(github_repos.keys()),
         ).update(dict(user_id=None, hook=None), synchronize_session=False)
 
         # Update repos and last sync
         self.account.extra_data.update(
             dict(
-                repos=active_repos,
+                repos=github_repos,
                 last_sync=iso_utcnow(),
             )
         )
         self.account.extra_data.changed()
         db.session.add(self.account)
 
     def _sync_hooks(self, repos, asynchronous=True):
@@ -236,17 +239,17 @@
         # If hook on GitHub exists, get or create corresponding db object and
         # enable the hook. Otherwise remove the old hook information.
         repo = Repository.get(repo_id, gh_repo.full_name)
         if not repo:
             repo = Repository.create(self.user_id, repo_id, gh_repo.full_name)
 
         if hook:
-            Repository.enable(repo, self.user_id, hook.id)
+            self.enable_repo(repo, hook.id)
         else:
-            Repository.disable(repo)
+            self.disable_repo(repo)
 
     def check_sync(self):
         """Check if sync is required based on last sync date."""
         # If refresh interval is not specified, we should refresh every time.
         expiration = utcnow()
         refresh_td = current_app.config.get("GITHUB_REFRESH_TIMEDELTA")
         if refresh_td:
@@ -288,15 +291,15 @@
                     "web",  # GitHub identifier for webhook service
                     hook_config,
                     events=["release"],
                 )
             else:
                 hook.edit(config=hook_config, events=["release"])
 
-            Repository.enable(repo, self.user_id, hook.id)
+            self.enable_repo(repo, hook.id)
             return True
 
         return False
 
     def remove_hook(self, repo_id, name):
         """Remove repository hook."""
         repo = Repository.get(github_id=repo_id, name=name)
@@ -311,66 +314,82 @@
         ghrepo = self.api.repository_with_id(repo_id)
         if ghrepo:
             hooks = (
                 h for h in ghrepo.hooks() if h.config.get("url", "") == self.webhook_url
             )
             hook = next(hooks, None)
             if not hook or hook.delete():
-                Repository.disable(repo)
+                self.disable_repo(repo)
                 return True
         return False
 
-    def get_repository_releases(self, repo_name="", repo=None):
-        """Retrieve repository releases."""
-        if not (repo or repo_name):
-            raise ValueError("At least one of (repo, repo_name) is required")
-
-        if not repo:
-            repo = Repository.get(name=repo_name)
-
-        check_repo_access_permissions(repo, self.user_id, repo.github_id, repo_name)
+    def get_repository_releases(self, repo):
+        """Retrieve repository releases. Returns API release objects."""
+        check_repo_access_permissions(repo, self.user_id, repo.github_id, repo.name)
 
         # Retrieve releases and sort them by creation date
-        release_objects = sorted(repo.releases.all(), key=lambda r: r.created)
+        release_instances = []
+        for release_object in repo.releases.order_by(Release.created):
+            release_instance = current_github.release_api_class(release_object)
+            release_instances.append(release_instance)
 
-        return release_objects
+        return release_instances
 
     def get_user_repositories(self):
-        """Retrieves user repositories."""
-        token = self.session_token
-        if token:
-            extra_data = self.account.extra_data
-        repos = extra_data.get("repos", [])
+        """Retrieves user repositories, containing db repositories plus remote repositories."""
+        repos = deepcopy(self.user_available_repositories)
         if repos:
             # 'Enhance' our repos dict, from our database model
-            db_repos = Repository.query.filter(
-                Repository.github_id.in_([int(k) for k in repos.keys()]),
-            ).all()
+            db_repos = self.user_enabled_repositories
             for repo in db_repos:
-                repos[str(repo.github_id)]["instance"] = repo
-                repos[str(repo.github_id)]["latest"] = GitHubRelease(
-                    repo.latest_release()
-                )
+                # TODO here
+                if str(repo.github_id) in repos:
+                    release_instance = current_github.release_api_class(
+                        repo.latest_release()
+                    )
+                    repos[str(repo.github_id)]["instance"] = repo
+                    repos[str(repo.github_id)]["latest"] = release_instance
         return repos
 
+    @property
+    def user_enabled_repositories(self):
+        """Retrieve user repositories from the model."""
+        return Repository.query.filter(Repository.user_id == self.user_id)
+
+    @property
+    def user_available_repositories(self):
+        """Retrieve user repositories from user's remote data."""
+        return self.account.extra_data.get("repos", [])
+
+    def disable_repo(self, repo):
+        """Disables an user repository if the user has permission to do so."""
+        check_repo_access_permissions(repo, self.user_id, repo.github_id, repo.name)
+
+        repo.hook = None
+        repo.user_id = None
+
+    def enable_repo(self, repo, hook):
+        """Enables an user repository if the user has permission to do so."""
+        check_repo_access_permissions(repo, self.user_id, repo.github_id, repo.name)
+
+        repo.hook = hook
+        repo.user_id = self.user_id
+
     def get_last_sync_time(self):
         """Retrieves the last sync delta time from github's client extra data.
 
         Time is computed as the delta between now and the last sync time.
         """
         if not self.account.extra_data.get("last_sync"):
             raise RemoteAccountDataNotSet(
                 self.user_id, "Last sync data is not set for user (remote data)."
             )
 
         extra_data = self.account.extra_data
-        last_sync = humanize.naturaltime(
-            (utcnow() - parse_timestamp(extra_data["last_sync"]))
-        )
-        return last_sync
+        return extra_data["last_sync"]
 
     def get_repository(self, repo_name):
         """Retrieves one repository.
 
         Checks for access permission.
         """
         repo = Repository.get(name=repo_name)
@@ -596,7 +615,11 @@
     def process_release(self):
         """Processes a github release."""
         raise NotImplementedError
 
     def resolve_record(self):
         """Resolves a record from the release. To be implemented by the API class implementation."""
         raise NotImplementedError
+
+    def serialize_record(self):
+        """Serializes the release record."""
+        raise NotImplementedError
```

### Comparing `invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/invenio_github/init.js` & `invenio-github-1.0.0b2/invenio_github/proxies.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,73 @@
-00000000: 2f2a 0a20 2a20 5468 6973 2066 696c 6520  /*. * This file 
-00000010: 6973 2070 6172 7420 6f66 2049 6e76 656e  is part of Inven
-00000020: 696f 2e0a 202a 2043 6f70 7972 6967 6874  io.. * Copyright
-00000030: 2028 4329 2032 3031 342c 2032 3031 352c   (C) 2014, 2015,
-00000040: 2032 3031 3620 4345 524e 2e0a 202a 0a20   2016 CERN.. *. 
-00000050: 2a20 496e 7665 6e69 6f20 6973 2066 7265  * Invenio is fre
-00000060: 6520 736f 6674 7761 7265 3a20 796f 7520  e software: you 
-00000070: 6361 6e20 7265 6469 7374 7269 6275 7465  can redistribute
-00000080: 2069 7420 616e 642f 6f72 206d 6f64 6966   it and/or modif
-00000090: 790a 202a 2069 7420 756e 6465 7220 7468  y. * it under th
-000000a0: 6520 7465 726d 7320 6f66 2074 6865 2047  e terms of the G
-000000b0: 4e55 2047 656e 6572 616c 2050 7562 6c69  NU General Publi
-000000c0: 6320 4c69 6365 6e73 6520 6173 2070 7562  c License as pub
-000000d0: 6c69 7368 6564 2062 790a 202a 2074 6865  lished by. * the
-000000e0: 2046 7265 6520 536f 6674 7761 7265 2046   Free Software F
-000000f0: 6f75 6e64 6174 696f 6e2c 2065 6974 6865  oundation, eithe
-00000100: 7220 7665 7273 696f 6e20 3320 6f66 2074  r version 3 of t
-00000110: 6865 204c 6963 656e 7365 2c20 6f72 0a20  he License, or. 
-00000120: 2a20 2861 7420 796f 7572 206f 7074 696f  * (at your optio
-00000130: 6e29 2061 6e79 206c 6174 6572 2076 6572  n) any later ver
-00000140: 7369 6f6e 2e0a 202a 0a20 2a20 496e 7665  sion.. *. * Inve
-00000150: 6e69 6f20 6973 2064 6973 7472 6962 7574  nio is distribut
-00000160: 6564 2069 6e20 7468 6520 686f 7065 2074  ed in the hope t
-00000170: 6861 7420 6974 2077 696c 6c20 6265 2075  hat it will be u
-00000180: 7365 6675 6c2c 0a20 2a20 6275 7420 5749  seful,. * but WI
-00000190: 5448 4f55 5420 414e 5920 5741 5252 414e  THOUT ANY WARRAN
-000001a0: 5459 3b20 7769 7468 6f75 7420 6576 656e  TY; without even
-000001b0: 2074 6865 2069 6d70 6c69 6564 2077 6172   the implied war
-000001c0: 7261 6e74 7920 6f66 0a20 2a20 4d45 5243  ranty of. * MERC
+00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
+00000010: 662d 3820 2d2a 2d0a 230a 2320 5468 6973  f-8 -*-.#.# This
+00000020: 2066 696c 6520 6973 2070 6172 7420 6f66   file is part of
+00000030: 2049 6e76 656e 696f 2e0a 2320 436f 7079   Invenio..# Copy
+00000040: 7269 6768 7420 2843 2920 3230 3233 2043  right (C) 2023 C
+00000050: 4552 4e2e 0a23 0a23 2049 6e76 656e 696f  ERN..#.# Invenio
+00000060: 2069 7320 6672 6565 2073 6f66 7477 6172   is free softwar
+00000070: 653b 2079 6f75 2063 616e 2072 6564 6973  e; you can redis
+00000080: 7472 6962 7574 6520 6974 0a23 2061 6e64  tribute it.# and
+00000090: 2f6f 7220 6d6f 6469 6679 2069 7420 756e  /or modify it un
+000000a0: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
+000000b0: 2074 6865 2047 4e55 2047 656e 6572 616c   the GNU General
+000000c0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+000000d0: 6173 0a23 2070 7562 6c69 7368 6564 2062  as.# published b
+000000e0: 7920 7468 6520 4672 6565 2053 6f66 7477  y the Free Softw
+000000f0: 6172 6520 466f 756e 6461 7469 6f6e 3b20  are Foundation; 
+00000100: 6569 7468 6572 2076 6572 7369 6f6e 2032  either version 2
+00000110: 206f 6620 7468 650a 2320 4c69 6365 6e73   of the.# Licens
+00000120: 652c 206f 7220 2861 7420 796f 7572 206f  e, or (at your o
+00000130: 7074 696f 6e29 2061 6e79 206c 6174 6572  ption) any later
+00000140: 2076 6572 7369 6f6e 2e0a 230a 2320 496e   version..#.# In
+00000150: 7665 6e69 6f20 6973 2064 6973 7472 6962  venio is distrib
+00000160: 7574 6564 2069 6e20 7468 6520 686f 7065  uted in the hope
+00000170: 2074 6861 7420 6974 2077 696c 6c20 6265   that it will be
+00000180: 0a23 2075 7365 6675 6c2c 2062 7574 2057  .# useful, but W
+00000190: 4954 484f 5554 2041 4e59 2057 4152 5241  ITHOUT ANY WARRA
+000001a0: 4e54 593b 2077 6974 686f 7574 2065 7665  NTY; without eve
+000001b0: 6e20 7468 6520 696d 706c 6965 6420 7761  n the implied wa
+000001c0: 7272 616e 7479 206f 660a 2320 4d45 5243  rranty of.# MERC
 000001d0: 4841 4e54 4142 494c 4954 5920 6f72 2046  HANTABILITY or F
 000001e0: 4954 4e45 5353 2046 4f52 2041 2050 4152  ITNESS FOR A PAR
 000001f0: 5449 4355 4c41 5220 5055 5250 4f53 452e  TICULAR PURPOSE.
-00000200: 2020 5365 6520 7468 650a 202a 2047 4e55    See the. * GNU
-00000210: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-00000220: 4c69 6365 6e73 6520 666f 7220 6d6f 7265  License for more
-00000230: 2064 6574 6169 6c73 2e0a 202a 0a20 2a20   details.. *. * 
-00000240: 596f 7520 7368 6f75 6c64 2068 6176 6520  You should have 
-00000250: 7265 6365 6976 6564 2061 2063 6f70 7920  received a copy 
-00000260: 6f66 2074 6865 2047 4e55 2047 656e 6572  of the GNU Gener
-00000270: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-00000280: 650a 202a 2061 6c6f 6e67 2077 6974 6820  e. * along with 
-00000290: 496e 7665 6e69 6f2e 2049 6620 6e6f 742c  Invenio. If not,
-000002a0: 2073 6565 203c 6874 7470 3a2f 2f77 7777   see <http://www
-000002b0: 2e67 6e75 2e6f 7267 2f6c 6963 656e 7365  .gnu.org/license
-000002c0: 732f 3e2e 0a20 2a0a 202a 2049 6e20 6170  s/>.. *. * In ap
-000002d0: 706c 7969 6e67 2074 6869 7320 6c69 6365  plying this lice
-000002e0: 6e63 652c 2043 4552 4e20 646f 6573 206e  nce, CERN does n
-000002f0: 6f74 2077 6169 7665 2074 6865 2070 7269  ot waive the pri
-00000300: 7669 6c65 6765 7320 616e 6420 696d 6d75  vileges and immu
-00000310: 6e69 7469 6573 0a20 2a20 6772 616e 7465  nities. * grante
-00000320: 6420 746f 2069 7420 6279 2076 6972 7475  d to it by virtu
-00000330: 6520 6f66 2069 7473 2073 7461 7475 7320  e of its status 
-00000340: 6173 2061 6e20 496e 7465 7267 6f76 6572  as an Intergover
-00000350: 6e6d 656e 7461 6c20 4f72 6761 6e69 7a61  nmental Organiza
-00000360: 7469 6f6e 0a20 2a20 6f72 2073 7562 6d69  tion. * or submi
-00000370: 7420 6974 7365 6c66 2074 6f20 616e 7920  t itself to any 
-00000380: 6a75 7269 7364 6963 7469 6f6e 2e0a 202a  jurisdiction.. *
-00000390: 2f0a 0a2f 2f20 7265 7175 6972 6528 5b0a  /..// require([.
-000003a0: 2f2f 2020 2027 6a71 7565 7279 272c 0a2f  //   'jquery',./
-000003b0: 2f20 2020 276e 6f64 655f 6d6f 6475 6c65  /   'node_module
-000003c0: 732f 626f 6f74 7374 7261 702d 7377 6974  s/bootstrap-swit
-000003d0: 6368 2f64 6973 742f 6a73 2f62 6f6f 7473  ch/dist/js/boots
-000003e0: 7472 6170 2d73 7769 7463 6827 2c0a 2f2f  trap-switch',.//
-000003f0: 2020 2027 6a73 2f67 6974 6875 622f 7669     'js/github/vi
-00000400: 6577 270a 2f2f 2020 205d 2c20 6675 6e63  ew'.//   ], func
-00000410: 7469 6f6e 2829 207b 0a2f 2f20 2020 2020  tion() {.//     
-00000420: 2f2a 0a2f 2f20 2020 2020 202a 2049 7420  /*.//      * It 
-00000430: 7072 656c 6f61 6473 206a 732f 6769 7468  preloads js/gith
-00000440: 7562 2f76 6965 7720 746f 2067 6976 6520  ub/view to give 
-00000450: 6974 2061 206e 616d 6520 736f 2079 6f75  it a name so you
-00000460: 2772 6520 6672 6565 2074 6f20 7573 6520  're free to use 
-00000470: 6974 0a2f 2f20 2020 2020 202a 2066 726f  it.//      * fro
-00000480: 6d20 616e 7920 706c 6163 6573 2e0a 2f2f  m any places..//
-00000490: 2020 2020 2020 2a2f 0a2f 2f20 2020 2020        */.//     
-000004a0: 636f 6e73 6f6c 652e 696e 666f 2822 6a73  console.info("js
-000004b0: 2f67 6974 6875 622f 696e 6974 2069 7320  /github/init is 
-000004c0: 6c6f 6164 6564 2229 3b0a 2f2f 207d 293b  loaded");.// });
-000004d0: 0a                                       .
+00000200: 2020 5365 6520 7468 6520 474e 550a 2320    See the GNU.# 
+00000210: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
+00000220: 6963 656e 7365 2066 6f72 206d 6f72 6520  icense for more 
+00000230: 6465 7461 696c 732e 0a23 0a23 2059 6f75  details..#.# You
+00000240: 2073 686f 756c 6420 6861 7665 2072 6563   should have rec
+00000250: 6569 7665 6420 6120 636f 7079 206f 6620  eived a copy of 
+00000260: 7468 6520 474e 5520 4765 6e65 7261 6c20  the GNU General 
+00000270: 5075 626c 6963 204c 6963 656e 7365 0a23  Public License.#
+00000280: 2061 6c6f 6e67 2077 6974 6820 496e 7665   along with Inve
+00000290: 6e69 6f3b 2069 6620 6e6f 742c 2077 7269  nio; if not, wri
+000002a0: 7465 2074 6f20 7468 650a 2320 4672 6565  te to the.# Free
+000002b0: 2053 6f66 7477 6172 6520 466f 756e 6461   Software Founda
+000002c0: 7469 6f6e 2c20 496e 632e 2c20 3539 2054  tion, Inc., 59 T
+000002d0: 656d 706c 6520 506c 6163 652c 2053 7569  emple Place, Sui
+000002e0: 7465 2033 3330 2c20 426f 7374 6f6e 2c0a  te 330, Boston,.
+000002f0: 2320 4d41 2030 3231 3131 2d31 3330 372c  # MA 02111-1307,
+00000300: 2055 5341 2e0a 230a 2320 496e 2061 7070   USA..#.# In app
+00000310: 6c79 696e 6720 7468 6973 206c 6963 656e  lying this licen
+00000320: 7365 2c20 4345 524e 2064 6f65 7320 6e6f  se, CERN does no
+00000330: 740a 2320 7761 6976 6520 7468 6520 7072  t.# waive the pr
+00000340: 6976 696c 6567 6573 2061 6e64 2069 6d6d  ivileges and imm
+00000350: 756e 6974 6965 7320 6772 616e 7465 6420  unities granted 
+00000360: 746f 2069 7420 6279 2076 6972 7475 6520  to it by virtue 
+00000370: 6f66 2069 7473 2073 7461 7475 730a 2320  of its status.# 
+00000380: 6173 2061 6e20 496e 7465 7267 6f76 6572  as an Intergover
+00000390: 6e6d 656e 7461 6c20 4f72 6761 6e69 7a61  nmental Organiza
+000003a0: 7469 6f6e 206f 7220 7375 626d 6974 2069  tion or submit i
+000003b0: 7473 656c 6620 746f 2061 6e79 206a 7572  tself to any jur
+000003c0: 6973 6469 6374 696f 6e2e 0a0a 2222 2250  isdiction..."""P
+000003d0: 726f 7879 2066 6f72 2063 7572 7265 6e74  roxy for current
+000003e0: 2070 7265 7669 6577 6572 2e22 2222 0a0a   previewer."""..
+000003f0: 6672 6f6d 2066 6c61 736b 2069 6d70 6f72  from flask impor
+00000400: 7420 6375 7272 656e 745f 6170 700a 6672  t current_app.fr
+00000410: 6f6d 2077 6572 6b7a 6575 672e 6c6f 6361  om werkzeug.loca
+00000420: 6c20 696d 706f 7274 204c 6f63 616c 5072  l import LocalPr
+00000430: 6f78 790a 0a63 7572 7265 6e74 5f67 6974  oxy..current_git
+00000440: 6875 6220 3d20 4c6f 6361 6c50 726f 7879  hub = LocalProxy
+00000450: 286c 616d 6264 613a 2063 7572 7265 6e74  (lambda: current
+00000460: 5f61 7070 2e65 7874 656e 7369 6f6e 735b  _app.extensions[
+00000470: 2269 6e76 656e 696f 2d67 6974 6875 6222  "invenio-github"
+00000480: 5d29 0a                                  ]).
```

### Comparing `invenio-github-1.0.0b1/invenio_github/config.py` & `invenio-github-1.0.0b2/invenio_github/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,19 +18,16 @@
 #
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization
 # or submit itself to any jurisdiction.
 
 """Configuration for GitHub module."""
 
-from copy import deepcopy
 from datetime import timedelta
 
-from invenio_oauthclient.contrib.github import REMOTE_APP
-
 GITHUB_WEBHOOK_RECEIVER_ID = "github"
 """Local name of webhook receiver."""
 
 GITHUB_WEBHOOK_RECEIVER_URL = None
 """URL format to be used when creating a webhook on GitHub.
 
 This configuration variable must be set explicitly. Example::
@@ -73,11 +70,9 @@
 
 GITHUB_ERROR_HANDLERS = None
 """Definition of the way specific exceptions are handled."""
 
 GITHUB_MAX_CONTRIBUTORS_NUMBER = 30
 """Max number of contributors of a release to be retrieved from Github."""
 
-# Copy the default GitHub OAuth application configuration, and update disconnect handlers and scope.
-"""OAuth Client configuration."""
-REMOTE_APP["disconnect_handler"] = "invenio_github.handlers:disconnect"
-REMOTE_APP["params"]["request_token_params"]["scope"] = "user,admin:repo_hook,read:org"
+GITHUB_INTEGRATION_ENABLED = False
+"""Enables the github integration."""
```

### Comparing `invenio-github-1.0.0b1/invenio_github/errors.py` & `invenio-github-1.0.0b2/invenio_github/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/models.py` & `invenio-github-1.0.0b2/invenio_github/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,19 +40,19 @@
     "PROCESSING": _("Processing"),
     "PUBLISHED": _("Published"),
     "FAILED": _("Failed"),
     "DELETED": _("Deleted"),
 }
 
 RELEASE_STATUS_ICON = {
-    "RECEIVED": "fa-spinner",
-    "PROCESSING": "fa-spinner",
-    "PUBLISHED": "fa-check",
-    "FAILED": "fa-times",
-    "DELETED": "fa-times",
+    "RECEIVED": "spinner icon",
+    "PROCESSING": "spinner icon",
+    "PUBLISHED": "check icon",
+    "FAILED": "times icon",
+    "DELETED": "times icon",
 }
 
 RELEASE_STATUS_COLOR = {
     "RECEIVED": "default",
     "PROCESSING": "default",
     "PUBLISHED": "success",
     "FAILED": "danger",
@@ -177,45 +177,14 @@
                  exist.
         """
         repo = cls.query.filter(
             (Repository.github_id == github_id) | (Repository.name == name)
         ).one_or_none()
         return repo
 
-    @classmethod
-    def enable(cls, repo, user_id, hook):
-        """Enable webhooks for a repository.
-
-        If the repository does not exist it will create one.
-
-        :param user_id: User identifier.
-        :param repo_id: GitHub repository identifier.
-        :param name: Fully qualified name of the repository.
-        :param hook: GitHub hook identifier (hook id).
-        """
-        repo.hook = hook
-        repo.user_id = user_id
-        db.session.add(repo)
-        return repo
-
-    @classmethod
-    def disable(cls, repo):
-        """Disable webhooks for a repository.
-
-        Disables the webhook from a repository if it exists in the DB.
-
-        :param user_id: User identifier.
-        :param repo_id: GitHub id of the repository.
-        :param name: Fully qualified name of the repository.
-        """
-        repo.hook = None
-        repo.user_id = None
-        db.session.add(repo)
-        return repo
-
     @property
     def enabled(self):
         """Return if the repository has webhooks enabled."""
         return bool(self.hook)
 
     def latest_release(self, status=None):
         """Chronologically latest published release of the repository."""
```

### Comparing `invenio-github-1.0.0b1/invenio_github/proxies.py` & `invenio-github-1.0.0b2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2023 CERN.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -18,13 +19,12 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
-"""Proxy for current previewer."""
+"""Invenio module that adds GitHub integration to the platform."""
 
-from flask import current_app
-from werkzeug.local import LocalProxy
+from setuptools import setup
 
-current_github = LocalProxy(lambda: current_app.extensions["invenio-github"])
+setup()
```

### Comparing `invenio-github-1.0.0b1/invenio_github/receivers.py` & `invenio-github-1.0.0b2/invenio_github/receivers.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,37 +32,28 @@
     InvalidSenderError,
     ReleaseAlreadyReceivedError,
     RepositoryAccessError,
     RepositoryDisabledError,
     RepositoryNotFoundError,
 )
 
-state = {}
-
 
 class GitHubReceiver(Receiver):
     """Handle incoming notification from GitHub on a new release."""
 
     def run(self, event):
         """Process an event.
 
         .. note::
 
             We should only do basic server side operation here, since we send
             the rest of the processing to a Celery task which will be mainly
             accessing the GitHub API.
         """
-        try:
-            self._handle_event(event)
-        except Exception as e:
-            # Event failed to be processed and error was not handled yet
-            if not event.response or event.response_code < 400:
-                event.response = {"status": 500, "message": str(e)}
-                event.response_code = 500
-            # Other cases were already handled (e.g. response/response_code were set by the event handler)
+        self._handle_event(event)
 
     def _handle_event(self, event):
         """Handles an incoming github event."""
         action = event.payload.get("action")
         is_draft_release = event.payload.get("release", {}).get("draft")
 
         # Draft releases do not create releases on invenio
@@ -75,19 +66,14 @@
         else:
             pass
 
     def _handle_create_release(self, event):
         """Creates a release in invenio."""
         try:
             release_id = event.payload["release"]["id"]
-            if release_id in state:
-                raise ReleaseAlreadyReceivedError()
-
-            # Lock event release to avoid concurrent processing
-            state.update({release_id: event})
 
             # Check if the release already exists
             existing_release = Release.query.filter_by(
                 release_id=release_id,
             ).first()
 
             if existing_release:
@@ -113,16 +99,14 @@
                 raise RepositoryDisabledError(repo=repo)
 
             # Process the release
             # Since 'process_release' is executed asynchronously, we commit the current state of session
             db.session.commit()
             process_release.delay(release.release_id)
 
-            # Unlock the event release
-            del state[release_id]
         except (ReleaseAlreadyReceivedError, RepositoryDisabledError) as e:
             event.response_code = 409
             event.response = dict(message=str(e), status=409)
         except (RepositoryAccessError, InvalidSenderError) as e:
             event.response_code = 403
             event.response = dict(message=str(e), status=403)
         except RepositoryNotFoundError as e:
```

### Comparing `invenio-github-1.0.0b1/invenio_github/tasks.py` & `invenio-github-1.0.0b2/invenio_github/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/base.html` & `invenio-github-1.0.0b2/tests/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-{# -*- coding: utf-8 -*-
+#!/usr/bin/env sh
+# -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -17,17 +18,9 @@
 # along with Invenio; if not, write to the
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
-#}
-{%- extends "invenio_oauth2server/base.html" %}
 
-{%- block page_body %}
-{%- block settings_content %}
-{%- block settings_body %}
-{%- block settings_form %}{%- endblock settings_form %}
-{%- endblock settings_body %}
-{%- endblock settings_content %}
-{%- endblock page_body %}
+"""Unit test for Invenio-Github."""
```

### Comparing `invenio-github-1.0.0b1/invenio_github/translations/cs/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b2/invenio_github/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/translations/da/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b2/invenio_github/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/translations/de/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b2/invenio_github/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/translations/en/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b2/invenio_github/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/translations/es/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b2/invenio_github/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/translations/fr/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b2/invenio_github/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/translations/it/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b2/invenio_github/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/translations/messages.pot` & `invenio-github-1.0.0b2/invenio_github/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/utils.py` & `invenio-github-1.0.0b2/invenio_github/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/views/__init__.py` & `invenio-github-1.0.0b2/invenio_github/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/views/badge.py` & `invenio-github-1.0.0b2/invenio_github/views/badge.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/invenio_github/views/github.py` & `invenio-github-1.0.0b2/invenio_github/views/github.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,190 +53,197 @@
             raise GithubTokenNotFound(current_user, "Github session token is requested")
 
         return inner
 
     return decorator
 
 
-blueprint = Blueprint(
-    "invenio_github",
-    __name__,
-    static_folder="../static",
-    template_folder="../templates",
-    url_prefix="/account/settings/github",
-)
-
-
-@blueprint.route("/")
-@login_required
-@request_session_token()
-@register_menu(  # TODO modify?
-    blueprint,
-    "settings.github",
-    # TODO substitute github for icon + 'Github'
-    _("Github"),
-    # _(
-    #     "%(icon)s GitHub",
-    #     icon=make_lazy_string(
-    #         lambda: '<i class="{icon}"></i>'.format(
-    #             icon=current_theme_icons.github
-    #         )  # TODO confirm if icon gets picked
-    #     ),
-    # ),
-    order=10,  # TODO confirm
-    # active_when=lambda: request.endpoint.startswith("invenio_github."),
-)
-@register_breadcrumb(blueprint, "breadcrumbs.settings.github", _("GitHub"))
-def get_repositories():
-    """Display list of the user's repositories."""
-    github = GitHubAPI(user_id=current_user.id)
-    ctx = dict(connected=False)
-
-    # Generate the repositories view object
-    repos = github.get_user_repositories()
-    last_sync = github.get_last_sync_time()
-
-    ctx.update(
-        {
-            # TODO maybe can be refactored. e.g. have two templates and render the correct one.
-            "connected": True,
-            "repos": sorted(repos.items(), key=lambda x: x[1]["full_name"]),
-            "last_sync": last_sync,
-        }
+def create_ui_blueprint(app):
+    """Creates blueprint and registers UI endpoints if the integration is enabled."""
+    blueprint = Blueprint(
+        "invenio_github",
+        __name__,
+        static_folder="../static",
+        template_folder="../templates",
+        url_prefix="/account/settings/github",
     )
+    if app.config.get("GITHUB_INTEGRATION_ENABLED", False):
+        register_ui_routes(blueprint)
+    return blueprint
+
+
+def create_api_blueprint(app):
+    """Creates blueprint and registers API endpoints if the integration is enabled."""
+    blueprint_api = Blueprint("invenio_github_api", __name__)
+    if app.config.get("GITHUB_INTEGRATION_ENABLED", False):
+        register_api_routes(blueprint_api)
+    return blueprint_api
+
+
+def register_ui_routes(blueprint):
+    """Register ui routes."""
+
+    @blueprint.route("/")
+    @login_required
+    @request_session_token()
+    @register_menu(  # TODO modify?
+        blueprint,
+        "settings.github",
+        # TODO substitute github for icon + 'Github'
+        _("Github"),
+        # _(
+        #     "%(icon)s GitHub",
+        #     icon=make_lazy_string(
+        #         lambda: '<i class="{icon}"></i>'.format(
+        #             icon=current_theme_icons.github
+        #         )  # TODO confirm if icon gets picked
+        #     ),
+        # ),
+        order=10,  # TODO confirm
+        # active_when=lambda: request.endpoint.startswith("invenio_github."),
+    )
+    @register_breadcrumb(blueprint, "breadcrumbs.settings.github", _("GitHub"))
+    def get_repositories():
+        """Display list of the user's repositories."""
+        github = GitHubAPI(user_id=current_user.id)
+        ctx = dict(connected=False)
 
-    return render_template(current_app.config["GITHUB_TEMPLATE_INDEX"], **ctx)
-
-
-@blueprint.route("/repository/<path:repo_name>")
-@request_session_token()
-def get_repository(repo_name):
-    """Displays one repository.
-
-    Retrieves and builds context to display all repository releases, if any.
-    """
-    user_id = current_user.id
-    github = GitHubAPI(user_id=user_id)
-
-    try:
-        # NOTE: Here we do not check for repository ownership, since it
-        # might have changed even though the user might have made releases
-        # in the past.
-        repo = github.get_repository(repo_name)
-        releases = github.get_repository_releases(repo=repo)
-        return render_template(
-            current_app.config["GITHUB_TEMPLATE_VIEW"],
-            repo=repo,
-            releases=releases,
-            serializer=current_github.record_serializer,
+        # Generate the repositories view object
+        repos = github.get_user_repositories()
+        last_sync = github.get_last_sync_time()
+
+        ctx.update(
+            {
+                # TODO maybe can be refactored. e.g. have two templates and render the correct one.
+                "connected": True,
+                "repos": sorted(repos.items(), key=lambda x: x[1]["full_name"]),
+                "last_sync": last_sync,
+            }
         )
-    except RepositoryAccessError as e:
-        abort(403)
-    except NoResultFound as e:
-        abort(404)
-
-
-###
-# TODO to be moved to its own folder (e.g. separate ui / api)
-# /api routes
-###
-
-blueprint_api = Blueprint("invenio_github_api", __name__)
-
-
-@login_required
-@blueprint_api.route("/user/github/repositories/sync", methods=["POST"])
-def sync_user_repositories():
-    """Synchronizes user repos.
-
-    Currently:
-        POST /api/user/github/repositories/sync
-    Previously:
-        POST /account/settings/github/hook
-    """
-    try:
-        github = GitHubAPI(user_id=current_user.id)
-        github.sync(async_hooks=False)
-        db.session.commit()
-    except Exception:
-        db.session.rollback()
-        abort(500)
-
-    return "", 200
 
+        return render_template(current_app.config["GITHUB_TEMPLATE_INDEX"], **ctx)
 
-@login_required
-@request_session_token()
-@blueprint_api.route("/user/github/", methods=["POST"])
-def init_user_github():
-    """Initialises github account for an user."""
-    try:
-        github = GitHubAPI(user_id=current_user.id)
-        github.init_account()
-        github.sync(async_hooks=False)
-        db.session.commit()
-    except Exception:
-        db.session.rollback()
-        abort(500)
-    return "", 200
-
-
-@login_required
-@request_session_token()
-@blueprint_api.route(
-    "/user/github/repositories/<repository_id>/enable", methods=["POST"]
-)
-def enable_repository(repository_id):
-    """Enables one repository.
-
-    Currently:
-        POST /api/user/github/repositories/<repository_id>/enable
-    Previously:
-        POST /account/settings/github/hook
-    """
-    try:
-        github = GitHubAPI(user_id=current_user.id)
+    @blueprint.route("/repository/<path:repo_name>")
+    @login_required
+    @request_session_token()
+    @register_breadcrumb(blueprint, "breadcrumbs.settings.github.repo", _("Repository"))
+    def get_repository(repo_name):
+        """Displays one repository.
+
+        Retrieves and builds context to display all repository releases, if any.
+        """
+        user_id = current_user.id
+        github = GitHubAPI(user_id=user_id)
+
+        try:
+            repo = github.get_repository(repo_name)
+            default_branch = (
+                github.account.extra_data.get("repos", [])
+                .get(str(repo.github_id), None)
+                .get("default_branch", None)
+            )
+            releases = github.get_repository_releases(repo=repo)
+            return render_template(
+                current_app.config["GITHUB_TEMPLATE_VIEW"],
+                repo=repo,
+                releases=releases,
+                default_branch=default_branch,
+            )
+        except RepositoryAccessError as e:
+            abort(403)
+        except NoResultFound as e:
+            abort(404)
+
+
+def register_api_routes(blueprint):
+    """Register API routes."""
+
+    @login_required
+    @blueprint.route("/user/github/repositories/sync", methods=["POST"])
+    def sync_user_repositories():
+        """Synchronizes user repos.
+
+        Currently:
+            POST /api/user/github/repositories/sync
+        Previously:
+            POST /account/settings/github/hook
+        """
+        try:
+            github = GitHubAPI(user_id=current_user.id)
+            github.sync(async_hooks=False)
+            db.session.commit()
+        except Exception:
+            abort(400)
 
-        repos = github.account.extra_data["repos"]
-        create_success = github.create_hook(
-            repository_id, repos[repository_id]["full_name"]
-        )
-        db.session.commit()
-        if create_success:
-            return "", 201
-        else:
+        return "", 200
+
+    @login_required
+    @request_session_token()
+    @blueprint.route("/user/github/", methods=["POST"])
+    def init_user_github():
+        """Initialises github account for an user."""
+        try:
+            github = GitHubAPI(user_id=current_user.id)
+            github.init_account()
+            github.sync(async_hooks=False)
+            db.session.commit()
+        except Exception:
             abort(400)
-    except Exception:
-        db.session.rollback()
-        abort(500)
-
-
-@login_required
-@request_session_token()
-@blueprint_api.route(
-    "/user/github/repositories/<repository_id>/disable", methods=["POST"]
-)
-def disable_repository(repository_id):
-    """Disables one repository.
-
-    Currently:
-        POST /api/user/github/repositories/<repository_id>/disable
-    Previously:
-        DELETE /account/settings/github/hook
-    """
-    try:
-        github = GitHubAPI(user_id=current_user.id)
+        return "", 200
+
+    @login_required
+    @request_session_token()
+    @blueprint.route(
+        "/user/github/repositories/<repository_id>/enable", methods=["POST"]
+    )
+    def enable_repository(repository_id):
+        """Enables one repository.
 
-        repos = github.account.extra_data.get("repos", [])
-        remove_success = False
-        if repos:
-            remove_success = github.remove_hook(
+        Currently:
+            POST /api/user/github/repositories/<repository_id>/enable
+        Previously:
+            POST /account/settings/github/hook
+        """
+        try:
+            github = GitHubAPI(user_id=current_user.id)
+
+            repos = github.account.extra_data.get("repos", [])
+            create_success = github.create_hook(
                 repository_id, repos[repository_id]["full_name"]
             )
             db.session.commit()
-        if remove_success:
-            return "", 204
-        else:
+            if create_success:
+                return "", 201
+            else:
+                abort(400)
+        except Exception:
+            abort(400)
+
+    @login_required
+    @request_session_token()
+    @blueprint.route(
+        "/user/github/repositories/<repository_id>/disable", methods=["POST"]
+    )
+    def disable_repository(repository_id):
+        """Disables one repository.
+
+        Currently:
+            POST /api/user/github/repositories/<repository_id>/disable
+        Previously:
+            DELETE /account/settings/github/hook
+        """
+        try:
+            github = GitHubAPI(user_id=current_user.id)
+
+            repos = github.account.extra_data.get("repos", [])
+            remove_success = False
+            if repos:
+                remove_success = github.remove_hook(
+                    repository_id, repos[repository_id]["full_name"]
+                )
+                db.session.commit()
+            if remove_success:
+                return "", 204
+            else:
+                abort(400)
+        except Exception:
             abort(400)
-    except Exception:
-        db.session.rollback()
-        abort(500)
```

### Comparing `invenio-github-1.0.0b1/invenio_github.egg-info/PKG-INFO` & `invenio-github-1.0.0b2/invenio_github.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,20 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.0b2 (released 2023-07-17)
+        
+        - global: restrain extension behind feature flag
+        - api: add record serialization
+        - handlers: fix hooks serialization
+        
         Version v1.0.0b1 (released 2023-07-03)
         
         - Initial beta release.
         
         Version v1.0.0a28 (released 2022-10-24)
         
         - Initial public release.
```

### Comparing `invenio-github-1.0.0b1/invenio_github.egg-info/SOURCES.txt` & `invenio-github-1.0.0b2/invenio_github.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -32,31 +32,28 @@
 docs/requirements.txt
 docs/usage.rst
 invenio_github/__init__.py
 invenio_github/api.py
 invenio_github/config.py
 invenio_github/errors.py
 invenio_github/ext.py
-invenio_github/handlers.py
 invenio_github/models.py
 invenio_github/proxies.py
 invenio_github/receivers.py
 invenio_github/tasks.py
 invenio_github/utils.py
 invenio_github/webpack.py
 invenio_github.egg-info/PKG-INFO
 invenio_github.egg-info/SOURCES.txt
 invenio_github.egg-info/dependency_links.txt
 invenio_github.egg-info/entry_points.txt
 invenio_github.egg-info/not-zip-safe
 invenio_github.egg-info/requires.txt
 invenio_github.egg-info/top_level.txt
-invenio_github/assets/semantic-ui/js/invenio_github/init.js
-invenio_github/assets/semantic-ui/js/invenio_github/view.js
-invenio_github/assets/semantic-ui/less/github/github.scss
+invenio_github/assets/semantic-ui/js/invenio_github/index.js
 invenio_github/templates/semantic-ui/invenio_github/base.html
 invenio_github/templates/semantic-ui/invenio_github/helpers.html
 invenio_github/templates/semantic-ui/invenio_github/settings/base.html
 invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
 invenio_github/templates/semantic-ui/invenio_github/settings/index.html
 invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
 invenio_github/templates/semantic-ui/invenio_github/settings/view.html
```

### Comparing `invenio-github-1.0.0b1/invenio_github.egg-info/entry_points.txt` & `invenio-github-1.0.0b2/invenio_github.egg-info/entry_points.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [invenio_assets.webpack]
 invenio_github = invenio_github.webpack:theme
 
 [invenio_base.api_apps]
 invenio_github = invenio_github:InvenioGitHub
 
 [invenio_base.api_blueprints]
-invenio_github = invenio_github.views.github:blueprint_api
+invenio_github = invenio_github.views.github:create_api_blueprint
 
 [invenio_base.apps]
 invenio_github = invenio_github:InvenioGitHub
 
 [invenio_base.blueprints]
 invenio_github_badge = invenio_github.views.badge:blueprint
-invenio_github_github = invenio_github.views.github:blueprint
+invenio_github_github = invenio_github.views.github:create_ui_blueprint
 
 [invenio_celery.tasks]
 invenio_github = invenio_github.tasks
 
 [invenio_db.models]
 invenio_github = invenio_github.models
```

### Comparing `invenio-github-1.0.0b1/invenio_github.egg-info/requires.txt` & `invenio-github-1.0.0b2/invenio_github.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/requirements-devel.txt` & `invenio-github-1.0.0b2/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/run-tests.sh` & `invenio-github-1.0.0b2/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/setup.cfg` & `invenio-github-1.0.0b2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,17 @@
 [options.entry_points]
 invenio_base.apps = 
 	invenio_github = invenio_github:InvenioGitHub
 invenio_base.api_apps = 
 	invenio_github = invenio_github:InvenioGitHub
 invenio_base.blueprints = 
 	invenio_github_badge = invenio_github.views.badge:blueprint
-	invenio_github_github = invenio_github.views.github:blueprint
+	invenio_github_github = invenio_github.views.github:create_ui_blueprint
 invenio_base.api_blueprints = 
-	invenio_github = invenio_github.views.github:blueprint_api
+	invenio_github = invenio_github.views.github:create_api_blueprint
 invenio_celery.tasks = 
 	invenio_github = invenio_github.tasks
 invenio_db.models = 
 	invenio_github = invenio_github.models
 invenio_i18n.translations = 
 	messages = invenio_github
 invenio_webhooks.receivers =
```

### Comparing `invenio-github-1.0.0b1/setup.py` & `invenio-github-1.0.0b2/tests/test_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2023 CERN.
-# Copyright (C) 2023 Graz University of Technology.
 #
-# Invenio is free software; you can redistribute it
-# and/or modify it under the terms of the GNU General Public License as
-# published by the Free Software Foundation; either version 2 of the
-# License, or (at your option) any later version.
+# Invenio is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
-# Invenio is distributed in the hope that it will be
-# useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# Invenio is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with Invenio; if not, write to the
-# Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
-# MA 02111-1307, USA.
+# along with Invenio. If not, see <http://www.gnu.org/licenses/>.
 #
-# In applying this license, CERN does not
-# waive the privileges and immunities granted to it by virtue of its status
-# as an Intergovernmental Organization or submit itself to any jurisdiction.
+# In applying this licence, CERN does not waive the privileges and immunities
+# granted to it by virtue of its status as an Intergovernmental Organization
+# or submit itself to any jurisdiction.
 
-"""Invenio module that adds GitHub integration to the platform."""
+"""Test cases for badge creation."""
 
-from setuptools import setup
+from invenio_github.models import Repository
 
-setup()
+
+def test_repository_unbound(app):
+    """Test create_badge method."""
+    assert Repository(name="org/repo", github_id=1).latest_release() is None
```

### Comparing `invenio-github-1.0.0b1/tests/conftest.py` & `invenio-github-1.0.0b2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         CELERY_RESULT_BACKEND="cache",
         GITHUB_APP_CREDENTIALS=dict(
             consumer_key="changeme",
             consumer_secret="changeme",
         ),
         GITHUB_SHARED_SECRET="changeme",
         GITHUB_INSECURE_SSL=False,
+        GITHUB_INTEGRATION_ENABLED=True,
         GITHUB_METADATA_FILE=".invenio.json",
         GITHUB_WEBHOOK_RECEIVER_URL="http://localhost:5000/api/receivers/github/events/?access_token={token}",
         GITHUB_WEBHOOK_RECEIVER_ID="github",
         GITHUB_RELEASE_CLASS=TestGithubRelease,
         LOGIN_DISABLED=False,
         OAUTHLIB_INSECURE_TRANSPORT=True,
         OAUTH2_CACHE_TYPE="simple",
@@ -200,15 +201,20 @@
 def test_repo_data_three():
     """Test repository."""
     return {"name": "arepo", "id": 3}
 
 
 @pytest.yield_fixture()
 def github_api(
-    running_app, db, test_repo_data_one, test_repo_data_two, test_repo_data_three
+    running_app,
+    db,
+    test_repo_data_one,
+    test_repo_data_two,
+    test_repo_data_three,
+    test_user,
 ):
     """Github API mock."""
     import github3
 
     from . import fixtures
 
     mock_api = MagicMock()
```

### Comparing `invenio-github-1.0.0b1/tests/fixtures.py` & `invenio-github-1.0.0b2/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/tests/test_api.py` & `invenio-github-1.0.0b2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/tests/test_badge.py` & `invenio-github-1.0.0b2/tests/test_badge.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/tests/test_invenio_github.py` & `invenio-github-1.0.0b2/tests/test_invenio_github.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/tests/test_tasks.py` & `invenio-github-1.0.0b2/tests/test_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization
 # or submit itself to any jurisdiction.
 
 from time import sleep
 
 from invenio_oauthclient.models import RemoteAccount
-
 from invenio_webhooks.models import Event
 from mock import patch
 
 from invenio_github.api import GitHubAPI
 from invenio_github.models import Release, ReleaseStatus, Repository
 from invenio_github.tasks import process_release, refresh_accounts
 from invenio_github.utils import iso_utcnow
@@ -50,17 +49,16 @@
     assert "repo-1" in extra_data["repos"][1]["full_name"]
     assert 2 in extra_data["repos"]
     assert "repo-2" in extra_data["repos"][2]["full_name"]
 
     repo_name = "repo-1"
     repo_id = 1
 
-    # Create the repository that will make the release
     repo = Repository.create(tester_id, repo_id, repo_name)
-    Repository.enable(repo, tester_id, hook=1234)
+    api.enable_repo(repo, 12345)
     event = Event(
         receiver_id="github",
         user_id=tester_id,
         payload=fixtures.PAYLOAD("auser", "repo-1", 1),
     )
 
     release_object = Release(
```

### Comparing `invenio-github-1.0.0b1/tests/test_views.py` & `invenio-github-1.0.0b2/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b1/tests/test_webhook.py` & `invenio-github-1.0.0b2/tests/test_webhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,37 +22,37 @@
 
 """Test GitHub hook."""
 
 import json
 
 # from invenio_rdm_records.proxies import current_rdm_records_service
 from invenio_webhooks.models import Event
-from sqlalchemy.orm.exc import NoResultFound
 
+from invenio_github.api import GitHubAPI
 from invenio_github.models import ReleaseStatus, Repository
 
 
 def test_webhook_post(app, db, tester_id, remote_token, github_api):
     """Test webhook POST success."""
     from . import fixtures
 
     repo_id = 3
     repo_name = "arepo"
     hook = 1234
     tag = "v1.0"
 
-    # Create a repository
     repo = Repository.get(github_id=repo_id, name=repo_name)
     if not repo:
         repo = Repository.create(tester_id, repo_id, repo_name)
 
+    api = GitHubAPI(tester_id)
+
     # Enable repository webhook.
-    Repository.enable(repo, tester_id, hook)
+    api.enable_repo(repo, hook)
 
-    # JSON payload parsing.
     payload = json.dumps(fixtures.PAYLOAD("auser", repo_name, repo_id, tag))
     headers = [("Content-Type", "application/json")]
     with app.test_request_context(headers=headers, data=payload):
         event = Event.create(receiver_id="github", user_id=tester_id)
         # Add event to session. Otherwise defaults are not added (e.g. response and response_code)
         db.session.add(event)
         db.session.commit()
@@ -79,16 +79,18 @@
     hook = 1234
 
     # Create a repository
     repo = Repository.get(github_id=repo_id, name=repo_name)
     if not repo:
         repo = Repository.create(tester_id, repo_id, repo_name)
 
+    api = GitHubAPI(tester_id)
+
     # Enable repository webhook.
-    Repository.enable(repo, tester_id, hook)
+    api.enable_repo(repo, hook)
 
     # Create an invalid payload (fake repo)
     fake_payload = json.dumps(
         fixtures.PAYLOAD("fake_user", "fake_repo", 1000, "v1000.0")
     )
     headers = [("Content-Type", "application/json")]
     with app.test_request_context(headers=headers, data=fake_payload):
```

