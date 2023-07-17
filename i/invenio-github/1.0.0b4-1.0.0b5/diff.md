# Comparing `tmp/invenio-github-1.0.0b4.tar.gz` & `tmp/invenio-github-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-github-1.0.0b4.tar", last modified: Mon Jul 17 12:53:52 2023, max compression
+gzip compressed data, was "dist/invenio-github-1.0.0b5.tar", last modified: Mon Jul 17 20:35:00 2023, max compression
```

## Comparing `invenio-github-1.0.0b4.tar` & `invenio-github-1.0.0b5.tar`

### file list

```diff
@@ -1,113 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/.lgtm
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/RELEASE-NOTES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/babel.ini
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10752 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22856 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/assets/semantic-ui/js/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/assets/semantic-ui/js/invenio_github/index.js
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/receivers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/helpers.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (122)     6503 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
--rw-r--r--   0 runner    (1001) docker     (122)    15043 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github/views/
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/views/badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     8193 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/views/github.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/invenio_github/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/invenio_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-17 12:53:51.000000 invenio-github-1.0.0b4/invenio_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:53:52.000000 invenio-github-1.0.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    21853 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_alembic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_invenio_github.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     3693 2023-07-17 12:53:42.000000 invenio-github-1.0.0b4/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2509 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/.lgtm
+-rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1549 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/RELEASE-NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10770 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/alembic/5a5428312b2b_create_github_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/alembic/b0eaee37b545_create_github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22856 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/assets/semantic-ui/js/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/assets/semantic-ui/js/invenio_github/index.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/oauth/
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/oauth/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/oauth/remote_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/helpers.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6503 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
+-rw-r--r--   0 runner    (1001) docker     (122)    15043 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/views/badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8193 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/views/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/invenio_github/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/invenio_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      347 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-07-17 20:35:00.000000 invenio-github-1.0.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-17 20:34:54.000000 invenio-github-1.0.0b5/setup.py
```

### Comparing `invenio-github-1.0.0b4/.editorconfig` & `invenio-github-1.0.0b5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -18,32 +19,12 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
+"""Invenio module that adds GitHub integration to the platform."""
 
-root = true
+from setuptools import setup
 
-[*]
-indent_style = space
-end_of_line = lf
-insert_final_newline = true
-trim_trailing_whitespace = true
-charset = utf-8
-
-# RST files (used by sphinx)
-[*.rst]
-indent_size = 4
-
-# CSS, HTML, JS, JSON, YML
-[*.{css,html,js,json,yml}]
-indent_size = 2
-
-# Matches the exact files either package.json or .travis.yml
-[{package.json,.travis.yml}]
-indent_size = 2
-
-# Dockerfile
-[Dockerfile]
-indent_size = 4
+setup()
```

### Comparing `invenio-github-1.0.0b4/AUTHORS.rst` & `invenio-github-1.0.0b5/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/CHANGES.rst` & `invenio-github-1.0.0b5/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,19 @@
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
 Changes
 =======
 
+Version v1.0.0b5 (released 2023-07-17)
+
+- setup: enable tests
+- setup: update Manifest.in
+
 Version v1.0.0b4 (released 2023-07-17)
 
 - alembic: add webhook dependency in alembic recipes
 
 Version v1.0.0b3 (released 2023-07-17)
 
 - alembic: add alembic recipes
```

### Comparing `invenio-github-1.0.0b4/CONTRIBUTING.rst` & `invenio-github-1.0.0b5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/LICENSE` & `invenio-github-1.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/MANIFEST.in` & `invenio-github-1.0.0b5/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -19,33 +19,40 @@
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
-include *.rst
-include *.sh
+exclude .dockerignore
+exclude .editorconfig
+exclude .tx/config
+exclude pytest.ini
 include *.txt
-include .dockerignore
-include .editorconfig
-include .tx/config
-include .lgtm
-include LICENSE
 include MAINTAINERS
+include *.rst
 include babel.ini
-include docs/requirements.txt
-include pytest.ini
+include .lgtm
+include LICENSE
+include .prettierrc
+include *.yml
+include run-js-linter.sh
+include run-tests.sh
+include run-i18n-tests.sh
+prune docs/_build
+prune docs/_build
+prune tests
+recursive-include .github/workflows *.yml
 recursive-include docs *.bat
 recursive-include docs *.py
 recursive-include docs *.rst
+recursive-include docs *.txt
 recursive-include docs Makefile
-recursive-include examples *.py
-recursive-include invenio_github *.css
 recursive-include invenio_github *.html
 recursive-include invenio_github *.js
-recursive-include invenio_github *.png
-recursive-include invenio_github *.po *.pot *.mo
-recursive-include invenio_github *.scss
-recursive-include invenio_github *.ttf
-recursive-include tests *.py
+recursive-include invenio_github *.json
+recursive-include invenio_github *.less
+recursive-include invenio_github *.mo
+recursive-include invenio_github *.po
+recursive-include invenio_github *.pot
+recursive-include invenio_github *.py
 include .git-blame-ignore-revs
```

### Comparing `invenio-github-1.0.0b4/PKG-INFO` & `invenio-github-1.0.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,19 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.0b5 (released 2023-07-17)
+        
+        - setup: enable tests
+        - setup: update Manifest.in
+        
         Version v1.0.0b4 (released 2023-07-17)
         
         - alembic: add webhook dependency in alembic recipes
         
         Version v1.0.0b3 (released 2023-07-17)
         
         - alembic: add alembic recipes
@@ -105,12 +110,11 @@
         
         - Initial public release.
         
 Keywords: invenio github
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
-Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: elasticsearch7
 Provides-Extra: opensearch1
 Provides-Extra: opensearch2
```

### Comparing `invenio-github-1.0.0b4/README.rst` & `invenio-github-1.0.0b5/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/RELEASE-NOTES.rst` & `invenio-github-1.0.0b5/RELEASE-NOTES.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/babel.ini` & `invenio-github-1.0.0b5/invenio_github/proxies.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
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
@@ -18,23 +18,13 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
-# Extraction from Python source files
+"""Proxy for current previewer."""
 
-[python: **.py]
-encoding = utf-8
+from flask import current_app
+from werkzeug.local import LocalProxy
 
-# Extraction from Jinja2 templates
-
-[jinja2: **/templates/**.html]
-encoding = utf-8
-extensions = jinja2.ext.autoescape, jinja2.ext.with_
-
-# Extraction from JavaScript files
-
-[javascript: **.js]
-encoding = utf-8
-extract_messages = $._, jQuery._
+current_github = LocalProxy(lambda: current_app.extensions["invenio-github"])
```

### Comparing `invenio-github-1.0.0b4/docs/Makefile` & `invenio-github-1.0.0b5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/docs/api.rst` & `invenio-github-1.0.0b5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/docs/authors.rst` & `invenio-github-1.0.0b5/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/docs/changes.rst` & `invenio-github-1.0.0b5/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/docs/conf.py` & `invenio-github-1.0.0b5/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,11 +324,12 @@
 # texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {"https://docs.python.org/": None}
-
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/", None),
+}
 # Autodoc configuraton.
 autoclass_content = "both"
```

### Comparing `invenio-github-1.0.0b4/docs/contributing.rst` & `invenio-github-1.0.0b5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/docs/index.rst` & `invenio-github-1.0.0b5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/docs/installation.rst` & `invenio-github-1.0.0b5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/docs/license.rst` & `invenio-github-1.0.0b5/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/docs/make.bat` & `invenio-github-1.0.0b5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/docs/usage.rst` & `invenio-github-1.0.0b5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/__init__.py` & `invenio-github-1.0.0b5/invenio_github/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
 from .ext import InvenioGitHub
 
-__version__ = "1.0.0b4"
+__version__ = "1.0.0b5"
 
 __all__ = ("__version__", "InvenioGitHub")
```

### Comparing `invenio-github-1.0.0b4/invenio_github/api.py` & `invenio-github-1.0.0b5/invenio_github/api.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/assets/semantic-ui/js/invenio_github/index.js` & `invenio-github-1.0.0b5/invenio_github/assets/semantic-ui/js/invenio_github/index.js`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/config.py` & `invenio-github-1.0.0b5/invenio_github/config.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/errors.py` & `invenio-github-1.0.0b5/invenio_github/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/ext.py` & `invenio-github-1.0.0b5/invenio_github/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/models.py` & `invenio-github-1.0.0b5/invenio_github/models.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/proxies.py` & `invenio-github-1.0.0b5/requirements-devel.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2023 CERN.
+# Copyright (C) 2016 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -17,14 +17,7 @@
 # along with Invenio; if not, write to the
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
-
-"""Proxy for current previewer."""
-
-from flask import current_app
-from werkzeug.local import LocalProxy
-
-current_github = LocalProxy(lambda: current_app.extensions["invenio-github"])
```

### Comparing `invenio-github-1.0.0b4/invenio_github/receivers.py` & `invenio-github-1.0.0b5/invenio_github/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/tasks.py` & `invenio-github-1.0.0b5/invenio_github/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/helpers.html` & `invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html` & `invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/index.html` & `invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html` & `invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/templates/semantic-ui/invenio_github/settings/view.html` & `invenio-github-1.0.0b5/invenio_github/templates/semantic-ui/invenio_github/settings/view.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/translations/cs/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b5/invenio_github/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/translations/da/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b5/invenio_github/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/translations/de/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b5/invenio_github/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/translations/en/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b5/invenio_github/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/translations/es/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b5/invenio_github/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/translations/fr/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b5/invenio_github/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/translations/it/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b5/invenio_github/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/translations/messages.pot` & `invenio-github-1.0.0b5/invenio_github/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/utils.py` & `invenio-github-1.0.0b5/invenio_github/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/views/__init__.py` & `invenio-github-1.0.0b5/invenio_github/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/views/badge.py` & `invenio-github-1.0.0b5/invenio_github/views/badge.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/views/github.py` & `invenio-github-1.0.0b5/invenio_github/views/github.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github/webpack.py` & `invenio-github-1.0.0b5/invenio_github/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github.egg-info/PKG-INFO` & `invenio-github-1.0.0b5/invenio_github.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,19 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.0b5 (released 2023-07-17)
+        
+        - setup: enable tests
+        - setup: update Manifest.in
+        
         Version v1.0.0b4 (released 2023-07-17)
         
         - alembic: add webhook dependency in alembic recipes
         
         Version v1.0.0b3 (released 2023-07-17)
         
         - alembic: add alembic recipes
@@ -105,12 +110,11 @@
         
         - Initial public release.
         
 Keywords: invenio github
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
-Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: elasticsearch7
 Provides-Extra: opensearch1
 Provides-Extra: opensearch2
```

### Comparing `invenio-github-1.0.0b4/invenio_github.egg-info/SOURCES.txt` & `invenio-github-1.0.0b5/invenio_github.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-.dockerignore
-.editorconfig
 .git-blame-ignore-revs
 .lgtm
+.travis.yml
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MAINTAINERS
 MANIFEST.in
 README.rst
 RELEASE-NOTES.rst
 babel.ini
 constraints-pypi.txt
 pyproject.toml
 requirements-devel.txt
+run-i18n-tests.sh
 run-tests.sh
 setup.cfg
 setup.py
-.tx/config
+.github/workflows/pypi-publish.yml
+.github/workflows/tests.yml
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changes.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
@@ -45,15 +46,19 @@
 invenio_github.egg-info/PKG-INFO
 invenio_github.egg-info/SOURCES.txt
 invenio_github.egg-info/dependency_links.txt
 invenio_github.egg-info/entry_points.txt
 invenio_github.egg-info/not-zip-safe
 invenio_github.egg-info/requires.txt
 invenio_github.egg-info/top_level.txt
+invenio_github/alembic/5a5428312b2b_create_github_branch.py
+invenio_github/alembic/b0eaee37b545_create_github_tables.py
 invenio_github/assets/semantic-ui/js/invenio_github/index.js
+invenio_github/oauth/handlers.py
+invenio_github/oauth/remote_app.py
 invenio_github/templates/semantic-ui/invenio_github/base.html
 invenio_github/templates/semantic-ui/invenio_github/helpers.html
 invenio_github/templates/semantic-ui/invenio_github/settings/base.html
 invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
 invenio_github/templates/semantic-ui/invenio_github/settings/index.html
 invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
 invenio_github/templates/semantic-ui/invenio_github/settings/view.html
@@ -64,19 +69,8 @@
 invenio_github/translations/en/LC_MESSAGES/messages.mo
 invenio_github/translations/en/LC_MESSAGES/messages.po
 invenio_github/translations/es/LC_MESSAGES/messages.po
 invenio_github/translations/fr/LC_MESSAGES/messages.po
 invenio_github/translations/it/LC_MESSAGES/messages.po
 invenio_github/views/__init__.py
 invenio_github/views/badge.py
-invenio_github/views/github.py
-tests/__init__.py
-tests/conftest.py
-tests/fixtures.py
-tests/test_alembic.py
-tests/test_api.py
-tests/test_badge.py
-tests/test_invenio_github.py
-tests/test_models.py
-tests/test_tasks.py
-tests/test_views.py
-tests/test_webhook.py
+invenio_github/views/github.py
```

### Comparing `invenio-github-1.0.0b4/invenio_github.egg-info/entry_points.txt` & `invenio-github-1.0.0b5/invenio_github.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/invenio_github.egg-info/requires.txt` & `invenio-github-1.0.0b5/invenio_github.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,30 +18,28 @@
 invenio-records-resources>=4.2.0
 mistune>=0.7.2
 six>=1.12.0
 uritemplate.py<2.0,>=0.2.0
 Flask<2.3.0,>=2.2.0
 PyYAML>=5.4.1
 
-[docs]
-Sphinx>=1.4.2
-
 [elasticsearch7]
 invenio-search[elasticsearch7]<3.0.0,>=2.1.0
 
 [opensearch1]
 invenio-search[opensearch1]<3.0.0,>=2.1.0
 
 [opensearch2]
 invenio-search[opensearch2]<3.0.0,>=2.1.0
 
 [tests]
-mock>=2.0.0
 httpretty>=0.8.14
-pytest-black>=0.3.0
+invenio-app>=1.3.4
+invenio-db[mysql,postgresql]<2.0.0,>=1.1.2
 invenio-files-rest<1.5.0,>=1.0.0a12
 isort>=4.2.2
-pytest-mock>=2.0.0
-pytest-invenio<3.0.0,>=2.1.0
+mock>=2.0.0
 pluggy<1.0,>=0.12
+pytest-black>=0.3.0
+pytest-invenio<3.0.0,>=2.1.0
+pytest-mock>=2.0.0
 sphinx>=4.5.0
-invenio-app>=1.3.4
```

### Comparing `invenio-github-1.0.0b4/run-tests.sh` & `invenio-github-1.0.0b5/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b4/setup.cfg` & `invenio-github-1.0.0b5/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -39,27 +39,26 @@
 	mistune>=0.7.2
 	six>=1.12.0
 	uritemplate.py>=0.2.0,<2.0
 	Flask>=2.2.0,<2.3.0
 	PyYAML>=5.4.1
 
 [options.extras_require]
-docs = 
-	Sphinx>=1.4.2
 tests = 
-	mock>=2.0.0
 	httpretty>=0.8.14
-	pytest-black>=0.3.0
+	invenio-app>=1.3.4
+	invenio-db[postgresql,mysql]>=1.1.2,<2.0.0
 	invenio-files-rest>=1.0.0a12,<1.5.0
 	isort>=4.2.2
-	pytest-mock>=2.0.0
-	pytest-invenio>=2.1.0,<3.0.0
+	mock>=2.0.0
 	pluggy>=0.12,<1.0
+	pytest-black>=0.3.0
+	pytest-invenio>=2.1.0,<3.0.0
+	pytest-mock>=2.0.0
 	sphinx>=4.5.0
-	invenio-app>=1.3.4
 elasticsearch7 = 
 	invenio-search[elasticsearch7]>=2.1.0,<3.0.0
 opensearch1 = 
 	invenio-search[opensearch1]>=2.1.0,<3.0.0
 opensearch2 = 
 	invenio-search[opensearch2]>=2.1.0,<3.0.0
```

