# Comparing `tmp/terminusdb-client-10.2.3.tar.gz` & `tmp/terminusdb-client-10.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminusdb-client-10.2.3.tar", last modified: Tue May 30 12:29:31 2023, max compression
+gzip compressed data, was "terminusdb-client-10.2.4.tar", last modified: Mon Jul 17 12:17:46 2023, max compression
```

## Comparing `terminusdb-client-10.2.3.tar` & `terminusdb-client-10.2.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.559061 terminusdb-client-10.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-30 12:29:31.559061 terminusdb-client-10.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-30 12:29:31.559061 terminusdb-client-10.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.547061 terminusdb-client-10.2.3/terminusdb_client/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.547061 terminusdb-client-10.2.3/terminusdb_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)    96359 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/client/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.547061 terminusdb-client-10.2.3/terminusdb_client/query_syntax/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/query_syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/query_syntax/query_syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.547061 terminusdb-client-10.2.3/terminusdb_client/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37919 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.551061 terminusdb-client-10.2.3/terminusdb_client/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/scripts/schema_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    34318 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/scripts/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.551061 terminusdb-client-10.2.3/terminusdb_client/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/AllServerRecords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/DBRecord.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/ans_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/ans_doctype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/ans_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/ans_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/ans_triple_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/connectCapabilitiesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/connectionObjDump.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/getSchemaTurtleResponse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.555061 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/mock_jsons.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/mockResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/serverRecordsFromCap.py
--rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_Client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_Schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_backwardsCompat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_woqlCore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_woqlExtra.py
--rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_woqlQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.555061 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlAndJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlCastJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlConcatJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlDeleteJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlDoctypeJson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlExtraJson.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlIdgenJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlJoinSplitJson.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlLimitStar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlMathJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlOptJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlOrJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlReJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlSelectJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlStarJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlTrimJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlWhenJson.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woql_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woql_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.555061 terminusdb-client-10.2.3/terminusdb_client/woqlclient/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqlclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.555061 terminusdb-client-10.2.3/terminusdb_client/woqldataframe/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqldataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqldataframe/woqlDataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.559061 terminusdb-client-10.2.3/terminusdb_client/woqlquery/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqlquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqlquery/woql_core.py
--rw-r--r--   0 runner    (1001) docker     (123)   106610 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqlquery/woql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.559061 terminusdb-client-10.2.3/terminusdb_client/woqlschema/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqlschema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.547061 terminusdb-client-10.2.3/terminusdb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.679246 terminusdb-client-10.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-07-17 12:17:46.679246 terminusdb-client-10.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-17 12:17:46.679246 terminusdb-client-10.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.671246 terminusdb-client-10.2.4/terminusdb_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.671246 terminusdb-client-10.2.4/terminusdb_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    96589 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/client/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.671246 terminusdb-client-10.2.4/terminusdb_client/query_syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/query_syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/query_syntax/query_syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.671246 terminusdb-client-10.2.4/terminusdb_client/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38417 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/schema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.671246 terminusdb-client-10.2.4/terminusdb_client/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/scripts/schema_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34318 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/scripts/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.675246 terminusdb-client-10.2.4/terminusdb_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/AllServerRecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/DBRecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/ans_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/ans_doctype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/ans_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/ans_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/ans_triple_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/connectCapabilitiesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/connectionObjDump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/getSchemaTurtleResponse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.675246 terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/mock_jsons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/mockResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/serverRecordsFromCap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/test_Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/test_Schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/test_backwardsCompat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/test_woqlCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/test_woqlExtra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/test_woqlQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.675246 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlAndJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlCastJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlConcatJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlDeleteJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlDoctypeJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlExtraJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlIdgenJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlJoinSplitJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlLimitStar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlMathJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlOptJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlOrJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlReJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlSelectJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlStarJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlTrimJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlWhenJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/woql_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/woql_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.675246 terminusdb-client-10.2.4/terminusdb_client/woqlclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/woqlclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.679246 terminusdb-client-10.2.4/terminusdb_client/woqldataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/woqldataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/woqldataframe/woqlDataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.679246 terminusdb-client-10.2.4/terminusdb_client/woqlquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/woqlquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/woqlquery/woql_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106610 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/woqlquery/woql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.679246 terminusdb-client-10.2.4/terminusdb_client/woqlschema/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 12:17:43.000000 terminusdb-client-10.2.4/terminusdb_client/woqlschema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:46.671246 terminusdb-client-10.2.4/terminusdb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-07-17 12:17:46.000000 terminusdb-client-10.2.4/terminusdb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-17 12:17:46.000000 terminusdb-client-10.2.4/terminusdb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:17:46.000000 terminusdb-client-10.2.4/terminusdb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 12:17:46.000000 terminusdb-client-10.2.4/terminusdb_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 12:17:46.000000 terminusdb-client-10.2.4/terminusdb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 12:17:46.000000 terminusdb-client-10.2.4/terminusdb_client.egg-info/top_level.txt
```

### Comparing `terminusdb-client-10.2.3/LICENSE` & `terminusdb-client-10.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/PKG-INFO` & `terminusdb-client-10.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 Metadata-Version: 2.1
 Name: terminusdb-client
-Version: 10.2.3
+Version: 10.2.4
 Summary: Python client for Terminus DB
 Home-page: https://github.com/terminusdb/terminusdb-client-python
 Author: TerminusDB group
 Author-email: terminusdatabase@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dataframe
 License-File: LICENSE
 
 [![TerminusDB Python Client](https://assets.terminusdb.com/readmes/terminusdb-client-python/header.gif)][terminusdb-client-python-docs]
 
-[terminusdb-client-python-docs]: https://terminusdb.com/docs/guides/reference-guides/python-client-reference
+[terminusdb-client-python-docs]: https://terminusdb.com/docs/python
 
 ---
 
 [![Discord](https://img.shields.io/discord/689805612053168129?label=Discord&logo=Discord&style=plastic)](https://discord.gg/yTJKAma)
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/TerminusDB?style=social)](https://www.reddit.com/r/TerminusDB/)
 [![Twitter](https://img.shields.io/twitter/follow/terminusdb?color=skyblue&label=Follow%20on%20Twitter&logo=twitter&style=flat)](https://twitter.com/TerminusDB)
 
 [![release version](https://img.shields.io/pypi/v/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 [![downloads](https://img.shields.io/pypi/dm/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 
 [![build status](https://img.shields.io/github/workflow/status/terminusdb/terminusdb-client-python/Python%20package?logo=github)](https://github.com/terminusdb/terminusdb-client-python/actions)
-[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.com/docs/guides/reference-guides/python-client-reference)
+[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.com/docs/python)
 [![code coverage](https://codecov.io/gh/terminusdb/terminusdb-client-python/branch/main/graph/badge.svg?token=BclAUaOPnQ)](https://codecov.io/gh/terminusdb/terminusdb-client-python)
 [![license](https://img.shields.io/github/license/terminusdb/terminusdb-client-python?color=pink&logo=apache)](https://github.com/terminusdb/terminusdb-client-python/blob/main/LICENSE)
 
 > Python client for TerminusDB and TerminusCMS.
 
 [**TerminusDB**][terminusdb] is an [open-source][terminusdb-repo] graph database
 and document store. It allows you to link JSON documents in a powerful knowledge
 graph all through a simple document API.
 
 [terminusdb]: https://terminusdb.com/
 [terminusdb-docs]: https://terminusdb.com/docs/
 [terminusdb-repo]: https://github.com/terminusdb/terminusdb
 
-[**TerminusCMS**](https://terminusdb.com/terminuscms/) is a hosted headless content management system. It is built upon TerminusDB and is a developer focused data management platform for complex data and content infrastructure. [Sign up and clone a demo project to see how it works][dashboard].
+[**TerminusCMS**](https://terminusdb.com/terminuscms/) is a hosted headless content management system. It is built upon TerminusDB and is a developer-focused data management platform for complex data and content infrastructure. [Sign up and clone a demo project to see how it works][dashboard].
 
 [dashboard]: https://dashboard.terminusdb.com/
 
 ## Requirements
 
 - [TerminusDB v10.0](https://github.com/terminusdb/terminusdb-server)
 - [Python >=3.7](https://www.python.org/downloads)
 
 ## Release Notes and Previous Versions
 
 TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusCMS. Please check the [Release Notes](https://github.com/terminusdb/terminusdb-client-python/blob/master/RELEASE_NOTES.md) to find out what has changed.
 
 ## Installation
--  TerminusDB Client can be downloaded form PyPI using pip:
+-  TerminusDB Client can be downloaded from PyPI using pip:
 `python -m pip install terminusdb-client`
 
 This only includes the core Python Client (Client) and WOQLQuery.
 
-If you want to use woqlDataframe or the import and export csv function in Scaffolding CLI tool:
+If you want to use woqlDataframe or the import and export CSV function in the Scaffolding CLI tool:
 
 `python -m pip install terminusdb-client[dataframe]`
 
-*if you are installing form `zsh` you have to quote the argument like this:*
+*if you are installing from `zsh` you have to quote the argument like this:*
 
 `python -m pip install 'terminusdb-client[dataframe]'`
 
 - Install from source:
 
 `python -m pip install git+https://github.com/terminusdb/terminusdb-client-python.git`
 
@@ -89,15 +89,15 @@
 
 client = Client("http://127.0.0.1:6363/")
 client.connect()
 ```
 
 Connect to TerminusCMS
 
-*check documentation for TerminusCMS about how to add the [API token](https://terminusdb.com/docs/terminuscms/get-api-key) to the environment variable*
+*check the documentation for TerminusCMS about how to add the [API token](https://terminusdb.com/docs/how-to-connect-terminuscms) to the environment variable*
 
 
 ```Python
 from terminusdb_client import Client
 
 team="MyTeam"
 client = Client(f"https://dashboard.terminusdb.com/{team}/")
@@ -123,15 +123,15 @@
     species: str
     age: int
     weight: float
 
 my_schema.commit(client)
 ```
 
-#### Create and insert doucments
+#### Create and insert documents
 
 ```Python
 my_dog = Pet(name="Honda", species="Huskey", age=3, weight=21.1)
 my_cat = Pet(name="Tiger", species="Bengal cat", age=5, weight=4.5)
 client.insert_document([my_dog, my_cat])
 ```
 
@@ -166,15 +166,15 @@
 ![Scaffolding Demo gif](https://github.com/terminusdb/terminusdb-web-assets/blob/master/images/terminusdb%20python%20v10%20scaffolding%20demo%202.gif)
 
 Start a project in the directory
 
 ```bash
 $ tdbpy startproject
 Please enter a project name (this will also be the database name): mydb
-Please enter a endpoint location (press enter to use localhost default) [http://127.0.0.1:6363/]:
+Please enter an endpoint location (press enter to use localhost default) [http://127.0.0.1:6363/]:
 config.json and schema.py created, please customize them to start your project.
 ```
 
 Import a CSV named `grades.csv`
 
 ``` bash
 $ tdbpy importcsv grades.csv --na=error
@@ -192,23 +192,23 @@
 [{'@id': 'Grades/Android_Electric_087-65-4321_42.0_23.0_36.0_45.0_47.0_B-', '@type': 'Grades', 'final': 47.0, 'first_name': 'Electric', 'grade': 'B-', 'last_name': 'Android', 'ssn': '087-65-4321', 'test1': 42.0, 'test2': 23.0, 'test3': 36.0, 'test4': 45.0}, {'@id': 'Grades/Elephant_Ima_456-71-9012_45.0_1.0_78.0_88.0_77.0_B-', '@type': 'Grades', 'final': 77.0, 'first_name': 'Ima', 'grade': 'B-', 'last_name': 'Elephant', 'ssn': '456-71-9012', 'test1': 45.0, 'test2': 1.0, 'test3': 78.0, 'test4': 88.0}, {'@id': 'Grades/Franklin_Benny_234-56-2890_50.0_1.0_90.0_80.0_90.0_B-', '@type': 'Grades', 'final': 90.0, 'first_name': 'Benny', 'grade': 'B-', 'last_name': 'Franklin', 'ssn': '234-56-2890', 'test1': 50.0, 'test2': 1.0, 'test3': 90.0, 'test4': 80.0}]
 ```
 
 Delete the database
 
 ```bash
 $ tdbpy deletedb
-Do you want to delete 'mydb'? WARNING: This opertation is non-reversible. [y/N]: y
+Do you want to delete 'mydb'? WARNING: This operation is non-reversible. [y/N]: y
 mydb deleted.
 ```
 
-### Please check the [full Documentation](https://terminusdb.com/docs/guides/reference-guides/python-client-reference) for more information.
+### Please check the [full Documentation](https://terminusdb.com/docs/python) for more information.
 
 ## Guides & Tutorials
 
-Visit our documentation for a range of short how to guides, [how-to use the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-the-python-client) and [how to use the collaboration features with the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-collaboration-features/with-the-python-client). Alternatively, undertake the  [Getting Started with the Python Client Tutorial Series.](https://github.com/terminusdb/terminusdb-tutorials/blob/main/getting_started/python-client/README.md).
+Visit our documentation for a range of short how-to guides, [how-to use the Python Client](https://terminusdb.com/docs/use-the-python-client) and [how to use the collaboration features with the Python Client](https://terminusdb.com/docs/collaboration-with-python-client). Alternatively, undertake the  [Getting Started with the Python Client Tutorial Series.](https://github.com/terminusdb/terminusdb-tutorials/blob/main/getting_started/python-client/README.md).
 
 ## Testing
 
 1. Clone this repository
 `git clone https://github.com/terminusdb/terminusdb-client-python.git`
 
 2. Install all development dependencies using poetry
@@ -240,15 +240,15 @@
 `git clone https://github.com/terminusdb/terminusdb-client-python.git`
 
 2. Install all development dependencies
 ```sh
 $ make init
 ```
 
-3. Change directory to docs
+3. Change the directory to docs
 ```sh
 $ cd docs/
 ```
 
 4. Build with Sphinx
 ```sh
 $ make html
@@ -261,15 +261,15 @@
 If you encounter any issues, please [report them](https://github.com/terminusdb/terminusdb-client-python/issues) with your os and environment setup, the version that you are using and a simple reproducible case.
 
 If you have other questions, you can ask in our community [community Subreddit](https://www.reddit.com/r/TerminusDB/) or [Discord server](https://discord.gg/Gvdqw97).
 
 ## Community
 
 Come visit us on our [discord server](https://discord.gg/yTJKAma)
-or our [community Subreddit](https://www.reddit.com/r/TerminusDB/). We are also on [twitter](https://twitter.com/TerminusDB)
+or our [community Subreddit](https://www.reddit.com/r/TerminusDB/). We are also on [Twitter](https://twitter.com/TerminusDB)
 <img align="right" src="https://assets.terminusdb.com/images/TerminusDB%20color%20mascot.png" width="256px"/>
 
 ## Contribute
 
 It will be nice, if you open an issue first so that we can know what is going on, then, fork this repo and push in your ideas. Do not forget to add some test(s) of what value you adding.
 
 Please check [CONTRIBUTING.md](https://github.com/terminusdb/terminusdb-client-python/blob/master/CONTRIBUTING.md) for more information.
```

### Comparing `terminusdb-client-10.2.3/README.md` & `terminusdb-client-10.2.4/terminusdb_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,74 @@
+Metadata-Version: 2.1
+Name: terminusdb-client
+Version: 10.2.4
+Summary: Python client for Terminus DB
+Home-page: https://github.com/terminusdb/terminusdb-client-python
+Author: TerminusDB group
+Author-email: terminusdatabase@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dataframe
+License-File: LICENSE
+
 [![TerminusDB Python Client](https://assets.terminusdb.com/readmes/terminusdb-client-python/header.gif)][terminusdb-client-python-docs]
 
-[terminusdb-client-python-docs]: https://terminusdb.com/docs/guides/reference-guides/python-client-reference
+[terminusdb-client-python-docs]: https://terminusdb.com/docs/python
 
 ---
 
 [![Discord](https://img.shields.io/discord/689805612053168129?label=Discord&logo=Discord&style=plastic)](https://discord.gg/yTJKAma)
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/TerminusDB?style=social)](https://www.reddit.com/r/TerminusDB/)
 [![Twitter](https://img.shields.io/twitter/follow/terminusdb?color=skyblue&label=Follow%20on%20Twitter&logo=twitter&style=flat)](https://twitter.com/TerminusDB)
 
 [![release version](https://img.shields.io/pypi/v/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 [![downloads](https://img.shields.io/pypi/dm/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 
 [![build status](https://img.shields.io/github/workflow/status/terminusdb/terminusdb-client-python/Python%20package?logo=github)](https://github.com/terminusdb/terminusdb-client-python/actions)
-[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.com/docs/guides/reference-guides/python-client-reference)
+[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.com/docs/python)
 [![code coverage](https://codecov.io/gh/terminusdb/terminusdb-client-python/branch/main/graph/badge.svg?token=BclAUaOPnQ)](https://codecov.io/gh/terminusdb/terminusdb-client-python)
 [![license](https://img.shields.io/github/license/terminusdb/terminusdb-client-python?color=pink&logo=apache)](https://github.com/terminusdb/terminusdb-client-python/blob/main/LICENSE)
 
 > Python client for TerminusDB and TerminusCMS.
 
 [**TerminusDB**][terminusdb] is an [open-source][terminusdb-repo] graph database
 and document store. It allows you to link JSON documents in a powerful knowledge
 graph all through a simple document API.
 
 [terminusdb]: https://terminusdb.com/
 [terminusdb-docs]: https://terminusdb.com/docs/
 [terminusdb-repo]: https://github.com/terminusdb/terminusdb
 
-[**TerminusCMS**](https://terminusdb.com/terminuscms/) is a hosted headless content management system. It is built upon TerminusDB and is a developer focused data management platform for complex data and content infrastructure. [Sign up and clone a demo project to see how it works][dashboard].
+[**TerminusCMS**](https://terminusdb.com/terminuscms/) is a hosted headless content management system. It is built upon TerminusDB and is a developer-focused data management platform for complex data and content infrastructure. [Sign up and clone a demo project to see how it works][dashboard].
 
 [dashboard]: https://dashboard.terminusdb.com/
 
 ## Requirements
 
 - [TerminusDB v10.0](https://github.com/terminusdb/terminusdb-server)
 - [Python >=3.7](https://www.python.org/downloads)
 
 ## Release Notes and Previous Versions
 
-TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusCMS. Please check the [Release Notes](RELEASE_NOTES.md) to find out what has changed.
+TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusCMS. Please check the [Release Notes](https://github.com/terminusdb/terminusdb-client-python/blob/master/RELEASE_NOTES.md) to find out what has changed.
 
 ## Installation
--  TerminusDB Client can be downloaded form PyPI using pip:
+-  TerminusDB Client can be downloaded from PyPI using pip:
 `python -m pip install terminusdb-client`
 
 This only includes the core Python Client (Client) and WOQLQuery.
 
-If you want to use woqlDataframe or the import and export csv function in Scaffolding CLI tool:
+If you want to use woqlDataframe or the import and export CSV function in the Scaffolding CLI tool:
 
 `python -m pip install terminusdb-client[dataframe]`
 
-*if you are installing form `zsh` you have to quote the argument like this:*
+*if you are installing from `zsh` you have to quote the argument like this:*
 
 `python -m pip install 'terminusdb-client[dataframe]'`
 
 - Install from source:
 
 `python -m pip install git+https://github.com/terminusdb/terminusdb-client-python.git`
 
@@ -74,15 +89,15 @@
 
 client = Client("http://127.0.0.1:6363/")
 client.connect()
 ```
 
 Connect to TerminusCMS
 
-*check documentation for TerminusCMS about how to add the [API token](https://terminusdb.com/docs/terminuscms/get-api-key) to the environment variable*
+*check the documentation for TerminusCMS about how to add the [API token](https://terminusdb.com/docs/how-to-connect-terminuscms) to the environment variable*
 
 
 ```Python
 from terminusdb_client import Client
 
 team="MyTeam"
 client = Client(f"https://dashboard.terminusdb.com/{team}/")
@@ -108,15 +123,15 @@
     species: str
     age: int
     weight: float
 
 my_schema.commit(client)
 ```
 
-#### Create and insert doucments
+#### Create and insert documents
 
 ```Python
 my_dog = Pet(name="Honda", species="Huskey", age=3, weight=21.1)
 my_cat = Pet(name="Tiger", species="Bengal cat", age=5, weight=4.5)
 client.insert_document([my_dog, my_cat])
 ```
 
@@ -151,15 +166,15 @@
 ![Scaffolding Demo gif](https://github.com/terminusdb/terminusdb-web-assets/blob/master/images/terminusdb%20python%20v10%20scaffolding%20demo%202.gif)
 
 Start a project in the directory
 
 ```bash
 $ tdbpy startproject
 Please enter a project name (this will also be the database name): mydb
-Please enter a endpoint location (press enter to use localhost default) [http://127.0.0.1:6363/]:
+Please enter an endpoint location (press enter to use localhost default) [http://127.0.0.1:6363/]:
 config.json and schema.py created, please customize them to start your project.
 ```
 
 Import a CSV named `grades.csv`
 
 ``` bash
 $ tdbpy importcsv grades.csv --na=error
@@ -177,23 +192,23 @@
 [{'@id': 'Grades/Android_Electric_087-65-4321_42.0_23.0_36.0_45.0_47.0_B-', '@type': 'Grades', 'final': 47.0, 'first_name': 'Electric', 'grade': 'B-', 'last_name': 'Android', 'ssn': '087-65-4321', 'test1': 42.0, 'test2': 23.0, 'test3': 36.0, 'test4': 45.0}, {'@id': 'Grades/Elephant_Ima_456-71-9012_45.0_1.0_78.0_88.0_77.0_B-', '@type': 'Grades', 'final': 77.0, 'first_name': 'Ima', 'grade': 'B-', 'last_name': 'Elephant', 'ssn': '456-71-9012', 'test1': 45.0, 'test2': 1.0, 'test3': 78.0, 'test4': 88.0}, {'@id': 'Grades/Franklin_Benny_234-56-2890_50.0_1.0_90.0_80.0_90.0_B-', '@type': 'Grades', 'final': 90.0, 'first_name': 'Benny', 'grade': 'B-', 'last_name': 'Franklin', 'ssn': '234-56-2890', 'test1': 50.0, 'test2': 1.0, 'test3': 90.0, 'test4': 80.0}]
 ```
 
 Delete the database
 
 ```bash
 $ tdbpy deletedb
-Do you want to delete 'mydb'? WARNING: This opertation is non-reversible. [y/N]: y
+Do you want to delete 'mydb'? WARNING: This operation is non-reversible. [y/N]: y
 mydb deleted.
 ```
 
-### Please check the [full Documentation](https://terminusdb.com/docs/guides/reference-guides/python-client-reference) for more information.
+### Please check the [full Documentation](https://terminusdb.com/docs/python) for more information.
 
 ## Guides & Tutorials
 
-Visit our documentation for a range of short how to guides, [how-to use the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-the-python-client) and [how to use the collaboration features with the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-collaboration-features/with-the-python-client). Alternatively, undertake the  [Getting Started with the Python Client Tutorial Series.](https://github.com/terminusdb/terminusdb-tutorials/blob/main/getting_started/python-client/README.md).
+Visit our documentation for a range of short how-to guides, [how-to use the Python Client](https://terminusdb.com/docs/use-the-python-client) and [how to use the collaboration features with the Python Client](https://terminusdb.com/docs/collaboration-with-python-client). Alternatively, undertake the  [Getting Started with the Python Client Tutorial Series.](https://github.com/terminusdb/terminusdb-tutorials/blob/main/getting_started/python-client/README.md).
 
 ## Testing
 
 1. Clone this repository
 `git clone https://github.com/terminusdb/terminusdb-client-python.git`
 
 2. Install all development dependencies using poetry
@@ -225,15 +240,15 @@
 `git clone https://github.com/terminusdb/terminusdb-client-python.git`
 
 2. Install all development dependencies
 ```sh
 $ make init
 ```
 
-3. Change directory to docs
+3. Change the directory to docs
 ```sh
 $ cd docs/
 ```
 
 4. Build with Sphinx
 ```sh
 $ make html
@@ -246,21 +261,21 @@
 If you encounter any issues, please [report them](https://github.com/terminusdb/terminusdb-client-python/issues) with your os and environment setup, the version that you are using and a simple reproducible case.
 
 If you have other questions, you can ask in our community [community Subreddit](https://www.reddit.com/r/TerminusDB/) or [Discord server](https://discord.gg/Gvdqw97).
 
 ## Community
 
 Come visit us on our [discord server](https://discord.gg/yTJKAma)
-or our [community Subreddit](https://www.reddit.com/r/TerminusDB/). We are also on [twitter](https://twitter.com/TerminusDB)
+or our [community Subreddit](https://www.reddit.com/r/TerminusDB/). We are also on [Twitter](https://twitter.com/TerminusDB)
 <img align="right" src="https://assets.terminusdb.com/images/TerminusDB%20color%20mascot.png" width="256px"/>
 
 ## Contribute
 
 It will be nice, if you open an issue first so that we can know what is going on, then, fork this repo and push in your ideas. Do not forget to add some test(s) of what value you adding.
 
-Please check [CONTRIBUTING.md](CONTRIBUTING.md) for more information.
+Please check [CONTRIBUTING.md](https://github.com/terminusdb/terminusdb-client-python/blob/master/CONTRIBUTING.md) for more information.
 
 ## Licence
 
 Apache License (Version 2.0)
 
 Copyright (c) 2019
```

### Comparing `terminusdb-client-10.2.3/pyproject.toml` & `terminusdb-client-10.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "terminusdb-client"
-version = "10.2.3"
+version = "10.2.4"
 description = "Python client for Terminus DB"
 authors = ["TerminusDB group"]
 license = "Apache Software License"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4.0"
 requests = "<2.29.2"
```

### Comparing `terminusdb-client-10.2.3/setup.cfg` & `terminusdb-client-10.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/setup.py` & `terminusdb-client-10.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 requires = ["requests", "numpydoc", "click<9.0,>=7.0", "shed", "typeguard>=2,<3", "tqdm"]
 
 extras_require = {"dataframe": ["numpy >= 1.13.0", "pandas >= 0.23.0"]}
 
 setuptools.setup(
     name="terminusdb-client",
-    version="10.2.3",
+    version="10.2.4",
     author="TerminusDB group",
     author_email="terminusdatabase@gmail.com",
     description="Python client for Terminus DB",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"": ["LICENSE"]},
     url="https://github.com/terminusdb/terminusdb-client-python",
```

### Comparing `terminusdb-client-10.2.3/terminusdb_client/client/Client.py` & `terminusdb-client-10.2.4/terminusdb_client/client/Client.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,29 +129,29 @@
 
 
 class Client:
     """Client for TerminusDB server.
 
     Attributes
     ----------
-    server_url: str
+    server_url : str
         URL of the server that this client connected.
-    api: str
+    api : str
         API endpoint for this client.
-    team: str
+    team : str
         Team that this client is using. "admin" for local dbs.
-    db: str
+    db : str
         Database that this client is connected to.
-    user: str
+    user : str
         TerminiusDB user that this client is using. "admin" for local dbs.
-    branch: str
+    branch : str
         Branch of the database that this client is connected to. Default to "main".
-    ref: str, None
+    ref : str, None
         Ref setting for the client. Default to None.
-    repo: str
+    repo : str
         Repo identifier of the database that this client is connected to. Default to "local".
     """
 
     def from_json(self, json_str):
         content = json.loads(json_str)
         if isinstance(content, dict):
             self.content = _dt_dict(content)
@@ -169,17 +169,17 @@
     ) -> None:
         r"""The Client constructor.
 
         Parameters
         ----------
         server_url : str
             URL of the server that this client will connect to.
-        user_agent: optional, str
+        user_agent : optional, str
             User agent header when making requests. Defaults to terminusdb-client-python with the version appended.
-        \**kwargs
+        **kwargs
             Extra configuration options
 
         """
         self.server_url = server_url.strip("/")
         self.api = f"{self.server_url}/api"
         self._connected = False
 
@@ -292,37 +292,37 @@
     ) -> None:
         r"""Connect to a Terminus server at the given URI with an API key.
 
         Stores the connection settings and necessary meta-data for the connected server. You need to connect before most database operations.
 
         Parameters
         ----------
-        team: str
+        team : str
             Name of the team, default to be "admin"
-        db: optional, str
+        db : optional, str
             Name of the database connected
-        remote_auth: optional, dict
+        remote_auth : optional, dict
             Remote Auth setting
-        key: optional, str
+        key : optional, str
             API key for connecting, default to be "root"
-        user: optional, str
+        user : optional, str
             Name of the user, default to be "admin"
-        use_token: bool
+        use_token : bool
             Use token to connect. If both `jwt_token` and `api_token` is not provided (None), then it will use the ENV variable TERMINUSDB_ACCESS_TOKEN to connect as the API token
-        jwt_token: optional, str
+        jwt_token : optional, str
             The Bearer JWT token to connect. Default to be None.
-        api_token: optional, strs
+        api_token : optional, strs
             The API token to connect. Default to be None.
-        branch: optional, str
+        branch : optional, str
             Branch to be connected, default to be "main"
-        ref: optional, str
+        ref : optional, str
             Ref setting
-        repo: optional, str
+        repo : optional, str
             Local or remote repo, default to be "local"
-        \**kwargs
+        **kwargs
             Extra configuration options.
 
         Examples
         --------
         >>> client = Client("http://127.0.0.1:6363")
         >>> client.connect(key="root", team="admin", user="admin", db="example_db")
         """
@@ -445,21 +445,21 @@
             team: Optional[str] = None,
             db: Optional[str] = None,
             start: int = 0,
             count: int = -1):
         """Get commit history of a database
         Parameters
         ----------
-        team: str, optional
+        team : str, optional
              The team from which the database is. Defaults to the class property.
-        db: str, optional
+        db : str, optional
              The database. Defaults to the class property.
-        start: int, optional
+        start : int, optional
              Commit index to start from. Defaults to 0.
-        count: int, optional
+        count : int, optional
              Amount of commits to get. Defaults to -1 which gets all.
 
         Returns
         -------
         list
 
              List of the following commit objects:
@@ -500,15 +500,15 @@
                "timestamp: <datetime object of the timestamp>"
              }
         }
         ```
 
         Parameters
         ----------
-        max_history: int, optional
+        max_history : int, optional
             maximum number of commit that would return, counting backwards from your current commit. Default is set to 500. It needs to be nop-negative, if input is 0 it will still give the last commit.
 
         Example
         -------
         >>> from terminusdb_client import Client
         >>> client = Client("http://127.0.0.1:6363"
         >>> client.connect(db="bank_balance_example")
@@ -729,15 +729,15 @@
 
         Parameters
         ----------
         dbid : str
             ID of the database to delete
         team : str, optional
             the team in which the database resides (defaults to "admin")
-        force: bool
+        force : bool
 
         Raises
         ------
         UserWarning
             If the value of dbid is None.
         InterfaceError
             if the client does not connect to a server.
@@ -876,17 +876,17 @@
 
         Parameters
         ----------
         document_template : dict
             Template for the document that is being retrived
         graph_type : GraphType
             Graph type, either GraphType.INSTANCE or GraphType.SCHEMA.
-        as_list: bool
+        as_list : bool
             If the result returned as list rather than an iterator.
-        get_data_version: bool
+        get_data_version : bool
             If the data version of the document(s) should be obtained. If True, the method return the result and the version as a tuple.
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a database
 
@@ -937,17 +937,17 @@
 
         Parameters
         ----------
         iri_id : str
             Iri id for the document that is to be retrieved
         graph_type : GraphType
             Graph type, either GraphType.INSTANCE or GraphType.SCHEMA.
-        get_data_version: bool
+        get_data_version : bool
             If the data version of the document(s) should be obtained. If True, the method return the result and the version as a tuple.
-        kwargs:
+        kwargs :
             Additional boolean flags for retriving. Currently avaliable: "prefixed", "minimized", "unfold"
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a database
 
@@ -989,23 +989,23 @@
 
         Parameters
         ----------
         doc_type : str
             Specific type for the docuemnts that is retriving
         graph_type : GraphType, optional
             Graph type, either GraphType.INSTANCE or GraphType.SCHEMA.
-        skip: int
+        skip : int
             The starting posiion of the returning results, default to be 0
-        count: int or None
+        count : int or None
             The maximum number of returned result, if None (default) it will return all of the avalible result.
-        as_list: bool
+        as_list : bool
             If the result returned as list rather than an iterator.
-        get_data_version: bool
+        get_data_version : bool
             If the version of the document(s) should be obtained. If True, the method return the result and the version as a tuple.
-        kwargs:
+        kwargs :
             Additional boolean flags for retriving. Currently avaliable: "prefixed", "unfold"
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a database
 
@@ -1030,23 +1030,23 @@
     ) -> Union[Iterable, list, tuple]:
         """Retrieves all avalibale the documents
 
         Parameters
         ----------
         graph_type : GraphType, optional
             Graph type, either GraphType.INSTANCE or GraphType.SCHEMA.
-        skip: int
+        skip : int
             The starting posiion of the returning results, default to be 0
-        count: int or None
+        count : int or None
             The maximum number of returned result, if None (default) it will return all of the avalible result.
-        as_list: bool
+        as_list : bool
             If the result returned as list rather than an iterator.
-        get_data_version: bool
+        get_data_version : bool
             If the version of the document(s) should be obtained. If True, the method return the result and the version as a tuple.
-        kwargs:
+        kwargs :
             Additional boolean flags for retriving. Currently avaliable: "prefixed", "unfold"
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a database
 
@@ -1161,19 +1161,19 @@
         compress: Union[str, int] = 1024,
         raw_json: bool = False
     ) -> None:
         """Inserts the specified document(s)
 
         Parameters
         ----------
-        document: dict or list of dict
+        document : dict or list of dict
             Document(s) to be inserted.
         graph_type : GraphType
             Graph type, either GraphType.INSTANCE or GraphType.SCHEMA.
-        full_replace:: bool
+        full_replace : bool
             If True then the whole graph will be replaced. WARNING: you should also supply the context object as the first element in the list of documents  if using this option.
         commit_msg : str
             Commit message.
         last_data_version : str
             Last version before the update, used to check if the document has been changed unknowingly
         compress : str or int
             If it is an integer, size of the data larger than this (in bytes) will be compress with gzip in the request (assume encoding as UTF-8, 0 = always compress). If it is `never` it will never compress the data.
@@ -1268,15 +1268,15 @@
         create: bool = False,
         raw_json: bool = False,
     ) -> dict:
         """Updates the specified document(s)
 
         Parameters
         ----------
-        document: dict or list of dict
+        document : dict or list of dict
             Document(s) to be updated.
         graph_type : GraphType
             Graph type, either GraphType.INSTANCE or GraphType.SCHEMA.
         commit_msg : str
             Commit message.
         last_data_version : str
             Last version before the update, used to check if the document has been changed unknowingly
@@ -1348,15 +1348,15 @@
         last_data_version: Optional[str] = None,
         compress: Union[str, int] = 1024,
     ) -> None:
         """Updates the specified document(s). Add the document if not existed.
 
         Parameters
         ----------
-        document: dict or list of dict
+        document : dict or list of dict
             Document(s) to be updated.
         graph_type : GraphType
             Graph type, either GraphType.INSTANCE or GraphType.SCHEMA.
         commit_msg : str
             Commit message.
         last_data_version : str
             Last version before the update, used to check if the document has been changed unknowingly
@@ -1379,15 +1379,15 @@
         commit_msg: Optional[str] = None,
         last_data_version: Optional[str] = None,
     ) -> None:
         """Delete the specified document(s)
 
         Parameters
         ----------
-        document: str or list of str
+        document : str or list of str
             Document(s) (as dictionary or DocumentTemplate objects) or id(s) of document(s) to be updated.
         graph_type : GraphType
             Graph type, either GraphType.INSTANCE or GraphType.SCHEMA.
         commit_msg : str
             Commit message.
         last_data_version : str
             Last version before the update, used to check if the document has been changed unknowingly
@@ -1430,15 +1430,15 @@
         )
 
     def has_doc(self, doc_id: str, graph_type: GraphType = GraphType.INSTANCE) -> bool:
         """Check if a certain document exist in a database
 
         Parameters
         ----------
-        doc_id: str
+        doc_id : str
             Id of document to be checked.
         graph_type : GraphType
             Graph type, either GraphType.INSTANCE or GraphType.SCHEMA.
 
         Raises
         ------
         InterfaceError
@@ -1467,15 +1467,15 @@
             raise exception
 
     def get_class_frame(self, class_name):
         """Get the frame of the class of class_name. Provide information about all the avaliable properties of that class.
 
         Parameters
         ----------
-        class_name: str
+        class_name : str
             Name of the class
 
         Returns
         -------
         dict
             Dictionary containing information
         """
@@ -1504,19 +1504,19 @@
 
         Parameters
         ----------
         woql_query : dict or WOQLQuery object
             A woql query as an object or dict
         commit_mg : str
             A message that will be written to the commit log to describe the change
-        get_data_version: bool
+        get_data_version : bool
             If the data version of the query result(s) should be obtained. If True, the method return the result and the version as a tuple.
         last_data_version : str
             Last version before the update, used to check if the document has been changed unknowingly
-        file_dict: **deprecated**
+        file_dict : **deprecated**
             File dictionary to be associated with post name => filename, for multipart POST
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a database
 
@@ -1623,21 +1623,21 @@
         message: Optional[str] = None,
         author: Optional[str] = None,
     ) -> dict:
         """Pull updates from a remote repository to the current database.
 
         Parameters
         ----------
-        remote: str
+        remote : str
             remote to pull from, default "origin"
-        remote_branch: str, optional
+        remote_branch : str, optional
             remote branch to pull from, default to be your current barnch
-        message: str, optional
+        message : str, optional
             optional commit message
-        author: str, optional
+        author : str, optional
             option to overide the author of the operation
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a database
 
@@ -1678,15 +1678,15 @@
     def fetch(self, remote_id: str,
               remote_auth: Optional[dict] = None,
               ) -> dict:
         """Fatch the brach from a remote
 
         Parameters
         ----------
-        remote_id: str
+        remote_id : str
             id of the remote
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a database"""
         self._check_connection()
@@ -1707,23 +1707,23 @@
         author: Optional[str] = None,
         remote_auth: Optional[dict] = None,
     ) -> dict:
         """Push changes from a branch to a remote repo
 
         Parameters
         ----------
-        remote: str
+        remote : str
             remote to push to, default "origin"
-        remote_branch: str, optional
+        remote_branch : str, optional
             remote branch to push to, default to be your current barnch
-        message: str, optional
+        message : str, optional
             optional commit message
-        author: str, optional
+        author : str, optional
             option to overide the author of the operation
-        remote_auth: dict, optional
+        remote_auth : dict, optional
             optional remote authorization (uses client remote auth otherwise)
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a database
 
@@ -1842,17 +1842,17 @@
 
         Notes
         -----
         The "remote" repo can live in the local database.
 
         Parameters
         ----------
-        commit: string
+        commit : string
             Commit id or path to the commit (if use_path is True), for instance '234980523ffaf93' or 'admin/database/local/commit/234980523ffaf93'. If not provided, it will reset to the newest commit (useful when need to go back after a soft reset).
-        soft: bool
+        soft : bool
             Flag indicating if the reset if soft, that is referencing to a previous commit instead of resetting to a previous commit in the backend and wipping newer commits.
         use_path : bool
             Wheather or not the commit given is an id or path. Default using id and use_path is False.
 
         Examples
         --------
         >>> client = Client("http://127.0.0.1:6363/")
@@ -2154,14 +2154,21 @@
         ],
         patch: Patch,
     ):
         """Apply the patch object to the before object and return an after object. Note that this change does not commit changes to the graph.
 
         Do not connect when using public API.
 
+        Parameters
+        ----------
+        before : dict
+            Object before to patch
+        patch : Patch
+            Patch object to apply to the dict
+
         Returns
         -------
         dict
             After object
 
         Examples
         --------
@@ -2376,15 +2383,15 @@
 
     def get_organization_users(self, org: str) -> Optional[dict]:
         """
         Returns a list of users in an organization.
 
         Parameters
         ----------
-        org: str
+        org : str
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a server
 
         Returns
@@ -2402,16 +2409,16 @@
 
     def get_organization_user(self, org: str, username: str) -> Optional[dict]:
         """
         Returns user info related to an organization.
 
         Parameters
         ----------
-        org: str
-        username: str
+        org : str
+        username : str
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a server
 
         Returns
@@ -2429,16 +2436,16 @@
 
     def get_organization_user_databases(self, org: str, username: str) -> Optional[dict]:
         """
         Returns the databases available to a user which are inside an organization
 
         Parameters
         ----------
-        org: str
-        username: str
+        org : str
+        username : str
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a server
 
         Returns
@@ -2530,15 +2537,15 @@
 
     def change_capabilities(self, capability_change: dict) -> Optional[dict]:
         """
         Change the capabilities of a certain user
 
         Parameters
         ----------
-        capability_change: dict
+        capability_change : dict
             Dict for the capability change request.
 
             Example:
             {
              "operation": "revoke",
              "scope": "UserDatabase/f5a0ef94469b32e1aee321678436c7dfd5a96d9c476672b3282ae89a45b5200e",
              "user": "User/admin",
@@ -2703,15 +2710,15 @@
         """
         Add a new user
 
         Parameters
         ----------
         username : str
             The username of the user
-        password: str
+        password : str
             The user's password
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a server
 
@@ -2805,15 +2812,15 @@
         """
         Change user's password
 
         Parameters
         ----------
         username : str
             The username of the user
-        password: str
+        password : str
             The new password
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a server
```

### Comparing `terminusdb-client-10.2.3/terminusdb_client/errors.py` & `terminusdb-client-10.2.4/terminusdb_client/errors.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/query_syntax/query_syntax.py` & `terminusdb-client-10.2.4/terminusdb_client/query_syntax/query_syntax.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/schema/schema.py` & `terminusdb-client-10.2.4/terminusdb_client/schema/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,46 @@
 from typing import List, Optional, Set, Union
 
 from numpydoc.docscrape import ClassDoc
 from typeguard import check_type
 
 from .. import woql_type as wt
 from ..client import Client, GraphType
-from ..woql_type import to_woql_type
+from ..woql_type import (  # noqa: F401
+    to_woql_type,
+    anySimpleType,
+    decimal,
+    dateTimeStamp,
+    gYear,
+    gMonth,
+    gDay,
+    gYearMonth,
+    yearMonthDuration,
+    dayTimeDuration,
+    byte,
+    short,
+    long,
+    unsignedByte,
+    unsignedShort,
+    unsignedInt,
+    unsignedLong,
+    positiveInteger,
+    negativeInteger,
+    nonPositiveInteger,
+    nonNegativeInteger,
+    base64Binary,
+    hexBinary,
+    anyURI,
+    language,
+    normalizedString,
+    token,
+    NMTOKEN,
+    Name,
+    NCName,
+)
 
 
 class TerminusKey:
     def __init__(self, keys: Union[str, list, None] = None):
         if keys is not None:
             if isinstance(keys, str):
                 self._keys = [keys]
@@ -790,15 +821,15 @@
                 if pipe:
                     return enum_dict
                 else:
                     self._construct_class(enum_dict)
                     return self.object[enum_name]._to_dict()
             # it's a List
             elif prop["type"] == "array":
-                prop_type = convert_property(prop["items"])
+                prop_type = convert_property(prop_name, prop["items"])
                 return {"@type": "List", "@class": prop_type}
             elif isinstance(prop["type"], list):
                 prop_type = prop["type"]
                 # it's Optional
                 if "null" in prop_type:
                     prop_type.remove("null")
                     prop_type = prop_type[0]  # can only have one type
```

### Comparing `terminusdb-client-10.2.3/terminusdb_client/scripts/schema_template.py` & `terminusdb-client-10.2.4/terminusdb_client/scripts/schema_template.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/scripts/scripts.py` & `terminusdb-client-10.2.4/terminusdb_client/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/AllServerRecords.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/AllServerRecords.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/DBRecord.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/DBRecord.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/ans_cardinality.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/ans_cardinality.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/ans_doctype.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/ans_doctype.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/ans_insert.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/ans_insert.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/ans_property.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/ans_property.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/ans_triple_quad.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/ans_triple_quad.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/conftest.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/connectCapabilitiesResponse.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/connectCapabilitiesResponse.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/connectionObjDump.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/connectionObjDump.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/getSchemaTurtleResponse.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/getSchemaTurtleResponse.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/conftest.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/mock_jsons.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/mock_jsons.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_client.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_schema.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_scripts.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/integration_tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/mockResponse.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/mockResponse.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/serverRecordsFromCap.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/serverRecordsFromCap.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/test_Client.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/test_Client.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/test_Schema.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/test_Schema.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/test_backwardsCompat.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/test_backwardsCompat.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/test_scripts.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/test_woqlExtra.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/test_woqlExtra.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/test_woqlQuery.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/test_woqlQuery.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlAndJson.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlAndJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlDeleteJson.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlDeleteJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlDoctypeJson.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlDoctypeJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlExtraJson.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlExtraJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlIdgenJson.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlIdgenJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlJoinSplitJson.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlJoinSplitJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlJson.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlMathJson.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlMathJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlOrJson.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlOrJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlSelectJson.py` & `terminusdb-client-10.2.4/terminusdb_client/tests/woqljson/woqlSelectJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/woql_utils.py` & `terminusdb-client-10.2.4/terminusdb_client/woql_utils.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/woqldataframe/woqlDataframe.py` & `terminusdb-client-10.2.4/terminusdb_client/woqldataframe/woqlDataframe.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/woqlquery/woql_core.py` & `terminusdb-client-10.2.4/terminusdb_client/woqlquery/woql_core.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client/woqlquery/woql_query.py` & `terminusdb-client-10.2.4/terminusdb_client/woqlquery/woql_query.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.3/terminusdb_client.egg-info/PKG-INFO` & `terminusdb-client-10.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,59 @@
-Metadata-Version: 2.1
-Name: terminusdb-client
-Version: 10.2.3
-Summary: Python client for Terminus DB
-Home-page: https://github.com/terminusdb/terminusdb-client-python
-Author: TerminusDB group
-Author-email: terminusdatabase@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dataframe
-License-File: LICENSE
-
 [![TerminusDB Python Client](https://assets.terminusdb.com/readmes/terminusdb-client-python/header.gif)][terminusdb-client-python-docs]
 
-[terminusdb-client-python-docs]: https://terminusdb.com/docs/guides/reference-guides/python-client-reference
+[terminusdb-client-python-docs]: https://terminusdb.com/docs/python
 
 ---
 
 [![Discord](https://img.shields.io/discord/689805612053168129?label=Discord&logo=Discord&style=plastic)](https://discord.gg/yTJKAma)
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/TerminusDB?style=social)](https://www.reddit.com/r/TerminusDB/)
 [![Twitter](https://img.shields.io/twitter/follow/terminusdb?color=skyblue&label=Follow%20on%20Twitter&logo=twitter&style=flat)](https://twitter.com/TerminusDB)
 
 [![release version](https://img.shields.io/pypi/v/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 [![downloads](https://img.shields.io/pypi/dm/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 
 [![build status](https://img.shields.io/github/workflow/status/terminusdb/terminusdb-client-python/Python%20package?logo=github)](https://github.com/terminusdb/terminusdb-client-python/actions)
-[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.com/docs/guides/reference-guides/python-client-reference)
+[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.com/docs/python)
 [![code coverage](https://codecov.io/gh/terminusdb/terminusdb-client-python/branch/main/graph/badge.svg?token=BclAUaOPnQ)](https://codecov.io/gh/terminusdb/terminusdb-client-python)
 [![license](https://img.shields.io/github/license/terminusdb/terminusdb-client-python?color=pink&logo=apache)](https://github.com/terminusdb/terminusdb-client-python/blob/main/LICENSE)
 
 > Python client for TerminusDB and TerminusCMS.
 
 [**TerminusDB**][terminusdb] is an [open-source][terminusdb-repo] graph database
 and document store. It allows you to link JSON documents in a powerful knowledge
 graph all through a simple document API.
 
 [terminusdb]: https://terminusdb.com/
 [terminusdb-docs]: https://terminusdb.com/docs/
 [terminusdb-repo]: https://github.com/terminusdb/terminusdb
 
-[**TerminusCMS**](https://terminusdb.com/terminuscms/) is a hosted headless content management system. It is built upon TerminusDB and is a developer focused data management platform for complex data and content infrastructure. [Sign up and clone a demo project to see how it works][dashboard].
+[**TerminusCMS**](https://terminusdb.com/terminuscms/) is a hosted headless content management system. It is built upon TerminusDB and is a developer-focused data management platform for complex data and content infrastructure. [Sign up and clone a demo project to see how it works][dashboard].
 
 [dashboard]: https://dashboard.terminusdb.com/
 
 ## Requirements
 
 - [TerminusDB v10.0](https://github.com/terminusdb/terminusdb-server)
 - [Python >=3.7](https://www.python.org/downloads)
 
 ## Release Notes and Previous Versions
 
-TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusCMS. Please check the [Release Notes](https://github.com/terminusdb/terminusdb-client-python/blob/master/RELEASE_NOTES.md) to find out what has changed.
+TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusCMS. Please check the [Release Notes](RELEASE_NOTES.md) to find out what has changed.
 
 ## Installation
--  TerminusDB Client can be downloaded form PyPI using pip:
+-  TerminusDB Client can be downloaded from PyPI using pip:
 `python -m pip install terminusdb-client`
 
 This only includes the core Python Client (Client) and WOQLQuery.
 
-If you want to use woqlDataframe or the import and export csv function in Scaffolding CLI tool:
+If you want to use woqlDataframe or the import and export CSV function in the Scaffolding CLI tool:
 
 `python -m pip install terminusdb-client[dataframe]`
 
-*if you are installing form `zsh` you have to quote the argument like this:*
+*if you are installing from `zsh` you have to quote the argument like this:*
 
 `python -m pip install 'terminusdb-client[dataframe]'`
 
 - Install from source:
 
 `python -m pip install git+https://github.com/terminusdb/terminusdb-client-python.git`
 
@@ -89,15 +74,15 @@
 
 client = Client("http://127.0.0.1:6363/")
 client.connect()
 ```
 
 Connect to TerminusCMS
 
-*check documentation for TerminusCMS about how to add the [API token](https://terminusdb.com/docs/terminuscms/get-api-key) to the environment variable*
+*check the documentation for TerminusCMS about how to add the [API token](https://terminusdb.com/docs/how-to-connect-terminuscms) to the environment variable*
 
 
 ```Python
 from terminusdb_client import Client
 
 team="MyTeam"
 client = Client(f"https://dashboard.terminusdb.com/{team}/")
@@ -123,15 +108,15 @@
     species: str
     age: int
     weight: float
 
 my_schema.commit(client)
 ```
 
-#### Create and insert doucments
+#### Create and insert documents
 
 ```Python
 my_dog = Pet(name="Honda", species="Huskey", age=3, weight=21.1)
 my_cat = Pet(name="Tiger", species="Bengal cat", age=5, weight=4.5)
 client.insert_document([my_dog, my_cat])
 ```
 
@@ -166,15 +151,15 @@
 ![Scaffolding Demo gif](https://github.com/terminusdb/terminusdb-web-assets/blob/master/images/terminusdb%20python%20v10%20scaffolding%20demo%202.gif)
 
 Start a project in the directory
 
 ```bash
 $ tdbpy startproject
 Please enter a project name (this will also be the database name): mydb
-Please enter a endpoint location (press enter to use localhost default) [http://127.0.0.1:6363/]:
+Please enter an endpoint location (press enter to use localhost default) [http://127.0.0.1:6363/]:
 config.json and schema.py created, please customize them to start your project.
 ```
 
 Import a CSV named `grades.csv`
 
 ``` bash
 $ tdbpy importcsv grades.csv --na=error
@@ -192,23 +177,23 @@
 [{'@id': 'Grades/Android_Electric_087-65-4321_42.0_23.0_36.0_45.0_47.0_B-', '@type': 'Grades', 'final': 47.0, 'first_name': 'Electric', 'grade': 'B-', 'last_name': 'Android', 'ssn': '087-65-4321', 'test1': 42.0, 'test2': 23.0, 'test3': 36.0, 'test4': 45.0}, {'@id': 'Grades/Elephant_Ima_456-71-9012_45.0_1.0_78.0_88.0_77.0_B-', '@type': 'Grades', 'final': 77.0, 'first_name': 'Ima', 'grade': 'B-', 'last_name': 'Elephant', 'ssn': '456-71-9012', 'test1': 45.0, 'test2': 1.0, 'test3': 78.0, 'test4': 88.0}, {'@id': 'Grades/Franklin_Benny_234-56-2890_50.0_1.0_90.0_80.0_90.0_B-', '@type': 'Grades', 'final': 90.0, 'first_name': 'Benny', 'grade': 'B-', 'last_name': 'Franklin', 'ssn': '234-56-2890', 'test1': 50.0, 'test2': 1.0, 'test3': 90.0, 'test4': 80.0}]
 ```
 
 Delete the database
 
 ```bash
 $ tdbpy deletedb
-Do you want to delete 'mydb'? WARNING: This opertation is non-reversible. [y/N]: y
+Do you want to delete 'mydb'? WARNING: This operation is non-reversible. [y/N]: y
 mydb deleted.
 ```
 
-### Please check the [full Documentation](https://terminusdb.com/docs/guides/reference-guides/python-client-reference) for more information.
+### Please check the [full Documentation](https://terminusdb.com/docs/python) for more information.
 
 ## Guides & Tutorials
 
-Visit our documentation for a range of short how to guides, [how-to use the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-the-python-client) and [how to use the collaboration features with the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-collaboration-features/with-the-python-client). Alternatively, undertake the  [Getting Started with the Python Client Tutorial Series.](https://github.com/terminusdb/terminusdb-tutorials/blob/main/getting_started/python-client/README.md).
+Visit our documentation for a range of short how-to guides, [how-to use the Python Client](https://terminusdb.com/docs/use-the-python-client) and [how to use the collaboration features with the Python Client](https://terminusdb.com/docs/collaboration-with-python-client). Alternatively, undertake the  [Getting Started with the Python Client Tutorial Series.](https://github.com/terminusdb/terminusdb-tutorials/blob/main/getting_started/python-client/README.md).
 
 ## Testing
 
 1. Clone this repository
 `git clone https://github.com/terminusdb/terminusdb-client-python.git`
 
 2. Install all development dependencies using poetry
@@ -240,15 +225,15 @@
 `git clone https://github.com/terminusdb/terminusdb-client-python.git`
 
 2. Install all development dependencies
 ```sh
 $ make init
 ```
 
-3. Change directory to docs
+3. Change the directory to docs
 ```sh
 $ cd docs/
 ```
 
 4. Build with Sphinx
 ```sh
 $ make html
@@ -261,21 +246,21 @@
 If you encounter any issues, please [report them](https://github.com/terminusdb/terminusdb-client-python/issues) with your os and environment setup, the version that you are using and a simple reproducible case.
 
 If you have other questions, you can ask in our community [community Subreddit](https://www.reddit.com/r/TerminusDB/) or [Discord server](https://discord.gg/Gvdqw97).
 
 ## Community
 
 Come visit us on our [discord server](https://discord.gg/yTJKAma)
-or our [community Subreddit](https://www.reddit.com/r/TerminusDB/). We are also on [twitter](https://twitter.com/TerminusDB)
+or our [community Subreddit](https://www.reddit.com/r/TerminusDB/). We are also on [Twitter](https://twitter.com/TerminusDB)
 <img align="right" src="https://assets.terminusdb.com/images/TerminusDB%20color%20mascot.png" width="256px"/>
 
 ## Contribute
 
 It will be nice, if you open an issue first so that we can know what is going on, then, fork this repo and push in your ideas. Do not forget to add some test(s) of what value you adding.
 
-Please check [CONTRIBUTING.md](https://github.com/terminusdb/terminusdb-client-python/blob/master/CONTRIBUTING.md) for more information.
+Please check [CONTRIBUTING.md](CONTRIBUTING.md) for more information.
 
 ## Licence
 
 Apache License (Version 2.0)
 
 Copyright (c) 2019
```

### Comparing `terminusdb-client-10.2.3/terminusdb_client.egg-info/SOURCES.txt` & `terminusdb-client-10.2.4/terminusdb_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

