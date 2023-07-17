# Comparing `tmp/invenio-github-1.0.0b3.tar.gz` & `tmp/invenio-github-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-github-1.0.0b3.tar", last modified: Mon Jul 17 12:38:00 2023, max compression
+gzip compressed data, was "dist/invenio-github-1.0.0b4.tar", last modified: Mon Jul 17 12:53:52 2023, max compression
```

## Comparing `invenio-github-1.0.0b3.tar` & `invenio-github-1.0.0b4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/.lgtm
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/RELEASE-NOTES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/babel.ini
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10752 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22856 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/assets/semantic-ui/js/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/assets/semantic-ui/js/invenio_github/index.js
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/receivers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/helpers.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (122)     6503 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
--rw-r--r--   0 runner    (1001) docker     (122)    15043 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github/views/
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/views/badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     8193 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/views/github.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/invenio_github/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/invenio_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-17 12:37:59.000000 invenio-github-1.0.0b3/invenio_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:38:00.000000 invenio-github-1.0.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    21853 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_alembic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_invenio_github.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     3693 2023-07-17 12:37:52.000000 invenio-github-1.0.0b3/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/.lgtm
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/RELEASE-NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10752 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22856 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/assets/semantic-ui/js/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/assets/semantic-ui/js/invenio_github/index.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/helpers.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6503 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
+-rw-r--r--   0 runner    (1001) docker     (122)    15043 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/views/badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8193 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/views/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21853 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_invenio_github.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3693 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_webhook.py
```

### Comparing `invenio-github-1.0.0b3/.editorconfig` & `invenio-github-1.0.0b4/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/.tx/config` & `invenio-github-1.0.0b4/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/AUTHORS.rst` & `invenio-github-1.0.0b4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/CHANGES.rst` & `invenio-github-1.0.0b4/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
 Changes
 =======
 
+Version v1.0.0b4 (released 2023-07-17)
+
+- alembic: add webhook dependency in alembic recipes
+
 Version v1.0.0b3 (released 2023-07-17)
 
 - alembic: add alembic recipes
 
 Version v1.0.0b2 (released 2023-07-17)
 
 - global: restrain extension behind feature flag
```

### Comparing `invenio-github-1.0.0b3/CONTRIBUTING.rst` & `invenio-github-1.0.0b4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/LICENSE` & `invenio-github-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/MANIFEST.in` & `invenio-github-1.0.0b4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/PKG-INFO` & `invenio-github-1.0.0b4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b3
+Version: 1.0.0b4
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
         
+        Version v1.0.0b4 (released 2023-07-17)
+        
+        - alembic: add webhook dependency in alembic recipes
+        
         Version v1.0.0b3 (released 2023-07-17)
         
         - alembic: add alembic recipes
         
         Version v1.0.0b2 (released 2023-07-17)
         
         - global: restrain extension behind feature flag
```

### Comparing `invenio-github-1.0.0b3/README.rst` & `invenio-github-1.0.0b4/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/RELEASE-NOTES.rst` & `invenio-github-1.0.0b4/RELEASE-NOTES.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/babel.ini` & `invenio-github-1.0.0b4/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/Makefile` & `invenio-github-1.0.0b4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/api.rst` & `invenio-github-1.0.0b4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/authors.rst` & `invenio-github-1.0.0b4/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/changes.rst` & `invenio-github-1.0.0b4/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/conf.py` & `invenio-github-1.0.0b4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/contributing.rst` & `invenio-github-1.0.0b4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/index.rst` & `invenio-github-1.0.0b4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/installation.rst` & `invenio-github-1.0.0b4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/license.rst` & `invenio-github-1.0.0b4/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/make.bat` & `invenio-github-1.0.0b4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/docs/usage.rst` & `invenio-github-1.0.0b4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/__init__.py` & `invenio-github-1.0.0b4/invenio_github/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
 from .ext import InvenioGitHub
 
-__version__ = "1.0.0b3"
+__version__ = "1.0.0b4"
 
 __all__ = ("__version__", "InvenioGitHub")
```

### Comparing `invenio-github-1.0.0b3/invenio_github/api.py` & `invenio-github-1.0.0b4/invenio_github/api.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/assets/semantic-ui/js/invenio_github/index.js` & `invenio-github-1.0.0b4/invenio_github/assets/semantic-ui/js/invenio_github/index.js`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/config.py` & `invenio-github-1.0.0b4/invenio_github/config.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/errors.py` & `invenio-github-1.0.0b4/invenio_github/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/ext.py` & `invenio-github-1.0.0b4/invenio_github/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/models.py` & `invenio-github-1.0.0b4/invenio_github/models.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/proxies.py` & `invenio-github-1.0.0b4/invenio_github/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/receivers.py` & `invenio-github-1.0.0b4/invenio_github/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/tasks.py` & `invenio-github-1.0.0b4/invenio_github/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/helpers.html` & `invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html` & `invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/index.html` & `invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html` & `invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/templates/semantic-ui/invenio_github/settings/view.html` & `invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/view.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/translations/cs/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b4/invenio_github/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/translations/da/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b4/invenio_github/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/translations/de/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b4/invenio_github/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/translations/en/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b4/invenio_github/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/translations/es/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b4/invenio_github/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/translations/fr/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b4/invenio_github/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/translations/it/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b4/invenio_github/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/translations/messages.pot` & `invenio-github-1.0.0b4/invenio_github/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/utils.py` & `invenio-github-1.0.0b4/invenio_github/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/views/__init__.py` & `invenio-github-1.0.0b4/invenio_github/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/views/badge.py` & `invenio-github-1.0.0b4/invenio_github/views/badge.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/views/github.py` & `invenio-github-1.0.0b4/invenio_github/views/github.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github/webpack.py` & `invenio-github-1.0.0b4/invenio_github/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github.egg-info/PKG-INFO` & `invenio-github-1.0.0b4/invenio_github.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b3
+Version: 1.0.0b4
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
         
+        Version v1.0.0b4 (released 2023-07-17)
+        
+        - alembic: add webhook dependency in alembic recipes
+        
         Version v1.0.0b3 (released 2023-07-17)
         
         - alembic: add alembic recipes
         
         Version v1.0.0b2 (released 2023-07-17)
         
         - global: restrain extension behind feature flag
```

### Comparing `invenio-github-1.0.0b3/invenio_github.egg-info/SOURCES.txt` & `invenio-github-1.0.0b4/invenio_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github.egg-info/entry_points.txt` & `invenio-github-1.0.0b4/invenio_github.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/invenio_github.egg-info/requires.txt` & `invenio-github-1.0.0b4/invenio_github.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/requirements-devel.txt` & `invenio-github-1.0.0b4/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/run-tests.sh` & `invenio-github-1.0.0b4/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/setup.cfg` & `invenio-github-1.0.0b4/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/setup.py` & `invenio-github-1.0.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/__init__.py` & `invenio-github-1.0.0b4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/conftest.py` & `invenio-github-1.0.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/fixtures.py` & `invenio-github-1.0.0b4/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/test_alembic.py` & `invenio-github-1.0.0b4/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/test_api.py` & `invenio-github-1.0.0b4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/test_badge.py` & `invenio-github-1.0.0b4/tests/test_badge.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/test_invenio_github.py` & `invenio-github-1.0.0b4/tests/test_invenio_github.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/test_models.py` & `invenio-github-1.0.0b4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/test_tasks.py` & `invenio-github-1.0.0b4/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/test_views.py` & `invenio-github-1.0.0b4/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b3/tests/test_webhook.py` & `invenio-github-1.0.0b4/tests/test_webhook.py`

 * *Files identical despite different names*

