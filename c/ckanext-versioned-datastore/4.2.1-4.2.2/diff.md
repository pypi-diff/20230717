# Comparing `tmp/ckanext-versioned-datastore-4.2.1.tar.gz` & `tmp/ckanext-versioned-datastore-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-versioned-datastore-4.2.1.tar", last modified: Tue Apr 11 08:37:04 2023, max compression
+gzip compressed data, was "ckanext-versioned-datastore-4.2.2.tar", last modified: Mon Jul 17 08:28:42 2023, max compression
```

## Comparing `ckanext-versioned-datastore-4.2.1.tar` & `ckanext-versioned-datastore-4.2.2.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.629442 ckanext-versioned-datastore-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-04-11 08:37:04.629442 ckanext-versioned-datastore-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.581442 ckanext-versioned-datastore-4.2.1/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.581442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16585 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.581442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.581442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/basic_query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/basic_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/basic_query/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/basic_query/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/basic_query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/datastore_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.585442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.585442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.585442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    17480 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.589442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/notifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/notifiers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/notifiers/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.589442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/servers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/servers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/servers/direct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.589442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.589442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.593442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/queuing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.593442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/query_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/slug_words.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/slugs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26610 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/v1_0_0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.593442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.593442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/basic_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.597442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    35737 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/meta/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/meta/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/multisearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.573442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.597442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/versioned_datastore/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/versioned_datastore/README
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/versioned_datastore/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/versioned_datastore/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.597442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/versioned_datastore/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.597442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/model/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/model/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/model/slugs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/model/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.601442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/routes/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/routes/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/routes/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/routes/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.577442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.601442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.605442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/less/download-status.less
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/less/search.less
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/less/slugerator.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.577442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.605442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/scripts/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.605442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/scripts/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.605442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/api.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.577442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.605442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.609442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/1.json
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/10.json
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/12.json
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/2.json
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/3.json
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/4.json
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/7.json
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/8.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.621442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/
--rw-r--r--   0 runner    (1001) docker     (123)  3183938 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson
--rw-r--r--   0 runner    (1001) docker     (123)  4137025 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson
--rw-r--r--   0 runner    (1001) docker     (123)  1316321 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.577442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.621442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/resource_data.html
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/resource_edit_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.621442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.621442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/search/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/search/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/search/slugerator.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.621442 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/status/
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/status/download.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.625442 ckanext-versioned-datastore-4.2.1/ckanext_versioned_datastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-04-11 08:37:04.000000 ckanext-versioned-datastore-4.2.1/ckanext_versioned_datastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-04-11 08:37:04.000000 ckanext-versioned-datastore-4.2.1/ckanext_versioned_datastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:37:04.000000 ckanext-versioned-datastore-4.2.1/ckanext_versioned_datastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-11 08:37:04.000000 ckanext-versioned-datastore-4.2.1/ckanext_versioned_datastore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:37:04.000000 ckanext-versioned-datastore-4.2.1/ckanext_versioned_datastore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-11 08:37:04.000000 ckanext-versioned-datastore-4.2.1/ckanext_versioned_datastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 08:37:04.000000 ckanext-versioned-datastore-4.2.1/ckanext_versioned_datastore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.577442 ckanext-versioned-datastore-4.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.625442 ckanext-versioned-datastore-4.2.1/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:37:04.629442 ckanext-versioned-datastore-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.577442 ckanext-versioned-datastore-4.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.625442 ckanext-versioned-datastore-4.2.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/helpers/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/helpers/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/helpers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.577442 ckanext-versioned-datastore-4.2.1/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.625442 ckanext-versioned-datastore-4.2.1/tests/integration/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/integration/downloads/test_downloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.625442 ckanext-versioned-datastore-4.2.1/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.625442 ckanext-versioned-datastore-4.2.1/tests/unit/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.625442 ckanext-versioned-datastore-4.2.1/tests/unit/lib/basic_query/
--rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/basic_query/test_basic_query_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/basic_query/test_basic_query_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/basic_query/test_basic_query_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.629442 ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.629442 ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/test_downloads_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/test_downloads_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/test_downloads_runmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/test_downloads_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.577442 ckanext-versioned-datastore-4.2.1/tests/unit/lib/importing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.629442 ckanext-versioned-datastore-4.2.1/tests/unit/lib/importing/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/importing/ingestion/test_ingestion_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.629442 ckanext-versioned-datastore-4.2.1/tests/unit/lib/query/
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/query/test_query_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/query/test_query_v1_0_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/lib/test_datastore_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.577442 ckanext-versioned-datastore-4.2.1/tests/unit/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:37:04.629442 ckanext-versioned-datastore-4.2.1/tests/unit/logic/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/logic/actions/test_actions_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-11 08:36:47.000000 ckanext-versioned-datastore-4.2.1/tests/unit/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16585 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/datastore_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17480 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/servers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/servers/direct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/queuing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/query_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/slug_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26610 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/v1_0_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/basic_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35737 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/multisearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/download-status.less
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/search.less
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/slugerator.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/api.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.654268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/12.json
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/8.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.662268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/
+-rw-r--r--   0 runner    (1001) docker     (123)  3183938 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)  4137025 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)  1316321 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.662268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/resource_data.html
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/resource_edit_base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.662268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.662268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/search/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/search/slugerator.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.662268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/status/download.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/helpers/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/helpers/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/helpers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/integration/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/integration/downloads/test_downloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_runmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/importing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/importing/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/importing/ingestion/test_ingestion_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/query/test_query_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/query/test_query_v1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/test_datastore_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/tests/unit/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/logic/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/logic/actions/test_actions_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/test_helpers.py
```

### Comparing `ckanext-versioned-datastore-4.2.1/LICENSE` & `ckanext-versioned-datastore-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/PKG-INFO` & `ckanext-versioned-datastore-4.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-versioned-datastore
-Version: 4.2.1
+Version: 4.2.2
 Summary: A CKAN extension providing a versioned datastore using MongoDB and Elasticsearch
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/blob/main/CHANGELOG.md
 Keywords: CKAN,data,versioned_datastore
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doi
 Provides-Extra: attribution
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-versioned-datastore
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-versioned-datastore/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-versioned-datastore/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-versioned-datastore)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-versioned-datastore-4.2.1/README.md` & `ckanext-versioned-datastore-4.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-versioned-datastore
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-versioned-datastore/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-versioned-datastore/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-versioned-datastore)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/cli.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/helpers.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/interfaces.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/basic_query/geo.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/geo.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/basic_query/search.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/basic_query/utils.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/common.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/common.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/datastore_utils.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/datastore_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/base.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/base.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/json.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/json.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/download.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/download.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/loaders.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/loaders.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/notifiers/base.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/notifiers/email.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/email.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/query.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/query.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/downloads/utils.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/details.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/details.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/importing.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/importing.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/indexing.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/indexing.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/readers.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/readers.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
                 # number
                 if field == '_id':
                     if isinstance(cell.value, numbers.Integral):
                         data[field] = cell.value
                     else:
                         raise Exception('_id not int')
                 # ignore empty cells
-                elif isinstance(cell, EmptyCell):
+                elif isinstance(cell, EmptyCell) or cell.value is None:
                     continue
                 else:
                     # convert everything else to unicode
                     value = str(cell.value)
                     if value:
                         data[field] = value
             # yield the row
```

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/records.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/records.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/ingestion/utils.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/queuing.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/queuing.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/stats.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/stats.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/importing/utils.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/fields.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/fields.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/query_log.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/query_log.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/schema.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/slug_words.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/slug_words.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/slugs.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/slugs.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/utils.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/lib/query/v1_0_0.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/v1_0_0.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/basic_search.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/basic_search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/crud.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/crud.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/downloads.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/downloads.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/extras.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/extras.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/meta/help.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/help.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/meta/schema.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/actions/multisearch.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/multisearch.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/logic/auth.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/versioned_datastore/env.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/model/details.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/details.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/model/downloads.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/downloads.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/model/slugs.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/slugs.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/model/stats.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/stats.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/plugin.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/routes/datastore.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/datastore.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/routes/downloads.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/downloads.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/routes/search.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/routes/status.py` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/status.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/assets/webassets.yml` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/webassets.yml`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/api.html` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/api.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/resource_data.html` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/resource_data.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/search/search.html` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/search/slugerator.html` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/search/slugerator.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext/versioned_datastore/theme/templates/status/download.html` & `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/status/download.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext_versioned_datastore.egg-info/PKG-INFO` & `ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-versioned-datastore
-Version: 4.2.1
+Version: 4.2.2
 Summary: A CKAN extension providing a versioned datastore using MongoDB and Elasticsearch
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/blob/main/CHANGELOG.md
 Keywords: CKAN,data,versioned_datastore
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doi
 Provides-Extra: attribution
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-versioned-datastore
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-versioned-datastore/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-versioned-datastore/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-versioned-datastore)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-versioned-datastore-4.2.1/ckanext_versioned_datastore.egg-info/SOURCES.txt` & `ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/docs/_scripts/gen_api_pages.py` & `ckanext-versioned-datastore-4.2.2/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/pyproject.toml` & `ckanext-versioned-datastore-4.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-versioned-datastore"
-version = "4.2.1"
+version = "4.2.2"
 description = "A CKAN extension providing a versioned datastore using MongoDB and Elasticsearch"
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -71,15 +71,15 @@
 
 [tool.setuptools.package-data]
 "ckanext.versioned_datastore.theme" = ["*", "**/*"]
 "ckanext.versioned_datastore.migration" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "4.2.1"
+version = "4.2.2"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-versioned-datastore-4.2.1/tests/helpers/data.py` & `ckanext-versioned-datastore-4.2.2/tests/helpers/data.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/helpers/patches.py` & `ckanext-versioned-datastore-4.2.2/tests/helpers/patches.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/helpers/utils.py` & `ckanext-versioned-datastore-4.2.2/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/integration/downloads/test_downloads.py` & `ckanext-versioned-datastore-4.2.2/tests/integration/downloads/test_downloads.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/basic_query/test_basic_query_geo.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_geo.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/basic_query/test_basic_query_search.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/basic_query/test_basic_query_utils.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/test_downloads_notifiers.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_notifiers.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/test_downloads_query.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_query.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/test_downloads_runmanager.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_runmanager.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/downloads/test_downloads_utils.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/importing/ingestion/test_ingestion_records.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/importing/ingestion/test_ingestion_records.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/query/test_query_query.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/query/test_query_query.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/query/test_query_v1_0_0.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/query/test_query_v1_0_0.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/lib/test_datastore_utils.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/lib/test_datastore_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/logic/actions/test_actions_downloads.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/logic/actions/test_actions_downloads.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.1/tests/unit/test_helpers.py` & `ckanext-versioned-datastore-4.2.2/tests/unit/test_helpers.py`

 * *Files identical despite different names*

