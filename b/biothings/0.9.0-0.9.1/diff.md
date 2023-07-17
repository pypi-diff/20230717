# Comparing `tmp/biothings-0.9.0.tar.gz` & `tmp/biothings-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biothings-0.9.0.tar", last modified: Sun Feb 21 20:34:52 2021, max compression
+gzip compressed data, was "dist/biothings-0.9.1.tar", last modified: Thu Mar 11 01:00:23 2021, max compression
```

## Comparing `biothings-0.9.0.tar` & `biothings-0.9.1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/
--rw-r--r--   0 root         (0) root         (0)       89 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/.git-info
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/utils/
--rw-r--r--   0 root         (0) root         (0)    12842 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/hub_db.py
--rw-r--r--   0 root         (0) root         (0)      528 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/slack.py
--rw-r--r--   0 root         (0) root         (0)     1999 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/dotfield.py
--rw-r--r--   0 root         (0) root         (0)    33614 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/dataload.py
--rw-r--r--   0 root         (0) root         (0)    33585 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/hub.py
--rw-r--r--   0 root         (0) root         (0)     2448 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/parallel.py
--rw-r--r--   0 root         (0) root         (0)     6688 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/loggers.py
--rw-r--r--   0 root         (0) root         (0)    23639 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/inspect.py
--rw-r--r--   0 root         (0) root         (0)     7996 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/jsonschema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/utils/web/
--rw-r--r--   0 root         (0) root         (0)      640 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/web/run.py
--rw-r--r--   0 root         (0) root         (0)     4265 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/web/es_transport.py
--rw-r--r--   0 root         (0) root         (0)     3817 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/web/analytics.py
--rw-r--r--   0 root         (0) root         (0)     6991 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/web/tracking.py
--rw-r--r--   0 root         (0) root         (0)      327 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2460 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/web/userquery.py
--rw-r--r--   0 root         (0) root         (0)     3196 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/web/es_connection.py
--rw-r--r--   0 root         (0) root         (0)     3279 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/web/es.py
--rw-r--r--   0 root         (0) root         (0)    19751 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/web/swagger.py
--rw-r--r--   0 root         (0) root         (0)     1963 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/web/es_dsl.py
--rw-r--r--   0 root         (0) root         (0)    27940 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/jsonpatch.py
--rw-r--r--   0 root         (0) root         (0)     3608 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/dotstring.py
--rw-r--r--   0 root         (0) root         (0)    12277 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/parallel_mp.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11778 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/backend.py
--rw-r--r--   0 root         (0) root         (0)     2775 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/redis.py
--rw-r--r--   0 root         (0) root         (0)     9605 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/jsondiff.py
--rw-r--r--   0 root         (0) root         (0)    10926 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/diff.py
--rw-r--r--   0 root         (0) root         (0)    48776 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/manager.py
--rw-r--r--   0 root         (0) root         (0)    36465 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/es.py
--rw-r--r--   0 root         (0) root         (0)    10666 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/version.py
--rw-r--r--   0 root         (0) root         (0)    26310 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     8116 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/aws.py
--rw-r--r--   0 root         (0) root         (0)    18961 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/mongo.py
--rw-r--r--   0 root         (0) root         (0)     1651 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/exclude_ids.py
--rw-r--r--   0 root         (0) root         (0)     8742 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/sqlite3.py
--rw-r--r--   0 root         (0) root         (0)     4290 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/shelve.py
--rw-r--r--   0 root         (0) root         (0)     3752 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/utils/doc_traversal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/web/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/web/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      852 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/utils.py
--rw-r--r--   0 root         (0) root         (0)    21477 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/options.py
--rw-r--r--   0 root         (0) root         (0)     4535 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/web/handlers/
--rw-r--r--   0 root         (0) root         (0)     9542 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/handlers/api.py
--rw-r--r--   0 root         (0) root         (0)       57 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4099 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/handlers/base.py
--rw-r--r--   0 root         (0) root         (0)    11059 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/handlers/es.py
--rw-r--r--   0 root         (0) root         (0)      606 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/handlers/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/web/pipeline/
--rw-r--r--   0 root         (0) root         (0)      111 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3688 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/pipeline/execute.py
--rw-r--r--   0 root         (0) root         (0)    11662 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/pipeline/transform.py
--rw-r--r--   0 root         (0) root         (0)     6629 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/pipeline/build.py
--rw-r--r--   0 root         (0) root         (0)     2380 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/index_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/web/settings/
--rw-r--r--   0 root         (0) root         (0)    14670 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/settings/data.py
--rw-r--r--   0 root         (0) root         (0)       86 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/settings/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7569 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/settings/default.py
--rw-r--r--   0 root         (0) root         (0)     3484 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/settings/descriptions.py
--rw-r--r--   0 root         (0) root         (0)    10839 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/web/settings/settings.py
--rw-r--r--   0 root         (0) root         (0)    25266 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4221 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/tests/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/datainspect/
--rw-r--r--   0 root         (0) root         (0)    14504 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datainspect/inspector.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datainspect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/datarelease/
--rw-r--r--   0 root         (0) root         (0)      359 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datarelease/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9162 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datarelease/releasenote.py
--rw-r--r--   0 root         (0) root         (0)    82039 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datarelease/publisher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/dataload/
--rw-r--r--   0 root         (0) root         (0)    52014 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataload/dumper.py
--rw-r--r--   0 root         (0) root         (0)     1318 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataload/sync.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataload/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2052 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataload/validator.py
--rw-r--r--   0 root         (0) root         (0)    35148 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataload/uploader.py
--rw-r--r--   0 root         (0) root         (0)    15926 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataload/source.py
--rw-r--r--   0 root         (0) root         (0)    11351 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataload/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/datatransform/
--rw-r--r--   0 root         (0) root         (0)    18086 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datatransform/datatransform_mdb.py
--rw-r--r--   0 root         (0) root         (0)    22311 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datatransform/datatransform.py
--rw-r--r--   0 root         (0) root         (0)     2198 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datatransform/ciidstruct.py
--rw-r--r--   0 root         (0) root         (0)     1149 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datatransform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17864 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datatransform/datatransform_api.py
--rw-r--r--   0 root         (0) root         (0)     1155 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/datatransform/histogram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/autoupdate/
--rw-r--r--   0 root         (0) root         (0)    26714 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/autoupdate/dumper.py
--rw-r--r--   0 root         (0) root         (0)      286 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/autoupdate/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10136 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/autoupdate/uploader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/dataindex/
--rw-r--r--   0 root         (0) root         (0)    19442 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataindex/snapshooter.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataindex/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45291 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataindex/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1066 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataindex/idcache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/dataplugin/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataplugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1201 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataplugin/manager.py
--rw-r--r--   0 root         (0) root         (0)    42116 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataplugin/assistant.py
--rw-r--r--   0 root         (0) root         (0)    69419 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/databuild/
--rw-r--r--   0 root         (0) root         (0)     8241 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/databuild/buildconfig.py
--rw-r--r--   0 root         (0) root         (0)    59337 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/databuild/differ.py
--rw-r--r--   0 root         (0) root         (0)    40593 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/databuild/syncer.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/databuild/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2869 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/databuild/mapper.py
--rw-r--r--   0 root         (0) root         (0)    15458 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/databuild/backend.py
--rw-r--r--   0 root         (0) root         (0)    72670 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/databuild/builder.py
--rw-r--r--   0 root         (0) root         (0)     2356 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/databuild/prebuilder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/dataexport/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataexport/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6152 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/dataexport/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/standalone/
--rw-r--r--   0 root         (0) root         (0)     9028 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/standalone/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/api/
--rw-r--r--   0 root         (0) root         (0)    11512 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/hub/api/handlers/
--rw-r--r--   0 root         (0) root         (0)     1332 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/api/handlers/shell.py
--rw-r--r--   0 root         (0) root         (0)     1589 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/api/handlers/log.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/api/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3182 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/api/handlers/base.py
--rw-r--r--   0 root         (0) root         (0)     3615 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/api/handlers/ws.py
--rw-r--r--   0 root         (0) root         (0)     3764 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/api/handlers/upload.py
--rw-r--r--   0 root         (0) root         (0)     4768 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/api/manager.py
--rw-r--r--   0 root         (0) root         (0)     5812 2021-02-21 20:33:47.000000 biothings-0.9.0/biothings/hub/upgrade.py
--rw-r--r--   0 root         (0) root         (0)      114 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings/schema/
--rw-r--r--   0 root         (0) root         (0)     1039 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/schema/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4255 2021-02-21 20:33:48.000000 biothings-0.9.0/biothings/schema/temp_schema.py
--rw-r--r--   0 root         (0) root         (0)      199 2021-02-21 20:34:52.000000 biothings-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4632 2021-02-21 20:33:49.000000 biothings-0.9.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      114 2021-02-21 20:33:47.000000 biothings-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6432 2021-02-21 20:34:52.000000 biothings-0.9.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings.egg-info/
--rw-r--r--   0 root         (0) root         (0)       10 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     3841 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      870 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     6432 2021-02-21 20:34:52.000000 biothings-0.9.0/biothings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4496 2021-02-21 20:33:47.000000 biothings-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)     4496 2021-03-11 00:59:17.000000 biothings-0.9.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     6432 2021-03-11 01:00:23.000000 biothings-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4632 2021-03-11 00:59:18.000000 biothings-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      870 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     6432 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     3841 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      199 2021-03-11 01:00:23.000000 biothings-0.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/schema/
+-rw-r--r--   0 root         (0) root         (0)     1039 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/schema/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4255 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/schema/temp_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/datatransform/
+-rw-r--r--   0 root         (0) root         (0)     1155 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datatransform/histogram.py
+-rw-r--r--   0 root         (0) root         (0)    18086 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datatransform/datatransform_mdb.py
+-rw-r--r--   0 root         (0) root         (0)    22311 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datatransform/datatransform.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datatransform/ciidstruct.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datatransform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17864 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datatransform/datatransform_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/autoupdate/
+-rw-r--r--   0 root         (0) root         (0)    10136 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/autoupdate/uploader.py
+-rw-r--r--   0 root         (0) root         (0)      286 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/autoupdate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26714 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/autoupdate/dumper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/dataindex/
+-rw-r--r--   0 root         (0) root         (0)     1066 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataindex/idcache.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataindex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45291 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataindex/indexer.py
+-rw-r--r--   0 root         (0) root         (0)    19442 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataindex/snapshooter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/datainspect/
+-rw-r--r--   0 root         (0) root         (0)    14504 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datainspect/inspector.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datainspect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/datarelease/
+-rw-r--r--   0 root         (0) root         (0)    82039 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datarelease/publisher.py
+-rw-r--r--   0 root         (0) root         (0)      359 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datarelease/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9162 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/datarelease/releasenote.py
+-rw-r--r--   0 root         (0) root         (0)    69419 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/standalone/
+-rw-r--r--   0 root         (0) root         (0)     9028 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/standalone/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/dataexport/
+-rw-r--r--   0 root         (0) root         (0)     6152 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataexport/ids.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataexport/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5812 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/upgrade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/dataplugin/
+-rw-r--r--   0 root         (0) root         (0)    42116 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataplugin/assistant.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataplugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1201 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataplugin/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/dataload/
+-rw-r--r--   0 root         (0) root         (0)    35148 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataload/uploader.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataload/sync.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataload/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15926 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataload/source.py
+-rw-r--r--   0 root         (0) root         (0)    52014 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataload/dumper.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataload/validator.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/dataload/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/databuild/
+-rw-r--r--   0 root         (0) root         (0)    59337 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/databuild/differ.py
+-rw-r--r--   0 root         (0) root         (0)    72670 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/databuild/builder.py
+-rw-r--r--   0 root         (0) root         (0)    15458 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/databuild/backend.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/databuild/prebuilder.py
+-rw-r--r--   0 root         (0) root         (0)     2869 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/databuild/mapper.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/databuild/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40593 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/databuild/syncer.py
+-rw-r--r--   0 root         (0) root         (0)     8241 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/databuild/buildconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/api/
+-rw-r--r--   0 root         (0) root         (0)    11512 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/hub/api/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1589 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/api/handlers/log.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/api/handlers/shell.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/api/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3615 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/api/handlers/ws.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/api/handlers/upload.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/api/handlers/base.py
+-rw-r--r--   0 root         (0) root         (0)     4768 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/hub/api/manager.py
+-rw-r--r--   0 root         (0) root         (0)    25266 2021-03-11 00:59:17.000000 biothings-0.9.1/biothings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/web/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/web/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      852 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/utils.py
+-rw-r--r--   0 root         (0) root         (0)    21697 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/options.py
+-rw-r--r--   0 root         (0) root         (0)     4535 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/web/settings/
+-rw-r--r--   0 root         (0) root         (0)    14670 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/settings/data.py
+-rw-r--r--   0 root         (0) root         (0)    10839 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/settings/settings.py
+-rw-r--r--   0 root         (0) root         (0)     7569 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/settings/default.py
+-rw-r--r--   0 root         (0) root         (0)     3484 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/settings/descriptions.py
+-rw-r--r--   0 root         (0) root         (0)       86 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/settings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/web/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     3688 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/pipeline/execute.py
+-rw-r--r--   0 root         (0) root         (0)      111 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6910 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/pipeline/build.py
+-rw-r--r--   0 root         (0) root         (0)    11955 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/pipeline/transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/web/handlers/
+-rw-r--r--   0 root         (0) root         (0)      606 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/handlers/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9542 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/handlers/api.py
+-rw-r--r--   0 root         (0) root         (0)       57 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/handlers/base.py
+-rw-r--r--   0 root         (0) root         (0)    11059 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/handlers/es.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/web/index_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/tests/
+-rw-r--r--   0 root         (0) root         (0)     4221 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/tests/web.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/utils/
+-rw-r--r--   0 root         (0) root         (0)    18961 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/mongo.py
+-rw-r--r--   0 root         (0) root         (0)     6688 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/loggers.py
+-rw-r--r--   0 root         (0) root         (0)    26310 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)    23639 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/inspect.py
+-rw-r--r--   0 root         (0) root         (0)     8116 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/aws.py
+-rw-r--r--   0 root         (0) root         (0)    33614 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/dataload.py
+-rw-r--r--   0 root         (0) root         (0)     3608 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/dotstring.py
+-rw-r--r--   0 root         (0) root         (0)    27940 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/jsonpatch.py
+-rw-r--r--   0 root         (0) root         (0)    11778 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/backend.py
+-rw-r--r--   0 root         (0) root         (0)     3752 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/doc_traversal.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/redis.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/shelve.py
+-rw-r--r--   0 root         (0) root         (0)     7996 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/jsonschema.py
+-rw-r--r--   0 root         (0) root         (0)    12277 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/parallel_mp.py
+-rw-r--r--   0 root         (0) root         (0)     9605 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/jsondiff.py
+-rw-r--r--   0 root         (0) root         (0)    33585 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/hub.py
+-rw-r--r--   0 root         (0) root         (0)    10926 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/diff.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12842 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/hub_db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/utils/web/
+-rw-r--r--   0 root         (0) root         (0)     3817 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/web/analytics.py
+-rw-r--r--   0 root         (0) root         (0)    19751 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/web/swagger.py
+-rw-r--r--   0 root         (0) root         (0)      327 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/web/es_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/web/userquery.py
+-rw-r--r--   0 root         (0) root         (0)     4265 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/web/es_transport.py
+-rw-r--r--   0 root         (0) root         (0)     6991 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/web/tracking.py
+-rw-r--r--   0 root         (0) root         (0)      640 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/web/run.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/web/es_dsl.py
+-rw-r--r--   0 root         (0) root         (0)     3279 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/web/es.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/dotfield.py
+-rw-r--r--   0 root         (0) root         (0)     8742 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/sqlite3.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/exclude_ids.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/parallel.py
+-rw-r--r--   0 root         (0) root         (0)    48776 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/manager.py
+-rw-r--r--   0 root         (0) root         (0)    36465 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/es.py
+-rw-r--r--   0 root         (0) root         (0)    10666 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/version.py
+-rw-r--r--   0 root         (0) root         (0)      528 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/utils/slack.py
+-rw-r--r--   0 root         (0) root         (0)      114 2021-03-11 00:59:18.000000 biothings-0.9.1/biothings/version.py
+-rw-r--r--   0 root         (0) root         (0)       89 2021-03-11 01:00:23.000000 biothings-0.9.1/biothings/.git-info
+-rw-r--r--   0 root         (0) root         (0)      114 2021-03-11 00:59:17.000000 biothings-0.9.1/MANIFEST.in
```

### Comparing `biothings-0.9.0/biothings/utils/hub_db.py` & `biothings-0.9.1/biothings/utils/hub_db.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/slack.py` & `biothings-0.9.1/biothings/utils/slack.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/dotfield.py` & `biothings-0.9.1/biothings/utils/dotfield.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/dataload.py` & `biothings-0.9.1/biothings/utils/dataload.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/hub.py` & `biothings-0.9.1/biothings/utils/hub.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/parallel.py` & `biothings-0.9.1/biothings/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/loggers.py` & `biothings-0.9.1/biothings/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/inspect.py` & `biothings-0.9.1/biothings/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/jsonschema.py` & `biothings-0.9.1/biothings/utils/jsonschema.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/web/run.py` & `biothings-0.9.1/biothings/utils/web/run.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/web/es_transport.py` & `biothings-0.9.1/biothings/utils/web/es_transport.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/web/analytics.py` & `biothings-0.9.1/biothings/utils/web/analytics.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/web/tracking.py` & `biothings-0.9.1/biothings/utils/web/tracking.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/web/userquery.py` & `biothings-0.9.1/biothings/utils/web/userquery.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/web/es_connection.py` & `biothings-0.9.1/biothings/utils/web/es_connection.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/web/es.py` & `biothings-0.9.1/biothings/utils/web/es.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/web/swagger.py` & `biothings-0.9.1/biothings/utils/web/swagger.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/web/es_dsl.py` & `biothings-0.9.1/biothings/utils/web/es_dsl.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/jsonpatch.py` & `biothings-0.9.1/biothings/utils/jsonpatch.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/dotstring.py` & `biothings-0.9.1/biothings/utils/dotstring.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/parallel_mp.py` & `biothings-0.9.1/biothings/utils/parallel_mp.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/backend.py` & `biothings-0.9.1/biothings/utils/backend.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/redis.py` & `biothings-0.9.1/biothings/utils/redis.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/jsondiff.py` & `biothings-0.9.1/biothings/utils/jsondiff.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/diff.py` & `biothings-0.9.1/biothings/utils/diff.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/manager.py` & `biothings-0.9.1/biothings/utils/manager.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/es.py` & `biothings-0.9.1/biothings/utils/es.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/version.py` & `biothings-0.9.1/biothings/utils/version.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/common.py` & `biothings-0.9.1/biothings/utils/common.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/aws.py` & `biothings-0.9.1/biothings/utils/aws.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/mongo.py` & `biothings-0.9.1/biothings/utils/mongo.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/exclude_ids.py` & `biothings-0.9.1/biothings/utils/exclude_ids.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/sqlite3.py` & `biothings-0.9.1/biothings/utils/sqlite3.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/shelve.py` & `biothings-0.9.1/biothings/utils/shelve.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/utils/doc_traversal.py` & `biothings-0.9.1/biothings/utils/doc_traversal.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/utils.py` & `biothings-0.9.1/biothings/web/utils.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/options.py` & `biothings-0.9.1/biothings/web/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 import logging
 import re
 from collections import UserDict, abc, defaultdict, namedtuple
 from functools import partial
 from types import MappingProxyType
 
 try:
-    from functools import singledispatchmethod
+    from re import Pattern  # py>=3.7
+except ImportError:
+    from typing import Pattern
+
+try:
+    from functools import singledispatchmethod  # py>=3.7
 except ImportError:
     from singledispatchmethod import singledispatchmethod
 
 from biothings.utils.common import dotdict, split_ids
 
 
 class OptionError(ValueError):
@@ -44,15 +49,15 @@
 
         self.translations = []
 
         if isinstance(translations, dict):
             translations = translations.items()
 
         for pattern, repl in translations:
-            if hasattr(re, "Pattern") and isinstance(pattern, re.Pattern): # PY3.6 COMPATIBILITY
+            if isinstance(pattern, Pattern):
                 self.translations.append(
                     (pattern, repl))
             elif isinstance(pattern, tuple):
                 self.translations.append(
                     (re.compile(*pattern), repl))
             elif isinstance(pattern, str):
                 self.translations.append(
@@ -245,14 +250,18 @@
 
         if self.strict:
             # since JSON support value types
             # strict mode enforces it and essentially
             # makes this step a validation step.
             raise OptionError(f"Expect type {to_type.__name__}.")
 
+        # mostly for biothings client 0.2.3 compatibility
+        if isinstance(value, str) and to_type is list:
+            return self.str_to_list(value)
+
         return self.to_type(value, to_type)
 
     def to_type(self, val, type_):
 
         if issubclass(type_, (list, tuple, set)) and not self.strict:
             val = (val, )  # "abc" -> ["abc"] instead of ["a", "b", "c"]
 
@@ -356,15 +365,15 @@
         self.keyword = defdict.get('keyword')
         self.path = defdict.get('path')
         aliases = defdict.get('alias', [])
 
         assert isinstance(self.path, (str, int, type(None)))
         assert isinstance(self.keyword, (str, type(None)))
 
-        if isinstance(aliases, list):
+        if isinstance(aliases, (list, tuple)):
             self.aliases = aliases
         elif isinstance(aliases, str):
             self.aliases = [aliases]
         else:  # validation failed
             raise ValueError("Unknown Alias.")
 
     @singledispatchmethod
```

### Comparing `biothings-0.9.0/biothings/web/__init__.py` & `biothings-0.9.1/biothings/web/__init__.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/handlers/api.py` & `biothings-0.9.1/biothings/web/handlers/api.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/handlers/base.py` & `biothings-0.9.1/biothings/web/handlers/base.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/handlers/es.py` & `biothings-0.9.1/biothings/web/handlers/es.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/handlers/exceptions.py` & `biothings-0.9.1/biothings/web/handlers/exceptions.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/pipeline/execute.py` & `biothings-0.9.1/biothings/web/pipeline/execute.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/pipeline/transform.py` & `biothings-0.9.1/biothings/web/pipeline/transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
     # for compatibility
     traverse = staticmethod(traverse)
 
     def transform(self, response, options):
         """
         Transform the query response to a user-friendly structure.
+        Mainly deconstruct the elasticsearch response structure and
+        hand over to transform_doc to apply the options below.
 
         Options:
             dotfield: flatten a dictionary using dotfield notation
             _sorted: sort keys alaphabetically in ascending order
             always_list: ensure the fields specified are lists or wrapped in a list
             allow_null: ensure the fields specified are present in the result,
                         the fields may be provided as type None or [].
@@ -68,31 +70,42 @@
         if isinstance(response, dict):
             response.update(response.pop('hits', {}))  # collapse one level
             response.pop('_shards')
             response.pop('timed_out')
             if 'hits' in response:
                 for hit in response['hits']:
                     hit.update(hit.pop('_source', {}))  # collapse one level
-                    for path, obj in self.traverse(hit):
-                        self.transform_hit(path, obj, options)
-                        if options.allow_null:
-                            self.option_allow_null(path, obj, options.allow_null)
-                        if options.always_list:
-                            self.option_always_list(path, obj, options.always_list)
-                        if options._sorted:
-                            self.option_sorted(path, obj)
-                    if options.dotfield:
-                        self.option_dotfield(hit, options)
+                    self.transform_doc(hit, options)
             if 'aggregations' in response:
                 self.transform_aggs(response['aggregations'])
                 response['facets'] = response.pop('aggregations')
                 response['hits'] = response.pop('hits')  # order
             return response
         return {}
 
+    def transform_doc(self, doc, options):
+        """
+        In-place apply a variety of transformations to a document like:
+        {
+            "_id": ... ,
+            "_index": ... ,
+            ...
+        }
+        """
+        for path, obj in self.traverse(doc):
+            self.transform_hit(path, obj, options)
+            if options.allow_null:
+                self.option_allow_null(path, obj, options.allow_null)
+            if options.always_list:
+                self.option_always_list(path, obj, options.always_list)
+            if options._sorted:
+                self.option_sorted(path, obj)
+        if options.dotfield:
+            self.option_dotfield(doc, options)
+
     @staticmethod
     def option_allow_null(path, obj, fields):
         """
         The specified fields should be set to None if it does not exist.
         When flattened, the field could be converted to an empty list.
         """
         if isinstance(obj, dict):
```

### Comparing `biothings-0.9.0/biothings/web/pipeline/build.py` & `biothings-0.9.1/biothings/web/pipeline/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,28 +55,30 @@
 
             if options.scopes is not None:
                 build_query = self._build_match_query
             else:  # no scopes, only q
                 build_query = self._build_string_query
 
             if isinstance(q, list):
+                if not q:  # es cannot execute empty multisearch
+                    raise ValueError("No search terms.")
                 search = AsyncMultiSearch()
                 for _q in q:
                     _search = build_query(_q, options)
                     _search = self._apply_extras(_search, options)
                     search = search.add(_search)
             else:  # str, int ...
                 search = build_query(str(q), options)
                 # pass through es query options. (from, size ...)
                 search = self._apply_extras(search, options)
 
         except (TypeError, ValueError) as exc:
             raise BadRequest(reason=type(exc).__name__, details=str(exc))
         except IllegalOperation as exc:
-            raise BadRequest(reason=str(exc)) # ex. sorting by -_score
+            raise BadRequest(reason=str(exc))  # ex. sorting by -_score
         else:
             return search
 
     def default_string_query(self, q, options):
         """
         Override this to customize default string query.
         By default it implements a query string query.
@@ -95,16 +97,17 @@
         return search
 
     def default_match_query(self, q, scopes, options):
         """
         Override this to customize default match query.
         By default it implements a multi_match query.
         """
-        if isinstance(q, (str, int, float)):
-            query = Q('multi_match', query=str(q),
+
+        if isinstance(q, (str, int, float, bool)):
+            query = Q('multi_match', query=q,
                       operator="and", fields=scopes,
                       lenient=True)
 
         elif isinstance(q, list):
             if not isinstance(scopes, list):
                 raise TypeError(scopes)
             if len(q) != len(scopes):
@@ -128,15 +131,18 @@
             options:
                 userquery
         """
         assert isinstance(q, str)
         search = AsyncSearch()
         userquery = options.userquery or ''
 
-        if self.user_query.has_query(userquery):
+        if not q:  # same empty q behavior as that of ES.
+            search = search.query("match_none")
+
+        elif self.user_query.has_query(userquery):
             userquery_ = self.user_query.get_query(userquery, q=q)
             search = search.query(userquery_)
 
         else:  # customization here
             search = self.default_string_query(q, options)
 
         if self.user_query.has_filter(userquery):
@@ -148,14 +154,16 @@
     def _build_match_query(self, q, options):
         """ q + options -> query object
 
             options:
                 scopes - default scopes
                 regexs - q -> scopes override
         """
+
+        # takes care of implied scopes from q
         scopes = options.scopes or []
         if isinstance(q, str):
             for regex, scope in options.regexs or []:
                 match = re.fullmatch(regex, q)
                 if match:
                     q = match.groupdict().get('search_term') or q
                     scopes = scope if isinstance(scope, list) else [scope]
```

### Comparing `biothings-0.9.0/biothings/web/index_base.py` & `biothings-0.9.1/biothings/web/index_base.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/settings/data.py` & `biothings-0.9.1/biothings/web/settings/data.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/settings/default.py` & `biothings-0.9.1/biothings/web/settings/default.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/settings/descriptions.py` & `biothings-0.9.1/biothings/web/settings/descriptions.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/web/settings/settings.py` & `biothings-0.9.1/biothings/web/settings/settings.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -171,16 +171,16 @@
             setting = rule[2] if len(rule) == 3 else {}
             assert handler, rule[1]
             if issubclass(handler, BaseAPIHandler) and handler.name:
                 handler_name = handler.name
                 handler_options = handler.kwargs
                 setting_attr = '_'.join((handler_name, 'kwargs')).upper()
                 setting_options = getattr(self, setting_attr, {})
-                self.optionsets.add(handler_name, handler_options, handler.kwarg_groups)
                 self.optionsets.add(handler_name, setting_options)
+                self.optionsets.add(handler_name, handler_options, handler.kwarg_groups)
             if '{typ}' in pattern:
                 if not issubclass(handler, BaseESRequestHandler):
                     raise BiothingConfigError()
                 for biothing_type in self.BIOTHING_TYPES:
                     _pattern = pattern.format(
                         pre=self.API_PREFIX,
                         ver=self.API_VERSION,
```

### Comparing `biothings-0.9.0/biothings/__init__.py` & `biothings-0.9.1/biothings/__init__.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/tests/web.py` & `biothings-0.9.1/biothings/tests/web.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/datainspect/inspector.py` & `biothings-0.9.1/biothings/hub/datainspect/inspector.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/datarelease/releasenote.py` & `biothings-0.9.1/biothings/hub/datarelease/releasenote.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/datarelease/publisher.py` & `biothings-0.9.1/biothings/hub/datarelease/publisher.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataload/dumper.py` & `biothings-0.9.1/biothings/hub/dataload/dumper.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataload/sync.py` & `biothings-0.9.1/biothings/hub/dataload/sync.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataload/validator.py` & `biothings-0.9.1/biothings/hub/dataload/validator.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataload/uploader.py` & `biothings-0.9.1/biothings/hub/dataload/uploader.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataload/source.py` & `biothings-0.9.1/biothings/hub/dataload/source.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataload/storage.py` & `biothings-0.9.1/biothings/hub/dataload/storage.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/datatransform/datatransform_mdb.py` & `biothings-0.9.1/biothings/hub/datatransform/datatransform_mdb.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/datatransform/datatransform.py` & `biothings-0.9.1/biothings/hub/datatransform/datatransform.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/datatransform/ciidstruct.py` & `biothings-0.9.1/biothings/hub/datatransform/ciidstruct.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/datatransform/__init__.py` & `biothings-0.9.1/biothings/hub/datatransform/__init__.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/datatransform/datatransform_api.py` & `biothings-0.9.1/biothings/hub/datatransform/datatransform_api.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/datatransform/histogram.py` & `biothings-0.9.1/biothings/hub/datatransform/histogram.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/autoupdate/dumper.py` & `biothings-0.9.1/biothings/hub/autoupdate/dumper.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/autoupdate/uploader.py` & `biothings-0.9.1/biothings/hub/autoupdate/uploader.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataindex/snapshooter.py` & `biothings-0.9.1/biothings/hub/dataindex/snapshooter.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataindex/indexer.py` & `biothings-0.9.1/biothings/hub/dataindex/indexer.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataindex/idcache.py` & `biothings-0.9.1/biothings/hub/dataindex/idcache.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataplugin/manager.py` & `biothings-0.9.1/biothings/hub/dataplugin/manager.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataplugin/assistant.py` & `biothings-0.9.1/biothings/hub/dataplugin/assistant.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/__init__.py` & `biothings-0.9.1/biothings/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/databuild/buildconfig.py` & `biothings-0.9.1/biothings/hub/databuild/buildconfig.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/databuild/differ.py` & `biothings-0.9.1/biothings/hub/databuild/differ.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/databuild/syncer.py` & `biothings-0.9.1/biothings/hub/databuild/syncer.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/databuild/mapper.py` & `biothings-0.9.1/biothings/hub/databuild/mapper.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/databuild/backend.py` & `biothings-0.9.1/biothings/hub/databuild/backend.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/databuild/builder.py` & `biothings-0.9.1/biothings/hub/databuild/builder.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/databuild/prebuilder.py` & `biothings-0.9.1/biothings/hub/databuild/prebuilder.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/dataexport/ids.py` & `biothings-0.9.1/biothings/hub/dataexport/ids.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/standalone/__init__.py` & `biothings-0.9.1/biothings/hub/standalone/__init__.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/api/__init__.py` & `biothings-0.9.1/biothings/hub/api/__init__.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/api/handlers/shell.py` & `biothings-0.9.1/biothings/hub/api/handlers/shell.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/api/handlers/log.py` & `biothings-0.9.1/biothings/hub/api/handlers/log.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/api/handlers/base.py` & `biothings-0.9.1/biothings/hub/api/handlers/base.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/api/handlers/ws.py` & `biothings-0.9.1/biothings/hub/api/handlers/ws.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/api/handlers/upload.py` & `biothings-0.9.1/biothings/hub/api/handlers/upload.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/api/manager.py` & `biothings-0.9.1/biothings/hub/api/manager.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/hub/upgrade.py` & `biothings-0.9.1/biothings/hub/upgrade.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/schema/utils.py` & `biothings-0.9.1/biothings/schema/utils.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings/schema/temp_schema.py` & `biothings-0.9.1/biothings/schema/temp_schema.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/setup.py` & `biothings-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/PKG-INFO` & `biothings-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biothings
-Version: 0.9.0
+Version: 0.9.1
 Summary: a toolkit for building high-performance data APIs in biology
 Home-page: https://github.com/biothings/biothings.api
 Author: Cyrus Afrasiabi, Sebastien Lelong, Xinghua Zhou, Chunlei Wu
 Author-email: cwu@scripps.edu
 License: Apache License, Version 2.0
 Description: [![Downloads](https://pepy.tech/badge/biothings)](https://pepy.tech/project/biothings)
         [![biothings package](https://badge.fury.io/py/biothings.svg)](https://pypi.python.org/pypi/biothings)
```

### Comparing `biothings-0.9.0/biothings.egg-info/SOURCES.txt` & `biothings-0.9.1/biothings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings.egg-info/requires.txt` & `biothings-0.9.1/biothings.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `biothings-0.9.0/biothings.egg-info/PKG-INFO` & `biothings-0.9.1/biothings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biothings
-Version: 0.9.0
+Version: 0.9.1
 Summary: a toolkit for building high-performance data APIs in biology
 Home-page: https://github.com/biothings/biothings.api
 Author: Cyrus Afrasiabi, Sebastien Lelong, Xinghua Zhou, Chunlei Wu
 Author-email: cwu@scripps.edu
 License: Apache License, Version 2.0
 Description: [![Downloads](https://pepy.tech/badge/biothings)](https://pepy.tech/project/biothings)
         [![biothings package](https://badge.fury.io/py/biothings.svg)](https://pypi.python.org/pypi/biothings)
```

### Comparing `biothings-0.9.0/README.md` & `biothings-0.9.1/README.md`

 * *Files identical despite different names*

