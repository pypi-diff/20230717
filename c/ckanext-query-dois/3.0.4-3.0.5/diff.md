# Comparing `tmp/ckanext-query-dois-3.0.4.tar.gz` & `tmp/ckanext-query-dois-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-query-dois-3.0.4.tar", last modified: Tue Apr 11 08:24:03 2023, max compression
+gzip compressed data, was "ckanext-query-dois-3.0.5.tar", last modified: Mon Jul 17 08:21:40 2023, max compression
```

## Comparing `ckanext-query-dois-3.0.4.tar` & `ckanext-query-dois-3.0.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.392981 ckanext-query-dois-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-04-11 08:24:03.392981 ckanext-query-dois-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.376981 ckanext-query-dois-3.0.4/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.376981 ckanext-query-dois-3.0.4/ckanext/query_dois/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.380981 ckanext-query-dois-3.0.4/ckanext/query_dois/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/lib/doi.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/lib/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/lib/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/lib/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.384981 ckanext-query-dois-3.0.4/ckanext/query_dois/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/logic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/logic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/logic/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/logic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.384981 ckanext-query-dois-3.0.4/ckanext/query_dois/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/routes/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/routes/query_doi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.372981 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.384981 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.384981 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/assets/less/query_dois.less
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/assets/less/visual_query.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.384981 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/assets/scripts/multisearch_download.js
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.372981 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.388981 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/multisearch_landing_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/single_landing_page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.388981 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/snippets/recent_dois_sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_multisearch.html
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.392981 ckanext-query-dois-3.0.4/ckanext_query_dois.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-04-11 08:24:03.000000 ckanext-query-dois-3.0.4/ckanext_query_dois.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-11 08:24:03.000000 ckanext-query-dois-3.0.4/ckanext_query_dois.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:24:03.000000 ckanext-query-dois-3.0.4/ckanext_query_dois.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-11 08:24:03.000000 ckanext-query-dois-3.0.4/ckanext_query_dois.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:24:02.000000 ckanext-query-dois-3.0.4/ckanext_query_dois.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-11 08:24:03.000000 ckanext-query-dois-3.0.4/ckanext_query_dois.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 08:24:03.000000 ckanext-query-dois-3.0.4/ckanext_query_dois.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.372981 ckanext-query-dois-3.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.392981 ckanext-query-dois-3.0.4/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:24:03.392981 ckanext-query-dois-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.372981 ckanext-query-dois-3.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:24:03.392981 ckanext-query-dois-3.0.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/tests/unit/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/tests/unit/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 08:23:43.000000 ckanext-query-dois-3.0.4/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.745512 ckanext-query-dois-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-17 08:21:40.745512 ckanext-query-dois-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.737512 ckanext-query-dois-3.0.5/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/doi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/routes/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/routes/query_doi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.737512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/less/query_dois.less
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/less/visual_query.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/scripts/multisearch_download.js
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.737512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/multisearch_landing_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/single_landing_page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/recent_dois_sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_multisearch.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.737512 ckanext-query-dois-3.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:21:40.745512 ckanext-query-dois-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.737512 ckanext-query-dois-3.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.745512 ckanext-query-dois-3.0.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/tests/unit/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/tests/unit/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/tests/unit/test_utils.py
```

### Comparing `ckanext-query-dois-3.0.4/LICENSE` & `ckanext-query-dois-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/PKG-INFO` & `ckanext-query-dois-3.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-query-dois
-Version: 3.0.4
+Version: 3.0.5
 Summary: A CKAN extension that creates DOIs for queries on resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-query-dois
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-query-dois/blob/main/CHANGELOG.md
 Keywords: CKAN,data,doi
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-query-dois/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-query-dois
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-query-dois/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-query-dois/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-query-dois/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-query-dois)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-query-dois-3.0.4/README.md` & `ckanext-query-dois-3.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-query-dois/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-query-dois
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-query-dois/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-query-dois/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-query-dois/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-query-dois)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/cli.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/helpers.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/lib/doi.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/lib/doi.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/lib/emails.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/lib/emails.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/lib/query.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/lib/query.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/lib/stats.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/lib/stats.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/lib/utils.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/lib/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/logic/action.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/logic/schema.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/logic/utils.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/logic/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/model.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/model.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/plugin.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/routes/_helpers.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/routes/_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/routes/query_doi.py` & `ckanext-query-dois-3.0.5/ckanext/query_dois/routes/query_doi.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/theme/assets/less/query_dois.less` & `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/less/query_dois.less`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/theme/assets/scripts/multisearch_download.js` & `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/scripts/multisearch_download.js`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/multisearch_landing_page.html` & `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/multisearch_landing_page.html`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/single_landing_page.html` & `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/single_landing_page.html`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/snippets/recent_dois_sidebar.html` & `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/recent_dois_sidebar.html`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_search.html` & `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_search.html`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/ckanext_query_dois.egg-info/PKG-INFO` & `ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-query-dois
-Version: 3.0.4
+Version: 3.0.5
 Summary: A CKAN extension that creates DOIs for queries on resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-query-dois
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-query-dois/blob/main/CHANGELOG.md
 Keywords: CKAN,data,doi
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-query-dois/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-query-dois
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-query-dois/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-query-dois/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-query-dois/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-query-dois)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-query-dois-3.0.4/ckanext_query_dois.egg-info/SOURCES.txt` & `ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/docs/_scripts/gen_api_pages.py` & `ckanext-query-dois-3.0.5/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/pyproject.toml` & `ckanext-query-dois-3.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-query-dois"
-version = "3.0.4"
+version = "3.0.5"
 description = "A CKAN extension that creates DOIs for queries on resources."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -54,15 +54,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.query_dois.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "3.0.4"
+version = "3.0.5"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-query-dois-3.0.4/tests/unit/test_helpers.py` & `ckanext-query-dois-3.0.5/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/tests/unit/test_plugin.py` & `ckanext-query-dois-3.0.5/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.4/tests/unit/test_utils.py` & `ckanext-query-dois-3.0.5/tests/unit/test_utils.py`

 * *Files identical despite different names*

