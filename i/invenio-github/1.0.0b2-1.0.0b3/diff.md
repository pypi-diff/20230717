# Comparing `tmp/invenio-github-1.0.0b2.tar.gz` & `tmp/invenio-github-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-github-1.0.0b2.tar", last modified: Mon Jul 17 09:34:13 2023, max compression
+gzip compressed data, was "dist/invenio-github-1.0.0b3.tar", last modified: Mon Jul 17 12:38:00 2023, max compression
```

## Comparing `invenio-github-1.0.0b2.tar` & `invenio-github-1.0.0b3.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/.lgtm
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4517 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/RELEASE-NOTES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/babel.ini
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10752 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22856 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/assets/semantic-ui/js/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/assets/semantic-ui/js/invenio_github/index.js
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/receivers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/helpers.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (122)     6503 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
--rw-r--r--   0 runner    (1001) docker     (122)    15043 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github/views/
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/views/badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     8193 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/views/github.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/invenio_github/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4517 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2356 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/invenio_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-17 09:34:12.000000 invenio-github-1.0.0b2/invenio_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:34:13.000000 invenio-github-1.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    21853 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_invenio_github.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     3693 2023-07-17 09:34:05.000000 invenio-github-1.0.0b2/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/.lgtm
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/RELEASE-NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10752 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22856 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/assets/semantic-ui/js/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/assets/semantic-ui/js/invenio_github/index.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/helpers.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6503 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
+-rw-r--r--   0 runner    (1001) docker     (122)    15043 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/views/badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8193 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/views/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21853 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_invenio_github.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3693 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_webhook.py
```

### Comparing `invenio-github-1.0.0b2/.editorconfig` & `invenio-github-1.0.0b3/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/.tx/config` & `invenio-github-1.0.0b3/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/AUTHORS.rst` & `invenio-github-1.0.0b3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/CHANGES.rst` & `invenio-github-1.0.0b3/docs/contributing.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ..
     This file is part of Invenio.
-    Copyright (C) 2016-2022 CERN.
+    Copyright (C) 2016 CERN.
 
     Invenio is free software; you can redistribute it
     and/or modify it under the terms of the GNU General Public License as
     published by the Free Software Foundation; either version 2 of the
     License, or (at your option) any later version.
 
     Invenio is distributed in the hope that it will be
@@ -18,23 +18,8 @@
     MA 02111-1307, USA.
 
     In applying this license, CERN does not
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
-Changes
-=======
-
-Version v1.0.0b2 (released 2023-07-17)
-
-- global: restrain extension behind feature flag
-- api: add record serialization
-- handlers: fix hooks serialization
-
-Version v1.0.0b1 (released 2023-07-03)
-
-- Initial beta release.
-
-Version v1.0.0a28 (released 2022-10-24)
-
-- Initial public release.
+.. include:: ../CONTRIBUTING.rst
```

### Comparing `invenio-github-1.0.0b2/CONTRIBUTING.rst` & `invenio-github-1.0.0b3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/LICENSE` & `invenio-github-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/MANIFEST.in` & `invenio-github-1.0.0b3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/PKG-INFO` & `invenio-github-1.0.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,18 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.0b3 (released 2023-07-17)
+        
+        - alembic: add alembic recipes
+        
         Version v1.0.0b2 (released 2023-07-17)
         
         - global: restrain extension behind feature flag
         - api: add record serialization
         - handlers: fix hooks serialization
         
         Version v1.0.0b1 (released 2023-07-03)
```

### Comparing `invenio-github-1.0.0b2/README.rst` & `invenio-github-1.0.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/RELEASE-NOTES.rst` & `invenio-github-1.0.0b3/RELEASE-NOTES.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/babel.ini` & `invenio-github-1.0.0b3/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/docs/Makefile` & `invenio-github-1.0.0b3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/docs/api.rst` & `invenio-github-1.0.0b3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/docs/authors.rst` & `invenio-github-1.0.0b3/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/docs/changes.rst` & `invenio-github-1.0.0b3/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/docs/conf.py` & `invenio-github-1.0.0b3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/docs/contributing.rst` & `invenio-github-1.0.0b3/docs/usage.rst`

 * *Files 4% similar despite different names*

```diff
@@ -18,8 +18,11 @@
     MA 02111-1307, USA.
 
     In applying this license, CERN does not
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
-.. include:: ../CONTRIBUTING.rst
+Usage
+=====
+
+.. automodule:: invenio_github
```

### Comparing `invenio-github-1.0.0b2/docs/index.rst` & `invenio-github-1.0.0b3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/docs/installation.rst` & `invenio-github-1.0.0b3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/docs/license.rst` & `invenio-github-1.0.0b3/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/docs/make.bat` & `invenio-github-1.0.0b3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/docs/usage.rst` & `invenio-github-1.0.0b3/requirements-devel.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-..
-    This file is part of Invenio.
-    Copyright (C) 2016 CERN.
-
-    Invenio is free software; you can redistribute it
-    and/or modify it under the terms of the GNU General Public License as
-    published by the Free Software Foundation; either version 2 of the
-    License, or (at your option) any later version.
-
-    Invenio is distributed in the hope that it will be
-    useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-    General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with Invenio; if not, write to the
-    Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
-    MA 02111-1307, USA.
-
-    In applying this license, CERN does not
-    waive the privileges and immunities granted to it by virtue of its status
-    as an Intergovernmental Organization or submit itself to any jurisdiction.
-
-
-Usage
-=====
-
-.. automodule:: invenio_github
+# -*- coding: utf-8 -*-
+#
+# This file is part of Invenio.
+# Copyright (C) 2016 CERN.
+#
+# Invenio is free software; you can redistribute it
+# and/or modify it under the terms of the GNU General Public License as
+# published by the Free Software Foundation; either version 2 of the
+# License, or (at your option) any later version.
+#
+# Invenio is distributed in the hope that it will be
+# useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with Invenio; if not, write to the
+# Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
+# MA 02111-1307, USA.
+#
+# In applying this license, CERN does not
+# waive the privileges and immunities granted to it by virtue of its status
+# as an Intergovernmental Organization or submit itself to any jurisdiction.
```

### Comparing `invenio-github-1.0.0b2/invenio_github/__init__.py` & `invenio-github-1.0.0b3/invenio_github/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
 from .ext import InvenioGitHub
 
-__version__ = "1.0.0b2"
+__version__ = "1.0.0b3"
 
 __all__ = ("__version__", "InvenioGitHub")
```

### Comparing `invenio-github-1.0.0b2/invenio_github/api.py` & `invenio-github-1.0.0b3/invenio_github/api.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/assets/semantic-ui/js/invenio_github/index.js` & `invenio-github-1.0.0b3/invenio_github/assets/semantic-ui/js/invenio_github/index.js`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/config.py` & `invenio-github-1.0.0b3/invenio_github/config.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/errors.py` & `invenio-github-1.0.0b3/invenio_github/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/ext.py` & `invenio-github-1.0.0b3/invenio_github/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/models.py` & `invenio-github-1.0.0b3/invenio_github/models.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/proxies.py` & `invenio-github-1.0.0b3/invenio_github/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/receivers.py` & `invenio-github-1.0.0b3/invenio_github/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/tasks.py` & `invenio-github-1.0.0b3/invenio_github/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/helpers.html` & `invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html` & `invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/index.html` & `invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html` & `invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/templates/semantic-ui/invenio_github/settings/view.html` & `invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/view.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/translations/cs/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b3/invenio_github/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/translations/da/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b3/invenio_github/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/translations/de/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b3/invenio_github/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/translations/en/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b3/invenio_github/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/translations/es/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b3/invenio_github/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/translations/fr/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b3/invenio_github/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/translations/it/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b3/invenio_github/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/translations/messages.pot` & `invenio-github-1.0.0b3/invenio_github/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/utils.py` & `invenio-github-1.0.0b3/invenio_github/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/views/__init__.py` & `invenio-github-1.0.0b3/invenio_github/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/views/badge.py` & `invenio-github-1.0.0b3/invenio_github/views/badge.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/views/github.py` & `invenio-github-1.0.0b3/invenio_github/views/github.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github/webpack.py` & `invenio-github-1.0.0b3/invenio_github/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/invenio_github.egg-info/PKG-INFO` & `invenio-github-1.0.0b3/invenio_github.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,18 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.0b3 (released 2023-07-17)
+        
+        - alembic: add alembic recipes
+        
         Version v1.0.0b2 (released 2023-07-17)
         
         - global: restrain extension behind feature flag
         - api: add record serialization
         - handlers: fix hooks serialization
         
         Version v1.0.0b1 (released 2023-07-03)
```

### Comparing `invenio-github-1.0.0b2/invenio_github.egg-info/SOURCES.txt` & `invenio-github-1.0.0b3/invenio_github.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 invenio_github/translations/it/LC_MESSAGES/messages.po
 invenio_github/views/__init__.py
 invenio_github/views/badge.py
 invenio_github/views/github.py
 tests/__init__.py
 tests/conftest.py
 tests/fixtures.py
+tests/test_alembic.py
 tests/test_api.py
 tests/test_badge.py
 tests/test_invenio_github.py
 tests/test_models.py
 tests/test_tasks.py
 tests/test_views.py
 tests/test_webhook.py
```

### Comparing `invenio-github-1.0.0b2/invenio_github.egg-info/entry_points.txt` & `invenio-github-1.0.0b3/invenio_github.egg-info/entry_points.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 [invenio_base.blueprints]
 invenio_github_badge = invenio_github.views.badge:blueprint
 invenio_github_github = invenio_github.views.github:create_ui_blueprint
 
 [invenio_celery.tasks]
 invenio_github = invenio_github.tasks
 
+[invenio_db.alembic]
+invenio_github = invenio_github:alembic
+
 [invenio_db.models]
 invenio_github = invenio_github.models
 
 [invenio_i18n.translations]
 messages = invenio_github
 
 [invenio_webhooks.receivers]
```

### Comparing `invenio-github-1.0.0b2/invenio_github.egg-info/requires.txt` & `invenio-github-1.0.0b3/invenio_github.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/requirements-devel.txt` & `invenio-github-1.0.0b3/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+#!/usr/bin/env sh
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -17,7 +18,9 @@
 # along with Invenio; if not, write to the
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
+
+"""Unit test for Invenio-Github."""
```

### Comparing `invenio-github-1.0.0b2/run-tests.sh` & `invenio-github-1.0.0b3/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/setup.cfg` & `invenio-github-1.0.0b3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 invenio_base.blueprints = 
 	invenio_github_badge = invenio_github.views.badge:blueprint
 	invenio_github_github = invenio_github.views.github:create_ui_blueprint
 invenio_base.api_blueprints = 
 	invenio_github = invenio_github.views.github:create_api_blueprint
 invenio_celery.tasks = 
 	invenio_github = invenio_github.tasks
+invenio_db.alembic = 
+	invenio_github = invenio_github:alembic
 invenio_db.models = 
 	invenio_github = invenio_github.models
 invenio_i18n.translations = 
 	messages = invenio_github
 invenio_webhooks.receivers = 
 	github = invenio_github.receivers:GitHubReceiver
 invenio_assets.webpack =
```

### Comparing `invenio-github-1.0.0b2/setup.py` & `invenio-github-1.0.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/tests/conftest.py` & `invenio-github-1.0.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/tests/fixtures.py` & `invenio-github-1.0.0b3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/tests/test_api.py` & `invenio-github-1.0.0b3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/tests/test_badge.py` & `invenio-github-1.0.0b3/tests/test_badge.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/tests/test_invenio_github.py` & `invenio-github-1.0.0b3/tests/test_invenio_github.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/tests/test_models.py` & `invenio-github-1.0.0b3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/tests/test_tasks.py` & `invenio-github-1.0.0b3/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/tests/test_views.py` & `invenio-github-1.0.0b3/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b2/tests/test_webhook.py` & `invenio-github-1.0.0b3/tests/test_webhook.py`

 * *Files identical despite different names*

