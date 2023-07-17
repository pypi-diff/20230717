# Comparing `tmp/collective.restapi.facetedsearch-1.0.2.tar.gz` & `tmp/collective.restapi.facetedsearch-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.restapi.facetedsearch-1.0.2.tar", last modified: Mon Jul 17 06:56:02 2023, max compression
+gzip compressed data, was "collective.restapi.facetedsearch-1.0.3.tar", last modified: Mon Jul 17 11:54:42 2023, max compression
```

## Comparing `collective.restapi.facetedsearch-1.0.2.tar` & `collective.restapi.facetedsearch-1.0.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      300 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/CHANGES.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       63 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/CONTRIBUTORS.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      586 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/DEVELOP.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      671 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/LICENSE.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       67 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/MANIFEST.in
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6853 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4111 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/README.rst
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/docs/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7923 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/docs/conf.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      119 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/docs/index.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      321 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2690 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/setup.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       80 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       80 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      149 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      297 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/configure.zcml
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      300 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/configure.zcml
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/faceted_search/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/faceted_search/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      539 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/faceted_search/configure.zcml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      564 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/faceted_search/get.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      688 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/faceted_search/groupByModifiers.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10977 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/faceted_search/handler.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/browser/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/browser/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      645 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/browser/configure.zcml
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/browser/overrides/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/browser/overrides/.gitkeep
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/browser/static/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/browser/static/.gitkeep
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1480 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/configure.zcml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      280 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/interfaces.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      611 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/README.rst
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/collective.restapi.facetedsearch.pot
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/en/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/en/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       28 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/en/LC_MESSAGES/collective.restapi.facetedsearch.mo
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/en/LC_MESSAGES/collective.restapi.facetedsearch.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1770 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/update.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      533 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/update.sh
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      260 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/permissions.zcml
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/profiles/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/profiles/default/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      221 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/profiles/default/browserlayer.xml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      105 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/profiles/default/catalog.xml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      254 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/profiles/default/metadata.xml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      190 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/profiles/default/registry.xml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      118 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/profiles/default/rolemap.xml
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/profiles/uninstall/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      142 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      633 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/setuphandlers.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1769 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/testing.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/tests/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/tests/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/tests/robot/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2059 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/tests/robot/test_example.robot
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      932 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/tests/test_robot.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2732 2023-07-17 06:56:01.000000 collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/tests/test_setup.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6853 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2994 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      157 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       30 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/namespace_packages.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/not-zip-safe
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      201 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       11 2023-07-17 06:56:02.000000 collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/top_level.txt
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      465 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/CHANGES.rst
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       63 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/CONTRIBUTORS.rst
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      586 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/DEVELOP.rst
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      671 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/LICENSE.rst
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       67 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/MANIFEST.in
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7035 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4097 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/README.rst
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/docs/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7923 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/docs/conf.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      119 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/docs/index.rst
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      321 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/setup.cfg
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2673 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/setup.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/collective/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       80 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/__init__.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       80 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/__init__.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      149 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/__init__.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      297 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/configure.zcml
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      300 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/configure.zcml
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/faceted_search/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/faceted_search/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      539 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/faceted_search/configure.zcml
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      564 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/faceted_search/get.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      688 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/faceted_search/groupByModifiers.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10977 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/faceted_search/handler.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/browser/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/browser/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      645 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/browser/configure.zcml
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/browser/overrides/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/browser/overrides/.gitkeep
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/browser/static/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/browser/static/.gitkeep
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1480 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/configure.zcml
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      280 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/interfaces.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      611 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/README.rst
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/collective.restapi.facetedsearch.pot
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/en/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       28 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/en/LC_MESSAGES/collective.restapi.facetedsearch.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/en/LC_MESSAGES/collective.restapi.facetedsearch.po
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1770 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/update.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      533 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/update.sh
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      260 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/permissions.zcml
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/profiles/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/profiles/default/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      221 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/profiles/default/browserlayer.xml
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      105 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/profiles/default/catalog.xml
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      254 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/profiles/default/metadata.xml
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      190 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/profiles/default/registry.xml
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      118 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/profiles/default/rolemap.xml
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/profiles/uninstall/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      142 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      633 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/setuphandlers.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1769 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/testing.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/tests/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/tests/__init__.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.109323 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/tests/robot/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2059 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/tests/robot/test_example.robot
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      932 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/tests/test_robot.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2732 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/tests/test_setup.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 11:54:42.105322 collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7035 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2994 2023-07-17 11:54:42.000000 collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/SOURCES.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/dependency_links.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      157 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/entry_points.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       30 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/namespace_packages.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/not-zip-safe
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      201 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/requires.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       11 2023-07-17 11:54:41.000000 collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.restapi.facetedsearch-1.0.2/DEVELOP.rst` & `collective.restapi.facetedsearch-1.0.3/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/LICENSE.rst` & `collective.restapi.facetedsearch-1.0.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/PKG-INFO` & `collective.restapi.facetedsearch-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: collective.restapi.facetedsearch
-Version: 1.0.2
+Version: 1.0.3
 Summary: An add-on for Plone and plone.restapi providing a extended search service
-Home-page: https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch
+Home-page: https://github.com/collective/collective.restapi.facetedsearch
 Author: muellers
 Author-email: muellers@saw-leipzig.de
 License: GPL version 2
-Project-URL: PyPI, https://pypi.python.org/pypi/collective.restapi.facetedsearch
-Project-URL: Source, https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch.git
-Project-URL: Tracker, https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch/-/issues
+Project-URL: PyPI, https://pypi.python.org/project/collective.restapi.facetedsearch
+Project-URL: Source, https://github.com/collective/collective.restapi.facetedsearch.git
+Project-URL: Tracker, https://github.com/collective/collective.restapi.facetedsearch/issues
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
            This text does not appear on pypi or github. It is a comment.
         
         ================================
         collective.restapi.facetedsearch
         ================================
@@ -118,16 +118,16 @@
         - plone.restapi
         - collective.collectionfilter
         
         
         Contribute
         ==========
         
-        - Issue Tracker: https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch/-/issues
-        - Source Code: https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch.git
+        - Issue Tracker: https://github.com/collective/collective.restapi.facetedsearch/issues
+        - Source Code: https://github.com/collective/collective.restapi.facetedsearch.git
         - Documentation: https://docs.plone.org
         
         
         License
         =======
         
         The project is licensed under the GPLv2.
@@ -138,18 +138,24 @@
         
         - muellers, muellers@saw-leipzig.de
         
         
         Changelog
         =========
         
+        1.0.3 (2023-07-17)
+        ------------------
+        
+        - moved git repository to https://github.com/collective/collective.restapi.facetedsearch; modified readme.rst and setup.py
+        
+        
         1.0.2 (2023-07-05)
         ------------------
         
-        -added some project description
+        - added some project description
         
         
         1.0.1 (2022-06-02)
         ------------------
         
         - bugfix for empty query and empty resultset in post handler
         - removing limit in post handler
```

### Comparing `collective.restapi.facetedsearch-1.0.2/README.rst` & `collective.restapi.facetedsearch-1.0.3/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -107,16 +107,16 @@
 - plone.restapi
 - collective.collectionfilter
 
 
 Contribute
 ==========
 
-- Issue Tracker: https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch/-/issues
-- Source Code: https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch.git
+- Issue Tracker: https://github.com/collective/collective.restapi.facetedsearch/issues
+- Source Code: https://github.com/collective/collective.restapi.facetedsearch.git
 - Documentation: https://docs.plone.org
 
 
 License
 =======
 
 The project is licensed under the GPLv2.
```

### Comparing `collective.restapi.facetedsearch-1.0.2/docs/conf.py` & `collective.restapi.facetedsearch-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/setup.py` & `collective.restapi.facetedsearch-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='collective.restapi.facetedsearch',
-    version='1.0.2',
+    version='1.0.3',
     description="An add-on for Plone and plone.restapi providing a extended search service",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -29,19 +29,19 @@
         "Programming Language :: Python :: 3.7",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords='Python Plone',
     author='muellers',
     author_email='muellers@saw-leipzig.de',
-    url='https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch',
+    url='https://github.com/collective/collective.restapi.facetedsearch',
     project_urls={
-        'PyPI': 'https://pypi.python.org/pypi/collective.restapi.facetedsearch',
-        'Source': 'https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch.git',
-        'Tracker': 'https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch/-/issues',
+        'PyPI': 'https://pypi.python.org/project/collective.restapi.facetedsearch',
+        'Source': 'https://github.com/collective/collective.restapi.facetedsearch.git',
+        'Tracker': 'https://github.com/collective/collective.restapi.facetedsearch/issues',
         # 'Documentation': 'https://collective.restapi.facetedsearch.readthedocs.io/en/latest/',
     },
     license='GPL version 2',
     packages=find_packages('src', exclude=['ez_setup']),
     namespace_packages=['collective', 'collective.restapi'],
     package_dir={'': 'src'},
     include_package_data=True,
```

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/faceted_search/configure.zcml` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/faceted_search/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/faceted_search/get.py` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/faceted_search/get.py`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/faceted_search/groupByModifiers.py` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/faceted_search/groupByModifiers.py`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/api/services/faceted_search/handler.py` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/api/services/faceted_search/handler.py`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/browser/configure.zcml` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/configure.zcml` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/README.rst` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/update.py` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/locales/update.sh` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/setuphandlers.py` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/testing.py` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/testing.py`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/tests/robot/test_example.robot` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/tests/test_robot.py` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective/restapi/facetedsearch/tests/test_setup.py` & `collective.restapi.facetedsearch-1.0.3/src/collective/restapi/facetedsearch/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/PKG-INFO` & `collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: collective.restapi.facetedsearch
-Version: 1.0.2
+Version: 1.0.3
 Summary: An add-on for Plone and plone.restapi providing a extended search service
-Home-page: https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch
+Home-page: https://github.com/collective/collective.restapi.facetedsearch
 Author: muellers
 Author-email: muellers@saw-leipzig.de
 License: GPL version 2
-Project-URL: PyPI, https://pypi.python.org/pypi/collective.restapi.facetedsearch
-Project-URL: Source, https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch.git
-Project-URL: Tracker, https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch/-/issues
+Project-URL: PyPI, https://pypi.python.org/project/collective.restapi.facetedsearch
+Project-URL: Source, https://github.com/collective/collective.restapi.facetedsearch.git
+Project-URL: Tracker, https://github.com/collective/collective.restapi.facetedsearch/issues
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
            This text does not appear on pypi or github. It is a comment.
         
         ================================
         collective.restapi.facetedsearch
         ================================
@@ -118,16 +118,16 @@
         - plone.restapi
         - collective.collectionfilter
         
         
         Contribute
         ==========
         
-        - Issue Tracker: https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch/-/issues
-        - Source Code: https://git.saw-leipzig.de/muellers/collective.restapi.facetedsearch.git
+        - Issue Tracker: https://github.com/collective/collective.restapi.facetedsearch/issues
+        - Source Code: https://github.com/collective/collective.restapi.facetedsearch.git
         - Documentation: https://docs.plone.org
         
         
         License
         =======
         
         The project is licensed under the GPLv2.
@@ -138,18 +138,24 @@
         
         - muellers, muellers@saw-leipzig.de
         
         
         Changelog
         =========
         
+        1.0.3 (2023-07-17)
+        ------------------
+        
+        - moved git repository to https://github.com/collective/collective.restapi.facetedsearch; modified readme.rst and setup.py
+        
+        
         1.0.2 (2023-07-05)
         ------------------
         
-        -added some project description
+        - added some project description
         
         
         1.0.1 (2022-06-02)
         ------------------
         
         - bugfix for empty query and empty resultset in post handler
         - removing limit in post handler
```

### Comparing `collective.restapi.facetedsearch-1.0.2/src/collective.restapi.facetedsearch.egg-info/SOURCES.txt` & `collective.restapi.facetedsearch-1.0.3/src/collective.restapi.facetedsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

