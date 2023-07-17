# Comparing `tmp/invenio-formatter-1.2.0.tar.gz` & `tmp/invenio-formatter-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-formatter-1.2.0.tar", last modified: Tue Feb 28 12:22:09 2023, max compression
+gzip compressed data, was "dist/invenio-formatter-1.3.0.tar", last modified: Mon Jul 17 09:09:54 2023, max compression
```

## Comparing `invenio-formatter-1.2.0.tar` & `invenio-formatter-1.3.0.tar`

### file list

```diff
@@ -1,217 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      803 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7453 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10113 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/examplesapp.rst
--rw-r--r--   0 runner    (1001) docker     (122)      845 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/examples/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/examples/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/examples/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/context_processors/
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/context_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/context_processors/badges.py
--rw-r--r--   0 runner    (1001) docker     (122)     2377 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/filters/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/filters/html.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/templates/invenio_formatter/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/templates/invenio_formatter/macros/
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/templates/invenio_formatter/macros/badges.html
--rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/templates/invenio_formatter/macros/meta.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/templates/semantic-ui/invenio_formatter/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html
--rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      464 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      534 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1632 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1616 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1748 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      651 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1760 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      777 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/invenio_formatter/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5608 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/invenio_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-02-28 12:22:08.000000 invenio-formatter-1.2.0/invenio_formatter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      577 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 12:22:09.000000 invenio-formatter-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/tests/test_examples_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/tests/test_invenio_formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/tests/test_template_context_processors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/tests/test_template_macros.py
--rw-r--r--   0 runner    (1001) docker     (122)     3234 2023-02-28 12:22:04.000000 invenio-formatter-1.2.0/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7453 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10113 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/examplesapp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      845 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/examples/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/examples/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/examples/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/context_processors/
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/context_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/context_processors/badges.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/filters/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/filters/html.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/templates/invenio_formatter/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/templates/invenio_formatter/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/templates/invenio_formatter/macros/badges.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/templates/invenio_formatter/macros/meta.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/templates/semantic-ui/invenio_formatter/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1632 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1616 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1748 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1760 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/invenio_formatter/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7310 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/invenio_formatter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      577 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 09:09:54.000000 invenio-formatter-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/tests/test_examples_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/tests/test_invenio_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/tests/test_template_context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/tests/test_template_macros.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3234 2023-07-17 09:09:48.000000 invenio-formatter-1.3.0/tests/test_views.py
```

### Comparing `invenio-formatter-1.2.0/.editorconfig` & `invenio-formatter-1.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/.github/workflows/pypi-publish.yml` & `invenio-formatter-1.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/.github/workflows/tests.yml` & `invenio-formatter-1.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/.tx/config` & `invenio-formatter-1.3.0/.tx/config`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
+# Copyright (C)      2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 
 # 1) Create message catalog:
 #    $ python setup.py extract_messages
@@ -19,14 +20,14 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio-formatter-messages]
+[o:inveniosoftware:p:invenio:r:invenio-formatter-messages]
 file_filter = invenio_formatter/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_formatter/translations/messages.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-formatter-1.2.0/CHANGES.rst` & `invenio-formatter-1.3.0/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.3.0 (released 2023-07-17)
+
+- add template filter for human readable time
+
 Version 1.2.0 (released 2021-02-28)
 
 - remove flask-babelex deprecated dependency
 - upgrade invenio-i18n to manage babel globally
 
 Version 1.1.4 (released 2021-10-18)
```

### Comparing `invenio-formatter-1.2.0/CONTRIBUTING.rst` & `invenio-formatter-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/INSTALL.rst` & `invenio-formatter-1.3.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/LICENSE` & `invenio-formatter-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/MANIFEST.in` & `invenio-formatter-1.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/PKG-INFO` & `invenio-formatter-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-formatter
-Version: 1.2.0
+Version: 1.3.0
 Summary: "Jinja utilities for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-formatter
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.3.0 (released 2023-07-17)
+        
+        - add template filter for human readable time
+        
         Version 1.2.0 (released 2021-02-28)
         
         - remove flask-babelex deprecated dependency
         - upgrade invenio-i18n to manage babel globally
         
         Version 1.1.4 (released 2021-10-18)
```

### Comparing `invenio-formatter-1.2.0/README.rst` & `invenio-formatter-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/docs/Makefile` & `invenio-formatter-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/docs/api.rst` & `invenio-formatter-1.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/docs/conf.py` & `invenio-formatter-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/docs/index.rst` & `invenio-formatter-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/docs/make.bat` & `invenio-formatter-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/examples/app.py` & `invenio-formatter-1.3.0/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter/__init__.py` & `invenio-formatter-1.3.0/invenio_formatter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,10 +66,10 @@
 <http://localhost:5000/badge/ISBN/9780399547331.svg>`_.
 """
 
 from __future__ import absolute_import, print_function
 
 from .ext import InvenioFormatter
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 __all__ = ("__version__", "InvenioFormatter")
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/config.py` & `invenio-formatter-1.3.0/invenio_formatter/config.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter/context_processors/badges.py` & `invenio-formatter-1.3.0/invenio_formatter/context_processors/badges.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter/ext.py` & `invenio-formatter-1.3.0/invenio_formatter/ext.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 """Jinja utilities for Invenio."""
 
 from __future__ import absolute_import, print_function
 
 from pkg_resources import DistributionNotFound, get_distribution
 
 from . import config
-from .filters.datetime import format_arrow, from_isodate, from_isodatetime, to_arrow
+from .filters.datetime import (
+    format_arrow,
+    from_isodate,
+    from_isodatetime,
+    naturaltime,
+    to_arrow,
+)
 from .filters.html import sanitize_html
 from .views import create_badge_blueprint
 
 
 class InvenioFormatter(object):
     """Invenio-Formatter extension."""
 
@@ -39,14 +45,15 @@
         # Install datetime helpers.
         app.jinja_env.filters.update(
             from_isodate=from_isodate,
             from_isodatetime=from_isodatetime,
             to_arrow=to_arrow,
             format_arrow=format_arrow,
             sanitize_html=sanitize_html,
+            naturaltime=naturaltime,
         )
 
         if app.config["FORMATTER_BADGES_ENABLE"]:
             from invenio_formatter.context_processors.badges import badges_processor
 
             # Registration of context processors.
             app.context_processor(badges_processor)
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/filters/datetime.py` & `invenio-formatter-1.3.0/invenio_formatter/filters/datetime.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Datetime Jinja filters."""
 
 from __future__ import absolute_import, print_function
 
 import arrow
+from flask_babel import to_user_timezone
 
 
 def from_isodate(value, strict=False):
     """Convert an ISO formatted date into a Date object.
 
     :param value: The ISO formatted date.
     :param strict: If value is ``None``, then if strict is ``True`` it returns
@@ -55,7 +56,15 @@
     assert isinstance(value, arrow.Arrow)
     return value.format(format_string)
 
 
 def to_arrow(value):
     """Convert a Date object to an arrow datetime object."""
     return arrow.get(value)
+
+
+def naturaltime(value):
+    """Get humanized version of time."""
+    arrow_value = to_arrow(value)
+    humanized = arrow_value.humanize()
+
+    return humanized
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/filters/html.py` & `invenio-formatter-1.3.0/invenio_formatter/filters/html.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter/templates/invenio_formatter/macros/badges.html` & `invenio-formatter-1.3.0/invenio_formatter/templates/invenio_formatter/macros/badges.html`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter/templates/invenio_formatter/macros/meta.html` & `invenio-formatter-1.3.0/invenio_formatter/templates/invenio_formatter/macros/meta.html`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html` & `invenio-formatter-1.3.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html` & `invenio-formatter-1.3.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/af/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6166  SS>.Language: af
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4166 7269 6b61 616e 7320 2868 7474 7073  Afrikaans (https
-00000130: 3a2f 2f77 7777 2e74 7261 6e73 6966 6578  ://www.transifex
+00000130: 3a2f 2f61 7070 2e74 7261 6e73 6966 6578  ://app.transifex
 00000140: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
 00000150: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
 00000160: 2f61 662f 290a 506c 7572 616c 2d46 6f72  /af/).Plural-For
 00000170: 6d73 3a20 6e70 6c75 7261 6c73 3d32 3b20  ms: nplurals=2; 
 00000180: 706c 7572 616c 3d28 6e20 213d 2031 293b  plural=(n != 1);
 00000190: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 000001a0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
 000001b0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
 000001c0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
 000001d0: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
 000001e0: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
 000001f0: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000200: 2e31 322e 300a 00                        .12.0..
+00000200: 2e31 322e 310a 00                        .12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/af/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/el/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: af\n"
+"Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,22 +2,22 @@
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
 "Language: ar\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/"
 "ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "HTML"
 msgstr "HTML"
 
 msgid "Image URL"
 msgstr "عنوان ويب URL الصورة "
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6267  SS>.Language: bg
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4275 6c67 6172 6961 6e20 2868 7474 7073  Bulgarian (https
-00000130: 3a2f 2f77 7777 2e74 7261 6e73 6966 6578  ://www.transifex
+00000130: 3a2f 2f61 7070 2e74 7261 6e73 6966 6578  ://app.transifex
 00000140: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
 00000150: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
 00000160: 2f62 672f 290a 506c 7572 616c 2d46 6f72  /bg/).Plural-For
 00000170: 6d73 3a20 6e70 6c75 7261 6c73 3d32 3b20  ms: nplurals=2; 
 00000180: 706c 7572 616c 3d28 6e20 213d 2031 293b  plural=(n != 1);
 00000190: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 000001a0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
 000001b0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
 000001c0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
 000001d0: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
 000001e0: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
 000001f0: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000200: 2e31 322e 300a 00                        .12.0..
+00000200: 2e31 322e 310a 00                        .12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6361  SS>.Language: ca
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4361 7461 6c61 6e20 2868 7474 7073 3a2f  Catalan (https:/
-00000130: 2f77 7777 2e74 7261 6e73 6966 6578 2e63  /www.transifex.c
+00000130: 2f61 7070 2e74 7261 6e73 6966 6578 2e63  /app.transifex.c
 00000140: 6f6d 2f69 6e76 656e 696f 736f 6674 7761  om/inveniosoftwa
 00000150: 7265 2f74 6561 6d73 2f32 3335 3337 2f63  re/teams/23537/c
 00000160: 612f 290a 506c 7572 616c 2d46 6f72 6d73  a/).Plural-Forms
 00000170: 3a20 6e70 6c75 7261 6c73 3d32 3b20 706c  : nplurals=2; pl
 00000180: 7572 616c 3d28 6e20 213d 2031 293b 0a4d  ural=(n != 1);.M
 00000190: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
 000001a0: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
 000001b0: 6578 742f 706c 6169 6e3b 2063 6861 7273  ext/plain; chars
 000001c0: 6574 3d75 7466 2d38 0a43 6f6e 7465 6e74  et=utf-8.Content
 000001d0: 2d54 7261 6e73 6665 722d 456e 636f 6469  -Transfer-Encodi
 000001e0: 6e67 3a20 3862 6974 0a47 656e 6572 6174  ng: 8bit.Generat
 000001f0: 6564 2d42 793a 2042 6162 656c 2032 2e31  ed-By: Babel 2.1
-00000200: 322e 300a 00                             2.0..
+00000200: 322e 310a 00                             2.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/ne/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Nepali (https://app.transifex.com/inveniosoftware/teams/23537/ne/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ca\n"
+"Language: ne\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 000000b0: 0a50 4f2d 5265 7669 7369 6f6e 2d44 6174  .PO-Revision-Dat
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6373  SS>.Language: cs
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
-00000120: 437a 6563 6820 2868 7474 7073 3a2f 2f77  Czech (https://w
-00000130: 7777 2e74 7261 6e73 6966 6578 2e63 6f6d  ww.transifex.com
+00000120: 437a 6563 6820 2868 7474 7073 3a2f 2f61  Czech (https://a
+00000130: 7070 2e74 7261 6e73 6966 6578 2e63 6f6d  pp.transifex.com
 00000140: 2f69 6e76 656e 696f 736f 6674 7761 7265  /inveniosoftware
 00000150: 2f74 6561 6d73 2f32 3335 3337 2f63 732f  /teams/23537/cs/
 00000160: 290a 506c 7572 616c 2d46 6f72 6d73 3a20  ).Plural-Forms: 
 00000170: 6e70 6c75 7261 6c73 3d34 3b20 706c 7572  nplurals=4; plur
 00000180: 616c 3d28 6e20 3d3d 2031 2026 2620 6e20  al=(n == 1 && n 
 00000190: 2520 3120 3d3d 2030 2920 3f20 3020 3a20  % 1 == 0) ? 0 : 
 000001a0: 286e 203e 3d20 3220 2626 206e 203c 3d20  (n >= 2 && n <= 
@@ -31,8 +31,8 @@
 000001e0: 452d 5665 7273 696f 6e3a 2031 2e30 0a43  E-Version: 1.0.C
 000001f0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 00000200: 742f 706c 6169 6e3b 2063 6861 7273 6574  t/plain; charset
 00000210: 3d75 7466 2d38 0a43 6f6e 7465 6e74 2d54  =utf-8.Content-T
 00000220: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
 00000230: 3a20 3862 6974 0a47 656e 6572 6174 6564  : 8bit.Generated
 00000240: 2d42 793a 2042 6162 656c 2032 2e31 322e  -By: Babel 2.12.
-00000250: 300a 00                                  0..
+00000250: 310a 00                                  1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/no/LC_MESSAGES/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: cs\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Language: no\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:20
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/da/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/da/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6461  SS>.Language: da
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4461 6e69 7368 2028 6874 7470 733a 2f2f  Danish (https://
-00000130: 7777 772e 7472 616e 7369 6665 782e 636f  www.transifex.co
+00000130: 6170 702e 7472 616e 7369 6665 782e 636f  app.transifex.co
 00000140: 6d2f 696e 7665 6e69 6f73 6f66 7477 6172  m/inveniosoftwar
 00000150: 652f 7465 616d 732f 3233 3533 372f 6461  e/teams/23537/da
 00000160: 2f29 0a50 6c75 7261 6c2d 466f 726d 733a  /).Plural-Forms:
 00000170: 206e 706c 7572 616c 733d 323b 2070 6c75   nplurals=2; plu
 00000180: 7261 6c3d 286e 2021 3d20 3129 3b0a 4d49  ral=(n != 1);.MI
 00000190: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
 000001a0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
 000001b0: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
 000001c0: 743d 7574 662d 380a 436f 6e74 656e 742d  t=utf-8.Content-
 000001d0: 5472 616e 7366 6572 2d45 6e63 6f64 696e  Transfer-Encodin
 000001e0: 673a 2038 6269 740a 4765 6e65 7261 7465  g: 8bit.Generate
 000001f0: 642d 4279 3a20 4261 6265 6c20 322e 3132  d-By: Babel 2.12
-00000200: 2e30 0a00                                .0..
+00000200: 2e31 0a00                                .1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/da/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/da/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/de/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/de/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,21 +2,21 @@
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Alexander Gruber <alexander.gruber@tugraz.at>, 2021\n"
 "Language: de\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/"
 "de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "HTML"
 msgstr "HTML"
 
 msgid "Image URL"
 msgstr "Bild URL"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/de/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/de/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Alexander Gruber <alexander.gruber@tugraz.at>, 2021\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/de/)\n"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/el/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 d501 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 d801 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d66 6f72 6d61 7474   invenio-formatt
 00000050: 6572 2031 2e31 2e33 0a52 6570 6f72 742d  er 1.1.3.Report-
 00000060: 4d73 6769 642d 4275 6773 2d54 6f3a 2069  Msgid-Bugs-To: i
 00000070: 6e66 6f40 696e 7665 6e69 6f73 6f66 7477  nfo@inveniosoftw
 00000080: 6172 652e 6f72 670a 504f 542d 4372 6561  are.org.POT-Crea
 00000090: 7469 6f6e 2d44 6174 653a 2032 3032 322d  tion-Date: 2022-
 000000a0: 3130 2d31 3220 3039 3a31 332b 3030 3030  10-12 09:13+0000
 000000b0: 0a50 4f2d 5265 7669 7369 6f6e 2d44 6174  .PO-Revision-Dat
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
-00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 656c  SS>.Language: el
+00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 676c  SS>.Language: gl
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
-00000120: 4772 6565 6b20 2868 7474 7073 3a2f 2f77  Greek (https://w
-00000130: 7777 2e74 7261 6e73 6966 6578 2e63 6f6d  ww.transifex.com
-00000140: 2f69 6e76 656e 696f 736f 6674 7761 7265  /inveniosoftware
-00000150: 2f74 6561 6d73 2f32 3335 3337 2f65 6c2f  /teams/23537/el/
-00000160: 290a 506c 7572 616c 2d46 6f72 6d73 3a20  ).Plural-Forms: 
-00000170: 6e70 6c75 7261 6c73 3d32 3b20 706c 7572  nplurals=2; plur
-00000180: 616c 3d28 6e20 213d 2031 293b 0a4d 494d  al=(n != 1);.MIM
-00000190: 452d 5665 7273 696f 6e3a 2031 2e30 0a43  E-Version: 1.0.C
-000001a0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000001b0: 742f 706c 6169 6e3b 2063 6861 7273 6574  t/plain; charset
-000001c0: 3d75 7466 2d38 0a43 6f6e 7465 6e74 2d54  =utf-8.Content-T
-000001d0: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
-000001e0: 3a20 3862 6974 0a47 656e 6572 6174 6564  : 8bit.Generated
-000001f0: 2d42 793a 2042 6162 656c 2032 2e31 322e  -By: Babel 2.12.
-00000200: 300a 00                                  0..
+00000120: 4761 6c69 6369 616e 2028 6874 7470 733a  Galician (https:
+00000130: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
+00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
+00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
+00000160: 676c 2f29 0a50 6c75 7261 6c2d 466f 726d  gl/).Plural-Form
+00000170: 733a 206e 706c 7572 616c 733d 323b 2070  s: nplurals=2; p
+00000180: 6c75 7261 6c3d 286e 2021 3d20 3129 3b0a  lural=(n != 1);.
+00000190: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
+000001a0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
+000001b0: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
+000001c0: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
+000001d0: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
+000001e0: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
+000001f0: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
+00000200: 3132 2e31 0a00                           12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/el/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: el\n"
+"Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/en/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/es/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/es/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,22 +2,22 @@
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2021\n"
 "Language: es\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "HTML"
 msgstr "HTML"
 
 msgid "Image URL"
 msgstr "URL de la imagen"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/es/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/es/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2021\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/et/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/et/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,21 +2,21 @@
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2021\n"
 "Language: et\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/et/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "HTML"
 msgstr "HTML"
 
 msgid "Image URL"
 msgstr "Pildi URL"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/et/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/et/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2021\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/teams/23537/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/teams/23537/et/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6574  SS>.Language: et
 00000110: 5f45 450a 4c61 6e67 7561 6765 2d54 6561  _EE.Language-Tea
 00000120: 6d3a 2045 7374 6f6e 6961 6e20 2845 7374  m: Estonian (Est
-00000130: 6f6e 6961 2920 2868 7474 7073 3a2f 2f77  onia) (https://w
-00000140: 7777 2e74 7261 6e73 6966 6578 2e63 6f6d  ww.transifex.com
+00000130: 6f6e 6961 2920 2868 7474 7073 3a2f 2f61  onia) (https://a
+00000140: 7070 2e74 7261 6e73 6966 6578 2e63 6f6d  pp.transifex.com
 00000150: 2f69 6e76 656e 696f 736f 6674 7761 7265  /inveniosoftware
 00000160: 2f74 6561 6d73 2f32 3335 3337 2f65 745f  /teams/23537/et_
 00000170: 4545 2f29 0a50 6c75 7261 6c2d 466f 726d  EE/).Plural-Form
 00000180: 733a 206e 706c 7572 616c 733d 323b 2070  s: nplurals=2; p
 00000190: 6c75 7261 6c3d 286e 2021 3d20 3129 3b0a  lural=(n != 1);.
 000001a0: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
 000001b0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
 000001c0: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
 000001d0: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
 000001e0: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
 000001f0: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
 00000200: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
-00000210: 3132 2e30 0a00                           12.0..
+00000210: 3132 2e31 0a00                           12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: German (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/de_AT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: et_EE\n"
+"Language: de_AT\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6661  SS>.Language: fa
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 5065 7273 6961 6e20 2868 7474 7073 3a2f  Persian (https:/
-00000130: 2f77 7777 2e74 7261 6e73 6966 6578 2e63  /www.transifex.c
+00000130: 2f61 7070 2e74 7261 6e73 6966 6578 2e63  /app.transifex.c
 00000140: 6f6d 2f69 6e76 656e 696f 736f 6674 7761  om/inveniosoftwa
 00000150: 7265 2f74 6561 6d73 2f32 3335 3337 2f66  re/teams/23537/f
 00000160: 612f 290a 506c 7572 616c 2d46 6f72 6d73  a/).Plural-Forms
 00000170: 3a20 6e70 6c75 7261 6c73 3d32 3b20 706c  : nplurals=2; pl
 00000180: 7572 616c 3d28 6e20 3e20 3129 3b0a 4d49  ural=(n > 1);.MI
 00000190: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
 000001a0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
 000001b0: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
 000001c0: 743d 7574 662d 380a 436f 6e74 656e 742d  t=utf-8.Content-
 000001d0: 5472 616e 7366 6572 2d45 6e63 6f64 696e  Transfer-Encodin
 000001e0: 673a 2038 6269 740a 4765 6e65 7261 7465  g: 8bit.Generate
 000001f0: 642d 4279 3a20 4261 6265 6c20 322e 3132  d-By: Babel 2.12
-00000200: 2e30 0a00                                .0..
+00000200: 2e31 0a00                                .1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Language-Team: German (Germany) (https://app.transifex.com/inveniosoftware/teams/23537/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: fa\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Language: de_DE\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:20
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6672  SS>.Language: fr
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4672 656e 6368 2028 6874 7470 733a 2f2f  French (https://
-00000130: 7777 772e 7472 616e 7369 6665 782e 636f  www.transifex.co
+00000130: 6170 702e 7472 616e 7369 6665 782e 636f  app.transifex.co
 00000140: 6d2f 696e 7665 6e69 6f73 6f66 7477 6172  m/inveniosoftwar
 00000150: 652f 7465 616d 732f 3233 3533 372f 6672  e/teams/23537/fr
 00000160: 2f29 0a50 6c75 7261 6c2d 466f 726d 733a  /).Plural-Forms:
 00000170: 206e 706c 7572 616c 733d 333b 2070 6c75   nplurals=3; plu
 00000180: 7261 6c3d 286e 203d 3d20 3020 7c7c 206e  ral=(n == 0 || n
 00000190: 203d 3d20 3129 203f 2030 203a 206e 2021   == 1) ? 0 : n !
 000001a0: 3d20 3020 2626 206e 2025 2031 3030 3030  = 0 && n % 10000
@@ -29,8 +29,8 @@
 000001c0: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 000001d0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
 000001e0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
 000001f0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
 00000200: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
 00000210: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
 00000220: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000230: 2e31 322e 300a 00                        .12.0..
+00000230: 2e31 322e 310a 00                        .12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 d801 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 d601 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d66 6f72 6d61 7474   invenio-formatt
 00000050: 6572 2031 2e31 2e33 0a52 6570 6f72 742d  er 1.1.3.Report-
 00000060: 4d73 6769 642d 4275 6773 2d54 6f3a 2069  Msgid-Bugs-To: i
 00000070: 6e66 6f40 696e 7665 6e69 6f73 6f66 7477  nfo@inveniosoftw
 00000080: 6172 652e 6f72 670a 504f 542d 4372 6561  are.org.POT-Crea
 00000090: 7469 6f6e 2d44 6174 653a 2032 3032 322d  tion-Date: 2022-
 000000a0: 3130 2d31 3220 3039 3a31 332b 3030 3030  10-12 09:13+0000
 000000b0: 0a50 4f2d 5265 7669 7369 6f6e 2d44 6174  .PO-Revision-Dat
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
-00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 676c  SS>.Language: gl
+00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6b61  SS>.Language: ka
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
-00000120: 4761 6c69 6369 616e 2028 6874 7470 733a  Galician (https:
-00000130: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
+00000120: 4765 6f72 6769 616e 2028 6874 7470 733a  Georgian (https:
+00000130: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
 00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
 00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
-00000160: 676c 2f29 0a50 6c75 7261 6c2d 466f 726d  gl/).Plural-Form
+00000160: 6b61 2f29 0a50 6c75 7261 6c2d 466f 726d  ka/).Plural-Form
 00000170: 733a 206e 706c 7572 616c 733d 323b 2070  s: nplurals=2; p
-00000180: 6c75 7261 6c3d 286e 2021 3d20 3129 3b0a  lural=(n != 1);.
-00000190: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
-000001a0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
-000001b0: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
-000001c0: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
-000001d0: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
-000001e0: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
-000001f0: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
-00000200: 3132 2e30 0a00                           12.0..
+00000180: 6c75 7261 6c3d 286e 213d 3129 3b0a 4d49  lural=(n!=1);.MI
+00000190: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
+000001a0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+000001b0: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
+000001c0: 743d 7574 662d 380a 436f 6e74 656e 742d  t=utf-8.Content-
+000001d0: 5472 616e 7366 6572 2d45 6e63 6f64 696e  Transfer-Encodin
+000001e0: 673a 2038 6269 740a 4765 6e65 7261 7465  g: 8bit.Generate
+000001f0: 642d 4279 3a20 4261 6265 6c20 322e 3132  d-By: Babel 2.12
+00000200: 2e31 0a00                                .1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: Hindi (India) (https://app.transifex.com/inveniosoftware/teams/23537/hi_IN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: gl\n"
+"Language: hi_IN\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 2002 0000 2d00 0000 0050 726f  ,... ...-....Pro
+00000020: 2c00 0000 0d02 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d66 6f72 6d61 7474   invenio-formatt
 00000050: 6572 2031 2e31 2e33 0a52 6570 6f72 742d  er 1.1.3.Report-
 00000060: 4d73 6769 642d 4275 6773 2d54 6f3a 2069  Msgid-Bugs-To: i
 00000070: 6e66 6f40 696e 7665 6e69 6f73 6f66 7477  nfo@inveniosoftw
 00000080: 6172 652e 6f72 670a 504f 542d 4372 6561  are.org.POT-Crea
 00000090: 7469 6f6e 2d44 6174 653a 2032 3032 322d  tion-Date: 2022-
 000000a0: 3130 2d31 3220 3039 3a31 332b 3030 3030  10-12 09:13+0000
 000000b0: 0a50 4f2d 5265 7669 7369 6f6e 2d44 6174  .PO-Revision-Dat
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
-00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6872  SS>.Language: hr
-00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
-00000120: 4372 6f61 7469 616e 2028 6874 7470 733a  Croatian (https:
-00000130: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
-00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
-00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
-00000160: 6872 2f29 0a50 6c75 7261 6c2d 466f 726d  hr/).Plural-Form
-00000170: 733a 206e 706c 7572 616c 733d 333b 2070  s: nplurals=3; p
-00000180: 6c75 7261 6c3d 6e25 3130 3d3d 3120 2626  lural=n%10==1 &&
-00000190: 206e 2531 3030 213d 3131 203f 2030 203a   n%100!=11 ? 0 :
-000001a0: 206e 2531 303e 3d32 2026 2620 6e25 3130   n%10>=2 && n%10
-000001b0: 3c3d 3420 2626 2028 6e25 3130 303c 3130  <=4 && (n%100<10
-000001c0: 207c 7c20 6e25 3130 303e 3d32 3029 203f   || n%100>=20) ?
-000001d0: 2031 203a 2032 3b0a 4d49 4d45 2d56 6572   1 : 2;.MIME-Ver
-000001e0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
-000001f0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
-00000200: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
-00000210: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
-00000220: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
-00000230: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
-00000240: 4261 6265 6c20 322e 3132 2e30 0a00       Babel 2.12.0..
+00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6573  SS>.Language: es
+00000110: 5f4d 580a 4c61 6e67 7561 6765 2d54 6561  _MX.Language-Tea
+00000120: 6d3a 2053 7061 6e69 7368 2028 4d65 7869  m: Spanish (Mexi
+00000130: 636f 2920 2868 7474 7073 3a2f 2f61 7070  co) (https://app
+00000140: 2e74 7261 6e73 6966 6578 2e63 6f6d 2f69  .transifex.com/i
+00000150: 6e76 656e 696f 736f 6674 7761 7265 2f74  nveniosoftware/t
+00000160: 6561 6d73 2f32 3335 3337 2f65 735f 4d58  eams/23537/es_MX
+00000170: 2f29 0a50 6c75 7261 6c2d 466f 726d 733a  /).Plural-Forms:
+00000180: 206e 706c 7572 616c 733d 333b 2070 6c75   nplurals=3; plu
+00000190: 7261 6c3d 6e20 3d3d 2031 203f 2030 203a  ral=n == 1 ? 0 :
+000001a0: 206e 2021 3d20 3020 2626 206e 2025 2031   n != 0 && n % 1
+000001b0: 3030 3030 3030 203d 3d20 3020 3f20 3120  000000 == 0 ? 1 
+000001c0: 3a20 323b 0a4d 494d 452d 5665 7273 696f  : 2;.MIME-Versio
+000001d0: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
+000001e0: 7970 653a 2074 6578 742f 706c 6169 6e3b  ype: text/plain;
+000001f0: 2063 6861 7273 6574 3d75 7466 2d38 0a43   charset=utf-8.C
+00000200: 6f6e 7465 6e74 2d54 7261 6e73 6665 722d  ontent-Transfer-
+00000210: 456e 636f 6469 6e67 3a20 3862 6974 0a47  Encoding: 8bit.G
+00000220: 656e 6572 6174 6564 2d42 793a 2042 6162  enerated-By: Bab
+00000230: 656c 2032 2e31 322e 310a 00              el 2.12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,30 +1,30 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
-"Language: hu\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/hu/)\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Last-Translator: Kalven Richie, 2022\n"
+"Language: zh_CN\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/"
+"teams/23537/zh_CN/)\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "HTML"
 msgstr "HTML"
 
 msgid "Image URL"
-msgstr "Kép URL"
+msgstr "图像URL"
 
 msgid "Markdown"
 msgstr "Markdown"
 
 msgid "Target URL"
-msgstr "Cél URL"
+msgstr "目标URL"
 
 msgid "reStructedText"
 msgstr "reStructedText"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/hu/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 # Translations template for invenio-formatter.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-formatter
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Andrea Dömötör, 2022
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/teams/23537/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: hu\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ro\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
-msgstr "Markdown"
+msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:20
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:21
 msgid "reStructedText"
-msgstr "reStructedText"
+msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:27
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:28
 msgid "HTML"
-msgstr "HTML"
+msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:34
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:35
 msgid "Image URL"
-msgstr "Kép URL"
+msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:41
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:42
 msgid "Target URL"
-msgstr "Cél URL"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/it/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 fe01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 2002 0000 2d00 0000 0050 726f  ,... ...-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d66 6f72 6d61 7474   invenio-formatt
 00000050: 6572 2031 2e31 2e33 0a52 6570 6f72 742d  er 1.1.3.Report-
 00000060: 4d73 6769 642d 4275 6773 2d54 6f3a 2069  Msgid-Bugs-To: i
 00000070: 6e66 6f40 696e 7665 6e69 6f73 6f66 7477  nfo@inveniosoftw
 00000080: 6172 652e 6f72 670a 504f 542d 4372 6561  are.org.POT-Crea
 00000090: 7469 6f6e 2d44 6174 653a 2032 3032 322d  tion-Date: 2022-
 000000a0: 3130 2d31 3220 3039 3a31 332b 3030 3030  10-12 09:13+0000
 000000b0: 0a50 4f2d 5265 7669 7369 6f6e 2d44 6174  .PO-Revision-Dat
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
-00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6974  SS>.Language: it
-00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
-00000120: 4974 616c 6961 6e20 2868 7474 7073 3a2f  Italian (https:/
-00000130: 2f77 7777 2e74 7261 6e73 6966 6578 2e63  /www.transifex.c
-00000140: 6f6d 2f69 6e76 656e 696f 736f 6674 7761  om/inveniosoftwa
-00000150: 7265 2f74 6561 6d73 2f32 3335 3337 2f69  re/teams/23537/i
-00000160: 742f 290a 506c 7572 616c 2d46 6f72 6d73  t/).Plural-Forms
-00000170: 3a20 6e70 6c75 7261 6c73 3d33 3b20 706c  : nplurals=3; pl
-00000180: 7572 616c 3d6e 203d 3d20 3120 3f20 3020  ural=n == 1 ? 0 
-00000190: 3a20 6e20 213d 2030 2026 2620 6e20 2520  : n != 0 && n % 
-000001a0: 3130 3030 3030 3020 3d3d 2030 203f 2031  1000000 == 0 ? 1
-000001b0: 203a 2032 3b0a 4d49 4d45 2d56 6572 7369   : 2;.MIME-Versi
-000001c0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
-000001d0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
-000001e0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
-000001f0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
-00000200: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
-00000210: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000220: 6265 6c20 322e 3132 2e30 0a00            bel 2.12.0..
+00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6672  SS>.Language: fr
+00000110: 5f43 490a 4c61 6e67 7561 6765 2d54 6561  _CI.Language-Tea
+00000120: 6d3a 2046 7265 6e63 6820 2843 c3b4 7465  m: French (C..te
+00000130: 2064 2749 766f 6972 6529 2028 6874 7470   d'Ivoire) (http
+00000140: 733a 2f2f 6170 702e 7472 616e 7369 6665  s://app.transife
+00000150: 782e 636f 6d2f 696e 7665 6e69 6f73 6f66  x.com/inveniosof
+00000160: 7477 6172 652f 7465 616d 732f 3233 3533  tware/teams/2353
+00000170: 372f 6672 5f43 492f 290a 506c 7572 616c  7/fr_CI/).Plural
+00000180: 2d46 6f72 6d73 3a20 6e70 6c75 7261 6c73  -Forms: nplurals
+00000190: 3d33 3b20 706c 7572 616c 3d28 6e20 3d3d  =3; plural=(n ==
+000001a0: 2030 207c 7c20 6e20 3d3d 2031 2920 3f20   0 || n == 1) ? 
+000001b0: 3020 3a20 6e20 213d 2030 2026 2620 6e20  0 : n != 0 && n 
+000001c0: 2520 3130 3030 3030 3020 3d3d 2030 203f  % 1000000 == 0 ?
+000001d0: 2031 203a 2032 3b0a 4d49 4d45 2d56 6572   1 : 2;.MIME-Ver
+000001e0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
+000001f0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
+00000200: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
+00000210: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
+00000220: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
+00000230: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
+00000240: 4261 6265 6c20 322e 3132 2e31 0a00       Babel 2.12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/it/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/teams/23537/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: it\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: pt\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:20
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ja/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: English (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/en_AT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ja\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: en_AT\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:20
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 d601 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 e701 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d66 6f72 6d61 7474   invenio-formatt
 00000050: 6572 2031 2e31 2e33 0a52 6570 6f72 742d  er 1.1.3.Report-
 00000060: 4d73 6769 642d 4275 6773 2d54 6f3a 2069  Msgid-Bugs-To: i
 00000070: 6e66 6f40 696e 7665 6e69 6f73 6f66 7477  nfo@inveniosoftw
 00000080: 6172 652e 6f72 670a 504f 542d 4372 6561  are.org.POT-Crea
 00000090: 7469 6f6e 2d44 6174 653a 2032 3032 322d  tion-Date: 2022-
 000000a0: 3130 2d31 3220 3039 3a31 332b 3030 3030  10-12 09:13+0000
 000000b0: 0a50 4f2d 5265 7669 7369 6f6e 2d44 6174  .PO-Revision-Dat
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
-00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6b61  SS>.Language: ka
-00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
-00000120: 4765 6f72 6769 616e 2028 6874 7470 733a  Georgian (https:
-00000130: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
-00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
-00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
-00000160: 6b61 2f29 0a50 6c75 7261 6c2d 466f 726d  ka/).Plural-Form
-00000170: 733a 206e 706c 7572 616c 733d 323b 2070  s: nplurals=2; p
-00000180: 6c75 7261 6c3d 286e 213d 3129 3b0a 4d49  lural=(n!=1);.MI
-00000190: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
-000001a0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-000001b0: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
-000001c0: 743d 7574 662d 380a 436f 6e74 656e 742d  t=utf-8.Content-
-000001d0: 5472 616e 7366 6572 2d45 6e63 6f64 696e  Transfer-Encodin
-000001e0: 673a 2038 6269 740a 4765 6e65 7261 7465  g: 8bit.Generate
-000001f0: 642d 4279 3a20 4261 6265 6c20 322e 3132  d-By: Babel 2.12
-00000200: 2e30 0a00                                .0..
+00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 656e  SS>.Language: en
+00000110: 5f41 540a 4c61 6e67 7561 6765 2d54 6561  _AT.Language-Tea
+00000120: 6d3a 2045 6e67 6c69 7368 2028 4175 7374  m: English (Aust
+00000130: 7269 6129 2028 6874 7470 733a 2f2f 6170  ria) (https://ap
+00000140: 702e 7472 616e 7369 6665 782e 636f 6d2f  p.transifex.com/
+00000150: 696e 7665 6e69 6f73 6f66 7477 6172 652f  inveniosoftware/
+00000160: 7465 616d 732f 3233 3533 372f 656e 5f41  teams/23537/en_A
+00000170: 542f 290a 506c 7572 616c 2d46 6f72 6d73  T/).Plural-Forms
+00000180: 3a20 6e70 6c75 7261 6c73 3d32 3b20 706c  : nplurals=2; pl
+00000190: 7572 616c 3d28 6e20 213d 2031 293b 0a4d  ural=(n != 1);.M
+000001a0: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
+000001b0: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
+000001c0: 6578 742f 706c 6169 6e3b 2063 6861 7273  ext/plain; chars
+000001d0: 6574 3d75 7466 2d38 0a43 6f6e 7465 6e74  et=utf-8.Content
+000001e0: 2d54 7261 6e73 6665 722d 456e 636f 6469  -Transfer-Encodi
+000001f0: 6e67 3a20 3862 6974 0a47 656e 6572 6174  ng: 8bit.Generat
+00000200: 6564 2d42 793a 2042 6162 656c 2032 2e31  ed-By: Babel 2.1
+00000210: 322e 310a 00                             2.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6c74  SS>.Language: lt
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4c69 7468 7561 6e69 616e 2028 6874 7470  Lithuanian (http
-00000130: 733a 2f2f 7777 772e 7472 616e 7369 6665  s://www.transife
+00000130: 733a 2f2f 6170 702e 7472 616e 7369 6665  s://app.transife
 00000140: 782e 636f 6d2f 696e 7665 6e69 6f73 6f66  x.com/inveniosof
 00000150: 7477 6172 652f 7465 616d 732f 3233 3533  tware/teams/2353
 00000160: 372f 6c74 2f29 0a50 6c75 7261 6c2d 466f  7/lt/).Plural-Fo
 00000170: 726d 733a 206e 706c 7572 616c 733d 343b  rms: nplurals=4;
 00000180: 2070 6c75 7261 6c3d 286e 2025 2031 3020   plural=(n % 10 
 00000190: 3d3d 2031 2026 2620 286e 2025 2031 3030  == 1 && (n % 100
 000001a0: 203e 2031 3920 7c7c 206e 2025 2031 3030   > 19 || n % 100
@@ -34,8 +34,8 @@
 00000210: 2033 293b 0a4d 494d 452d 5665 7273 696f   3);.MIME-Versio
 00000220: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
 00000230: 7970 653a 2074 6578 742f 706c 6169 6e3b  ype: text/plain;
 00000240: 2063 6861 7273 6574 3d75 7466 2d38 0a43   charset=utf-8.C
 00000250: 6f6e 7465 6e74 2d54 7261 6e73 6665 722d  ontent-Transfer-
 00000260: 456e 636f 6469 6e67 3a20 3862 6974 0a47  Encoding: 8bit.G
 00000270: 656e 6572 6174 6564 2d42 793a 2042 6162  enerated-By: Bab
-00000280: 656c 2032 2e31 322e 300a 00              el 2.12.0..
+00000280: 656c 2032 2e31 322e 310a 00              el 2.12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/messages.pot` & `invenio-formatter-1.3.0/invenio_formatter/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/no/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 d901 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 1802 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d66 6f72 6d61 7474   invenio-formatt
 00000050: 6572 2031 2e31 2e33 0a52 6570 6f72 742d  er 1.1.3.Report-
 00000060: 4d73 6769 642d 4275 6773 2d54 6f3a 2069  Msgid-Bugs-To: i
 00000070: 6e66 6f40 696e 7665 6e69 6f73 6f66 7477  nfo@inveniosoftw
 00000080: 6172 652e 6f72 670a 504f 542d 4372 6561  are.org.POT-Crea
 00000090: 7469 6f6e 2d44 6174 653a 2032 3032 322d  tion-Date: 2022-
 000000a0: 3130 2d31 3220 3039 3a31 332b 3030 3030  10-12 09:13+0000
 000000b0: 0a50 4f2d 5265 7669 7369 6f6e 2d44 6174  .PO-Revision-Dat
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
-00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6e6f  SS>.Language: no
-00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
-00000120: 4e6f 7277 6567 6961 6e20 2868 7474 7073  Norwegian (https
-00000130: 3a2f 2f77 7777 2e74 7261 6e73 6966 6578  ://www.transifex
-00000140: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
-00000150: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
-00000160: 2f6e 6f2f 290a 506c 7572 616c 2d46 6f72  /no/).Plural-For
-00000170: 6d73 3a20 6e70 6c75 7261 6c73 3d32 3b20  ms: nplurals=2; 
-00000180: 706c 7572 616c 3d28 6e20 213d 2031 293b  plural=(n != 1);
-00000190: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
-000001a0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
-000001b0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
-000001c0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
-000001d0: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
-000001e0: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
-000001f0: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000200: 2e31 322e 300a 00                        .12.0..
+00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6672  SS>.Language: fr
+00000110: 5f46 520a 4c61 6e67 7561 6765 2d54 6561  _FR.Language-Tea
+00000120: 6d3a 2046 7265 6e63 6820 2846 7261 6e63  m: French (Franc
+00000130: 6529 2028 6874 7470 733a 2f2f 6170 702e  e) (https://app.
+00000140: 7472 616e 7369 6665 782e 636f 6d2f 696e  transifex.com/in
+00000150: 7665 6e69 6f73 6f66 7477 6172 652f 7465  veniosoftware/te
+00000160: 616d 732f 3233 3533 372f 6672 5f46 522f  ams/23537/fr_FR/
+00000170: 290a 506c 7572 616c 2d46 6f72 6d73 3a20  ).Plural-Forms: 
+00000180: 6e70 6c75 7261 6c73 3d33 3b20 706c 7572  nplurals=3; plur
+00000190: 616c 3d28 6e20 3d3d 2030 207c 7c20 6e20  al=(n == 0 || n 
+000001a0: 3d3d 2031 2920 3f20 3020 3a20 6e20 213d  == 1) ? 0 : n !=
+000001b0: 2030 2026 2620 6e20 2520 3130 3030 3030   0 && n % 100000
+000001c0: 3020 3d3d 2030 203f 2031 203a 2032 3b0a  0 == 0 ? 1 : 2;.
+000001d0: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
+000001e0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
+000001f0: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
+00000200: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
+00000210: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
+00000220: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
+00000230: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
+00000240: 3132 2e31 0a00                           12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/no/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Language-Team: Kinyarwanda (https://app.transifex.com/inveniosoftware/teams/23537/rw/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: no\n"
+"Language: rw\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 706c  SS>.Language: pl
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 506f 6c69 7368 2028 6874 7470 733a 2f2f  Polish (https://
-00000130: 7777 772e 7472 616e 7369 6665 782e 636f  www.transifex.co
+00000130: 6170 702e 7472 616e 7369 6665 782e 636f  app.transifex.co
 00000140: 6d2f 696e 7665 6e69 6f73 6f66 7477 6172  m/inveniosoftwar
 00000150: 652f 7465 616d 732f 3233 3533 372f 706c  e/teams/23537/pl
 00000160: 2f29 0a50 6c75 7261 6c2d 466f 726d 733a  /).Plural-Forms:
 00000170: 206e 706c 7572 616c 733d 343b 2070 6c75   nplurals=4; plu
 00000180: 7261 6c3d 286e 3d3d 3120 3f20 3020 3a20  ral=(n==1 ? 0 : 
 00000190: 286e 2531 303e 3d32 2026 2620 6e25 3130  (n%10>=2 && n%10
 000001a0: 3c3d 3429 2026 2620 286e 2531 3030 3c31  <=4) && (n%100<1
@@ -35,8 +35,8 @@
 00000220: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
 00000230: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
 00000240: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
 00000250: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
 00000260: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
 00000270: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
 00000280: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
-00000290: 3132 2e30 0a00                           12.0..
+00000290: 3132 2e31 0a00                           12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 7074  SS>.Language: pt
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 506f 7274 7567 7565 7365 2028 6874 7470  Portuguese (http
-00000130: 733a 2f2f 7777 772e 7472 616e 7369 6665  s://www.transife
+00000130: 733a 2f2f 6170 702e 7472 616e 7369 6665  s://app.transife
 00000140: 782e 636f 6d2f 696e 7665 6e69 6f73 6f66  x.com/inveniosof
 00000150: 7477 6172 652f 7465 616d 732f 3233 3533  tware/teams/2353
 00000160: 372f 7074 2f29 0a50 6c75 7261 6c2d 466f  7/pt/).Plural-Fo
 00000170: 726d 733a 206e 706c 7572 616c 733d 333b  rms: nplurals=3;
 00000180: 2070 6c75 7261 6c3d 286e 203d 3d20 3020   plural=(n == 0 
 00000190: 7c7c 206e 203d 3d20 3129 203f 2030 203a  || n == 1) ? 0 :
 000001a0: 206e 2021 3d20 3020 2626 206e 2025 2031   n != 0 && n % 1
@@ -29,8 +29,8 @@
 000001c0: 3a20 323b 0a4d 494d 452d 5665 7273 696f  : 2;.MIME-Versio
 000001d0: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
 000001e0: 7970 653a 2074 6578 742f 706c 6169 6e3b  ype: text/plain;
 000001f0: 2063 6861 7273 6574 3d75 7466 2d38 0a43   charset=utf-8.C
 00000200: 6f6e 7465 6e74 2d54 7261 6e73 6665 722d  ontent-Transfer-
 00000210: 456e 636f 6469 6e67 3a20 3862 6974 0a47  Encoding: 8bit.G
 00000220: 656e 6572 6174 6564 2d42 793a 2042 6162  enerated-By: Bab
-00000230: 656c 2032 2e31 322e 300a 00              el 2.12.0..
+00000230: 656c 2032 2e31 322e 310a 00              el 2.12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Hungarian (Hungary) (https://app.transifex.com/inveniosoftware/teams/23537/hu_HU/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: pt\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: hu_HU\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:20
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 19% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 726f  SS>.Language: ro
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 526f 6d61 6e69 616e 2028 6874 7470 733a  Romanian (https:
-00000130: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
+00000130: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
 00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
 00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
 00000160: 726f 2f29 0a50 6c75 7261 6c2d 466f 726d  ro/).Plural-Form
 00000170: 733a 206e 706c 7572 616c 733d 333b 2070  s: nplurals=3; p
 00000180: 6c75 7261 6c3d 286e 3d3d 313f 303a 2828  lural=(n==1?0:((
 00000190: 286e 2531 3030 3e31 3929 7c7c 2828 6e25  (n%100>19)||((n%
 000001a0: 3130 303d 3d30 2926 2628 6e21 3d30 2929  100==0)&&(n!=0))
 000001b0: 293f 323a 3129 293b 0a4d 494d 452d 5665  )?2:1));.MIME-Ve
 000001c0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
 000001d0: 6e74 2d54 7970 653a 2074 6578 742f 706c  nt-Type: text/pl
 000001e0: 6169 6e3b 2063 6861 7273 6574 3d75 7466  ain; charset=utf
 000001f0: 2d38 0a43 6f6e 7465 6e74 2d54 7261 6e73  -8.Content-Trans
 00000200: 6665 722d 456e 636f 6469 6e67 3a20 3862  fer-Encoding: 8b
 00000210: 6974 0a47 656e 6572 6174 6564 2d42 793a  it.Generated-By:
-00000220: 2042 6162 656c 2032 2e31 322e 300a 00     Babel 2.12.0..
+00000220: 2042 6162 656c 2032 2e31 322e 310a 00     Babel 2.12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ro\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
+"Language: zh_TW\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:20
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 7275  SS>.Language: ru
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 5275 7373 6961 6e20 2868 7474 7073 3a2f  Russian (https:/
-00000130: 2f77 7777 2e74 7261 6e73 6966 6578 2e63  /www.transifex.c
+00000130: 2f61 7070 2e74 7261 6e73 6966 6578 2e63  /app.transifex.c
 00000140: 6f6d 2f69 6e76 656e 696f 736f 6674 7761  om/inveniosoftwa
 00000150: 7265 2f74 6561 6d73 2f32 3335 3337 2f72  re/teams/23537/r
 00000160: 752f 290a 506c 7572 616c 2d46 6f72 6d73  u/).Plural-Forms
 00000170: 3a20 6e70 6c75 7261 6c73 3d34 3b20 706c  : nplurals=4; pl
 00000180: 7572 616c 3d28 6e25 3130 3d3d 3120 2626  ural=(n%10==1 &&
 00000190: 206e 2531 3030 213d 3131 203f 2030 203a   n%100!=11 ? 0 :
 000001a0: 206e 2531 303e 3d32 2026 2620 6e25 3130   n%10>=2 && n%10
@@ -34,8 +34,8 @@
 00000210: 2032 203a 2033 293b 0a4d 494d 452d 5665   2 : 3);.MIME-Ve
 00000220: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
 00000230: 6e74 2d54 7970 653a 2074 6578 742f 706c  nt-Type: text/pl
 00000240: 6169 6e3b 2063 6861 7273 6574 3d75 7466  ain; charset=utf
 00000250: 2d38 0a43 6f6e 7465 6e74 2d54 7261 6e73  -8.Content-Trans
 00000260: 6665 722d 456e 636f 6469 6e67 3a20 3862  fer-Encoding: 8b
 00000270: 6974 0a47 656e 6572 6174 6564 2d42 793a  it.Generated-By:
-00000280: 2042 6162 656c 2032 2e31 322e 300a 00     Babel 2.12.0..
+00000280: 2042 6162 656c 2032 2e31 322e 310a 00     Babel 2.12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 23% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 7277  SS>.Language: rw
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4b69 6e79 6172 7761 6e64 6120 2868 7474  Kinyarwanda (htt
-00000130: 7073 3a2f 2f77 7777 2e74 7261 6e73 6966  ps://www.transif
+00000130: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
 00000140: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
 00000150: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
 00000160: 3337 2f72 772f 290a 506c 7572 616c 2d46  37/rw/).Plural-F
 00000170: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
 00000180: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
 00000190: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
 000001a0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
 000001b0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
 000001c0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
 000001d0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
 000001e0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
 000001f0: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
-00000200: 2032 2e31 322e 300a 00                    2.12.0..
+00000200: 2032 2e31 322e 310a 00                    2.12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 # Translations template for invenio-formatter.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-formatter
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
+# Translators:
+# Sam Arbid, 2022
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Last-Translator: Sam Arbid, 2022\n"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/teams/23537/sv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: rw\n"
+"Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
-msgstr ""
+msgstr "Markdown"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:20
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:21
 msgid "reStructedText"
-msgstr ""
+msgstr "reStructedText"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:27
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:28
 msgid "HTML"
-msgstr ""
+msgstr "HTML"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:34
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:35
 msgid "Image URL"
-msgstr ""
+msgstr "Bild URL"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:41
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:42
 msgid "Target URL"
-msgstr ""
+msgstr "Mål URL"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 736b  SS>.Language: sk
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 536c 6f76 616b 2028 6874 7470 733a 2f2f  Slovak (https://
-00000130: 7777 772e 7472 616e 7369 6665 782e 636f  www.transifex.co
+00000130: 6170 702e 7472 616e 7369 6665 782e 636f  app.transifex.co
 00000140: 6d2f 696e 7665 6e69 6f73 6f66 7477 6172  m/inveniosoftwar
 00000150: 652f 7465 616d 732f 3233 3533 372f 736b  e/teams/23537/sk
 00000160: 2f29 0a50 6c75 7261 6c2d 466f 726d 733a  /).Plural-Forms:
 00000170: 206e 706c 7572 616c 733d 343b 2070 6c75   nplurals=4; plu
 00000180: 7261 6c3d 286e 2025 2031 203d 3d20 3020  ral=(n % 1 == 0 
 00000190: 2626 206e 203d 3d20 3120 3f20 3020 3a20  && n == 1 ? 0 : 
 000001a0: 6e20 2520 3120 3d3d 2030 2026 2620 6e20  n % 1 == 0 && n 
@@ -30,8 +30,8 @@
 000001d0: 3f20 323a 2033 293b 0a4d 494d 452d 5665  ? 2: 3);.MIME-Ve
 000001e0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
 000001f0: 6e74 2d54 7970 653a 2074 6578 742f 706c  nt-Type: text/pl
 00000200: 6169 6e3b 2063 6861 7273 6574 3d75 7466  ain; charset=utf
 00000210: 2d38 0a43 6f6e 7465 6e74 2d54 7261 6e73  -8.Content-Trans
 00000220: 6665 722d 456e 636f 6469 6e67 3a20 3862  fer-Encoding: 8b
 00000230: 6974 0a47 656e 6572 6174 6564 2d42 793a  it.Generated-By:
-00000240: 2042 6162 656c 2032 2e31 322e 300a 00     Babel 2.12.0..
+00000240: 2042 6162 656c 2032 2e31 322e 310a 00     Babel 2.12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,21 +2,21 @@
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Sam Arbid, 2022\n"
 "Language: sv\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "HTML"
 msgstr "HTML"
 
 msgid "Image URL"
 msgstr "Bild URL"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/af/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 # Translations template for invenio-formatter.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-formatter
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Sam Arbid, 2022
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Language-Team: Afrikaans (https://app.transifex.com/inveniosoftware/teams/23537/af/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: sv\n"
+"Language: af\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
-msgstr "Markdown"
+msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:20
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:21
 msgid "reStructedText"
-msgstr "reStructedText"
+msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:27
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:28
 msgid "HTML"
-msgstr "HTML"
+msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:34
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:35
 msgid "Image URL"
-msgstr "Bild URL"
+msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:41
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:42
 msgid "Target URL"
-msgstr "Mål URL"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,21 +3,21 @@
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume."
 "com>, 2021\n"
 "Language: tr\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/tr/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "HTML"
 msgstr "HTML"
 
 msgid "Image URL"
 msgstr "Görselin URL adresi"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2021\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 756b  SS>.Language: uk
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 556b 7261 696e 6961 6e20 2868 7474 7073  Ukrainian (https
-00000130: 3a2f 2f77 7777 2e74 7261 6e73 6966 6578  ://www.transifex
+00000130: 3a2f 2f61 7070 2e74 7261 6e73 6966 6578  ://app.transifex
 00000140: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
 00000150: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
 00000160: 2f75 6b2f 290a 506c 7572 616c 2d46 6f72  /uk/).Plural-For
 00000170: 6d73 3a20 6e70 6c75 7261 6c73 3d34 3b20  ms: nplurals=4; 
 00000180: 706c 7572 616c 3d28 6e20 2520 3120 3d3d  plural=(n % 1 ==
 00000190: 2030 2026 2620 6e20 2520 3130 203d 3d20   0 && n % 10 == 
 000001a0: 3120 2626 206e 2025 2031 3030 2021 3d20  1 && n % 100 != 
@@ -40,8 +40,8 @@
 00000270: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
 00000280: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
 00000290: 6578 742f 706c 6169 6e3b 2063 6861 7273  ext/plain; chars
 000002a0: 6574 3d75 7466 2d38 0a43 6f6e 7465 6e74  et=utf-8.Content
 000002b0: 2d54 7261 6e73 6665 722d 456e 636f 6469  -Transfer-Encodi
 000002c0: 6e67 3a20 3862 6974 0a47 656e 6572 6174  ng: 8bit.Generat
 000002d0: 6564 2d42 793a 2042 6162 656c 2032 2e31  ed-By: Babel 2.1
-000002e0: 322e 300a 00                             2.0..
+000002e0: 322e 310a 00                             2.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: Ukrainian (https://app.transifex.com/inveniosoftware/teams/23537/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
 "Last-Translator: Kalven Richie, 2022\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-formatter-1.3.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-formatter 1.1.3*

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 000000c0: 653a 2032 3031 362d 3038 2d32 3520 3038  e: 2016-08-25 08
 000000d0: 3a34 312b 3030 3030 0a4c 6173 742d 5472  :41+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 7a68  SS>.Language: zh
 00000110: 5f54 570a 4c61 6e67 7561 6765 2d54 6561  _TW.Language-Tea
 00000120: 6d3a 2043 6869 6e65 7365 2028 5461 6977  m: Chinese (Taiw
-00000130: 616e 2920 2868 7474 7073 3a2f 2f77 7777  an) (https://www
+00000130: 616e 2920 2868 7474 7073 3a2f 2f61 7070  an) (https://app
 00000140: 2e74 7261 6e73 6966 6578 2e63 6f6d 2f69  .transifex.com/i
 00000150: 6e76 656e 696f 736f 6674 7761 7265 2f74  nveniosoftware/t
 00000160: 6561 6d73 2f32 3335 3337 2f7a 685f 5457  eams/23537/zh_TW
 00000170: 2f29 0a50 6c75 7261 6c2d 466f 726d 733a  /).Plural-Forms:
 00000180: 206e 706c 7572 616c 733d 313b 2070 6c75   nplurals=1; plu
 00000190: 7261 6c3d 303b 0a4d 494d 452d 5665 7273  ral=0;.MIME-Vers
 000001a0: 696f 6e3a 2031 2e30 0a43 6f6e 7465 6e74  ion: 1.0.Content
 000001b0: 2d54 7970 653a 2074 6578 742f 706c 6169  -Type: text/plai
 000001c0: 6e3b 2063 6861 7273 6574 3d75 7466 2d38  n; charset=utf-8
 000001d0: 0a43 6f6e 7465 6e74 2d54 7261 6e73 6665  .Content-Transfe
 000001e0: 722d 456e 636f 6469 6e67 3a20 3862 6974  r-Encoding: 8bit
 000001f0: 0a47 656e 6572 6174 6564 2d42 793a 2042  .Generated-By: B
-00000200: 6162 656c 2032 2e31 322e 300a 00         abel 2.12.0..
+00000200: 6162 656c 2032 2e31 322e 310a 00         abel 2.12.1..
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-formatter-1.3.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-formatter 1.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:13+0000\n"
 "PO-Revision-Date: 2016-08-25 08:41+0000\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: Galician (https://app.transifex.com/inveniosoftware/teams/23537/gl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: zh_TW\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: gl\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:14
 #: invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html:15
 msgid "Markdown"
 msgstr ""
 
 #: invenio_formatter/templates/invenio_formatter/macros/badges.html:20
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter/views.py` & `invenio-formatter-1.3.0/invenio_formatter/views.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/invenio_formatter.egg-info/PKG-INFO` & `invenio-formatter-1.3.0/invenio_formatter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-formatter
-Version: 1.2.0
+Version: 1.3.0
 Summary: "Jinja utilities for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-formatter
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.3.0 (released 2023-07-17)
+        
+        - add template filter for human readable time
+        
         Version 1.2.0 (released 2021-02-28)
         
         - remove flask-babelex deprecated dependency
         - upgrade invenio-i18n to manage babel globally
         
         Version 1.1.4 (released 2021-10-18)
```

### Comparing `invenio-formatter-1.2.0/invenio_formatter.egg-info/SOURCES.txt` & `invenio-formatter-1.3.0/invenio_formatter.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -66,42 +66,66 @@
 invenio_formatter/translations/ca/LC_MESSAGES/messages.po
 invenio_formatter/translations/cs/LC_MESSAGES/messages.mo
 invenio_formatter/translations/cs/LC_MESSAGES/messages.po
 invenio_formatter/translations/da/LC_MESSAGES/messages.mo
 invenio_formatter/translations/da/LC_MESSAGES/messages.po
 invenio_formatter/translations/de/LC_MESSAGES/messages.mo
 invenio_formatter/translations/de/LC_MESSAGES/messages.po
+invenio_formatter/translations/de_AT/LC_MESSAGES/messages.mo
+invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po
+invenio_formatter/translations/de_DE/LC_MESSAGES/messages.mo
+invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po
 invenio_formatter/translations/el/LC_MESSAGES/messages.mo
 invenio_formatter/translations/el/LC_MESSAGES/messages.po
 invenio_formatter/translations/en/LC_MESSAGES/messages.mo
 invenio_formatter/translations/en/LC_MESSAGES/messages.po
+invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo
+invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po
+invenio_formatter/translations/en_HU/LC_MESSAGES/messages.mo
+invenio_formatter/translations/en_HU/LC_MESSAGES/messages.po
 invenio_formatter/translations/es/LC_MESSAGES/messages.mo
 invenio_formatter/translations/es/LC_MESSAGES/messages.po
+invenio_formatter/translations/es_CU/LC_MESSAGES/messages.mo
+invenio_formatter/translations/es_CU/LC_MESSAGES/messages.po
+invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo
+invenio_formatter/translations/es_MX/LC_MESSAGES/messages.po
 invenio_formatter/translations/et/LC_MESSAGES/messages.mo
 invenio_formatter/translations/et/LC_MESSAGES/messages.po
 invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo
 invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po
 invenio_formatter/translations/fa/LC_MESSAGES/messages.mo
 invenio_formatter/translations/fa/LC_MESSAGES/messages.po
+invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.mo
+invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.po
 invenio_formatter/translations/fr/LC_MESSAGES/messages.mo
 invenio_formatter/translations/fr/LC_MESSAGES/messages.po
+invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo
+invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.po
+invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo
+invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.po
 invenio_formatter/translations/gl/LC_MESSAGES/messages.mo
 invenio_formatter/translations/gl/LC_MESSAGES/messages.po
+invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.mo
+invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po
 invenio_formatter/translations/hr/LC_MESSAGES/messages.mo
 invenio_formatter/translations/hr/LC_MESSAGES/messages.po
 invenio_formatter/translations/hu/LC_MESSAGES/messages.mo
 invenio_formatter/translations/hu/LC_MESSAGES/messages.po
+invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.mo
+invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po
 invenio_formatter/translations/it/LC_MESSAGES/messages.mo
 invenio_formatter/translations/it/LC_MESSAGES/messages.po
 invenio_formatter/translations/ja/LC_MESSAGES/messages.mo
 invenio_formatter/translations/ja/LC_MESSAGES/messages.po
 invenio_formatter/translations/ka/LC_MESSAGES/messages.mo
 invenio_formatter/translations/ka/LC_MESSAGES/messages.po
 invenio_formatter/translations/lt/LC_MESSAGES/messages.mo
 invenio_formatter/translations/lt/LC_MESSAGES/messages.po
+invenio_formatter/translations/ne/LC_MESSAGES/messages.mo
+invenio_formatter/translations/ne/LC_MESSAGES/messages.po
 invenio_formatter/translations/no/LC_MESSAGES/messages.mo
 invenio_formatter/translations/no/LC_MESSAGES/messages.po
 invenio_formatter/translations/pl/LC_MESSAGES/messages.mo
 invenio_formatter/translations/pl/LC_MESSAGES/messages.po
 invenio_formatter/translations/pt/LC_MESSAGES/messages.mo
 invenio_formatter/translations/pt/LC_MESSAGES/messages.po
 invenio_formatter/translations/ro/LC_MESSAGES/messages.mo
@@ -110,18 +134,22 @@
 invenio_formatter/translations/ru/LC_MESSAGES/messages.po
 invenio_formatter/translations/rw/LC_MESSAGES/messages.mo
 invenio_formatter/translations/rw/LC_MESSAGES/messages.po
 invenio_formatter/translations/sk/LC_MESSAGES/messages.mo
 invenio_formatter/translations/sk/LC_MESSAGES/messages.po
 invenio_formatter/translations/sv/LC_MESSAGES/messages.mo
 invenio_formatter/translations/sv/LC_MESSAGES/messages.po
+invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.mo
+invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.po
 invenio_formatter/translations/tr/LC_MESSAGES/messages.mo
 invenio_formatter/translations/tr/LC_MESSAGES/messages.po
 invenio_formatter/translations/uk/LC_MESSAGES/messages.mo
 invenio_formatter/translations/uk/LC_MESSAGES/messages.po
+invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.mo
+invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.po
 invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo
 invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po
 invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo
 invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po
 tests/conftest.py
 tests/test_examples_app.py
 tests/test_filters.py
```

### Comparing `invenio-formatter-1.2.0/run-tests.sh` & `invenio-formatter-1.3.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/setup.cfg` & `invenio-formatter-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/tests/conftest.py` & `invenio-formatter-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/tests/test_examples_app.py` & `invenio-formatter-1.3.0/tests/test_examples_app.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/tests/test_filters.py` & `invenio-formatter-1.3.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/tests/test_invenio_formatter.py` & `invenio-formatter-1.3.0/tests/test_invenio_formatter.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/tests/test_template_context_processors.py` & `invenio-formatter-1.3.0/tests/test_template_context_processors.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/tests/test_template_macros.py` & `invenio-formatter-1.3.0/tests/test_template_macros.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-1.2.0/tests/test_views.py` & `invenio-formatter-1.3.0/tests/test_views.py`

 * *Files identical despite different names*

