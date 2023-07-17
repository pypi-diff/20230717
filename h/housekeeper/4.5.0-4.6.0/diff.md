# Comparing `tmp/housekeeper-4.5.0.tar.gz` & `tmp/housekeeper-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/housekeeper-4.5.0.tar", last modified: Mon May 29 14:16:59 2023, max compression
+gzip compressed data, was "dist/housekeeper-4.6.0.tar", last modified: Mon Jul 17 13:09:56 2023, max compression
```

## Comparing `housekeeper-4.5.0.tar` & `housekeeper-4.6.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-29 14:16:47.000000 housekeeper-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-29 14:16:47.000000 housekeeper-4.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-29 14:16:59.000000 housekeeper-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-29 14:16:47.000000 housekeeper-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/archive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/include.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/include.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/store/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/archive_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-29 14:16:47.000000 housekeeper-4.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-29 14:16:47.000000 housekeeper-4.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 14:16:59.000000 housekeeper-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-29 14:16:47.000000 housekeeper-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/add/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/add/test_cli_add_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/add/test_cli_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/add/test_cli_add_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/add/test_cli_add_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/delete/test_cli_delete_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/delete/test_cli_delete_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/delete/test_cli_delete_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/delete/test_cli_delete_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/get/test_get_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/get/test_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/get/test_get_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/get/test_get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/test_cli_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/test_cli_include.py
--rw-r--r--   0 runner    (1001) docker     (123)    15721 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/fixtures/sequencing_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/sequencing_files/lane1.spring
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/sequencing_files/lane2.spring
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/fixtures/vcfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/vcfs/example.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/vcfs/example.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/vcfs/family.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/vcfs/family.3.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/vcfs/family.vcf
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_archive_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_version_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/store/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/handlers/test_createhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/handlers/test_readhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/handlers/test_updatehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/test_include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-17 13:09:45.000000 housekeeper-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-17 13:09:45.000000 housekeeper-4.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-17 13:09:56.000000 housekeeper-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-17 13:09:45.000000 housekeeper-4.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/archive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/cli/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/cli/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/cli/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/api/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper/store/api/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/api/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/api/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/api/handlers/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/api/handlers/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/api/handlers/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/api/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/filters/archive_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/filters/bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/filters/file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/filters/tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/filters/version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/filters/version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-17 13:09:45.000000 housekeeper-4.6.0/housekeeper/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 13:09:56.000000 housekeeper-4.6.0/housekeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 13:09:45.000000 housekeeper-4.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 13:09:45.000000 housekeeper-4.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-17 13:09:56.000000 housekeeper-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-17 13:09:45.000000 housekeeper-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/add/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/add/test_cli_add_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/add/test_cli_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/add/test_cli_add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/add/test_cli_add_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/delete/test_cli_delete_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/delete/test_cli_delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/delete/test_cli_delete_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/delete/test_cli_delete_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/get/test_get_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/get/test_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/get/test_get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/get/test_get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/test_cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/cli/test_cli_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15721 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/fixtures/sequencing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/fixtures/sequencing_files/lane1.spring
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/fixtures/sequencing_files/lane2.spring
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/fixtures/vcfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/fixtures/vcfs/example.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/fixtures/vcfs/example.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/fixtures/vcfs/family.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/fixtures/vcfs/family.3.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/fixtures/vcfs/family.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/filters/test_archive_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/filters/test_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/filters/test_file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/filters/test_tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/filters/test_version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/filters/test_version_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:09:56.000000 housekeeper-4.6.0/tests/store/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/handlers/test_createhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/handlers/test_readhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/handlers/test_updatehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/store/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-17 13:09:45.000000 housekeeper-4.6.0/tests/test_include.py
```

### Comparing `housekeeper-4.5.0/LICENSE` & `housekeeper-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/PKG-INFO` & `housekeeper-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.5.0
+Version: 4.6.0
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.5.0/README.md` & `housekeeper-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/cli/add.py` & `housekeeper-4.6.0/housekeeper/cli/add.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/cli/core.py` & `housekeeper-4.6.0/housekeeper/cli/core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/cli/delete.py` & `housekeeper-4.6.0/housekeeper/cli/delete.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/cli/get.py` & `housekeeper-4.6.0/housekeeper/cli/get.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/cli/include.py` & `housekeeper-4.6.0/housekeeper/cli/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/cli/init.py` & `housekeeper-4.6.0/housekeeper/cli/init.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/cli/tables.py` & `housekeeper-4.6.0/housekeeper/cli/tables.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/date.py` & `housekeeper-4.6.0/housekeeper/date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/files.py` & `housekeeper-4.6.0/housekeeper/files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/include.py` & `housekeeper-4.6.0/housekeeper/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/api/core.py` & `housekeeper-4.6.0/housekeeper/store/api/core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/api/handlers/base.py` & `housekeeper-4.6.0/housekeeper/store/api/handlers/base.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/api/handlers/create.py` & `housekeeper-4.6.0/housekeeper/store/api/handlers/create.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/api/handlers/read.py` & `housekeeper-4.6.0/housekeeper/store/api/handlers/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 """
 This module handles finding things in the store/database
 """
 import datetime as dt
 import logging
 from pathlib import Path
 from typing import List, Optional, Set
-from sqlalchemy.orm import Query, Session
 
+from housekeeper.store.api.handlers.base import BaseHandler
+from housekeeper.store.filters.archive_filters import ArchiveFilter, apply_archive_filter
 from housekeeper.store.filters.bundle_filters import BundleFilters, apply_bundle_filter
-from housekeeper.store.filters.file_filters import (
-    FileFilter,
-    apply_file_filter,
-)
+from housekeeper.store.filters.file_filters import FileFilter, apply_file_filter
+from housekeeper.store.filters.tag_filters import TagFilter, apply_tag_filter
 from housekeeper.store.filters.version_bundle_filters import (
     VersionBundleFilters,
     apply_version_bundle_filter,
 )
-from housekeeper.store.filters.version_filters import (
-    VersionFilter,
-    apply_version_filter,
-)
-from housekeeper.store.models import Bundle, File, Tag, Version, Archive
-from housekeeper.store.filters.tag_filters import TagFilter, apply_tag_filter
-
-from housekeeper.store.api.handlers.base import BaseHandler
-from housekeeper.store.filters.archive_filters import (
-    apply_archive_filter,
-    ArchiveFilter,
-)
+from housekeeper.store.filters.version_filters import VersionFilter, apply_version_filter
+from housekeeper.store.models import Archive, Bundle, File, Tag, Version
+from sqlalchemy import exists
+from sqlalchemy.orm import Query, Session, aliased
 
 LOG = logging.getLogger(__name__)
 
 
 class ReadHandler(BaseHandler):
     """Handler for searching the database"""
 
@@ -196,21 +187,21 @@
             ],
             is_archived=True,
             tag_names=tags,
         ).all()
 
     def get_non_archived_files(self, bundle_name: str, tags: Optional[List]) -> List[File]:
         """Returns all files in the given bundle, with the given tags, and are not archived."""
-        files_filtered_om_bundle: Query = apply_bundle_filter(
+        files_filtered_on_bundle: Query = apply_bundle_filter(
             bundles=self._get_join_file_tags_archive_query(),
             bundle_name=bundle_name,
             filter_functions=[BundleFilters.FILTER_BY_NAME],
         )
         return apply_file_filter(
-            files=files_filtered_om_bundle,
+            files=files_filtered_on_bundle,
             filter_functions=[
                 FileFilter.FILTER_FILES_BY_TAGS,
                 FileFilter.FILTER_FILES_BY_IS_ARCHIVED,
             ],
             is_archived=False,
             tag_names=tags,
         ).all()
@@ -232,7 +223,23 @@
         return {
             archive.retrieval_task_id
             for archive in apply_archive_filter(
                 archives=self._get_query(table=Archive),
                 filter_functions=[ArchiveFilter.FILTER_RETRIEVAL_ONGOING],
             ).all()
         }
+
+    def get_bundle_name_from_file_path(self, file_path: str) -> str:
+        """Return the bundle name for the specified file."""
+        return self.get_files(file_path=file_path).first().version.bundle.name
+
+    def get_all_non_archived_files(self, tag_names: List[str]) -> List[File]:
+        """Return all spring files which are not marked as archived in Housekeeper."""
+        return apply_file_filter(
+            self._get_join_file_tags_archive_query(),
+            filter_functions=[
+                FileFilter.FILTER_FILES_BY_TAGS,
+                FileFilter.FILTER_FILES_BY_IS_ARCHIVED,
+            ],
+            tag_names=tag_names,
+            is_archived=False,
+        ).all()
```

### Comparing `housekeeper-4.5.0/housekeeper/store/api/handlers/update.py` & `housekeeper-4.6.0/housekeeper/store/api/handlers/update.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/api/schema.py` & `housekeeper-4.6.0/housekeeper/store/api/schema.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/filters/archive_filters.py` & `housekeeper-4.6.0/housekeeper/store/filters/archive_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/filters/bundle_filters.py` & `housekeeper-4.6.0/housekeeper/store/filters/bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/filters/file_filters.py` & `housekeeper-4.6.0/housekeeper/store/filters/file_filters.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 from typing import Callable, List, Optional
-from sqlalchemy import func as sqlalchemy_func
-from sqlalchemy.orm import Query
 
 from housekeeper.store.models import File, Tag
+from sqlalchemy import func as sqlalchemy_func
+from sqlalchemy.orm import Query
 
 
 def filter_files_by_id(files: Query, file_id: int, **kwargs) -> Query:
     """Filter files by file id."""
     return files.filter(File.id == file_id)
```

### Comparing `housekeeper-4.5.0/housekeeper/store/filters/tag_filters.py` & `housekeeper-4.6.0/housekeeper/store/filters/tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/filters/version_bundle_filters.py` & `housekeeper-4.6.0/housekeeper/store/filters/version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/filters/version_filters.py` & `housekeeper-4.6.0/housekeeper/store/filters/version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/housekeeper/store/models.py` & `housekeeper-4.6.0/housekeeper/store/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Module for the models"""
 
 import datetime as dt
 from pathlib import Path
 
-from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import Column, ForeignKey, Table, UniqueConstraint, orm, types
+from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import backref
 
 Model = declarative_base()
 
 file_tag_link = Table(
     "file_tag_link",
     Model.metadata,
     Column("file_id", types.Integer, ForeignKey("file.id"), nullable=False),
     Column("tag_id", types.Integer, ForeignKey("tag.id"), nullable=False),
     UniqueConstraint("file_id", "tag_id", name="_file_tag_uc"),
 )
 
 
 class Archive(Model):
-    """Information regarding the archival of a file."""
+    """Information regarding the archiving of a file."""
 
     __tablename__ = "archive"
     archiving_task_id = Column(types.Integer, nullable=False)
     retrieval_task_id = Column(types.Integer, nullable=True)
     file_id = Column(ForeignKey("file.id"), nullable=False, primary_key=True)
     archived_at = Column(types.DateTime(), nullable=True)
     retrieved_at = Column(types.DateTime(), nullable=True)
```

### Comparing `housekeeper-4.5.0/housekeeper.egg-info/PKG-INFO` & `housekeeper-4.6.0/housekeeper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.5.0
+Version: 4.6.0
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.5.0/housekeeper.egg-info/SOURCES.txt` & `housekeeper-4.6.0/housekeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/setup.py` & `housekeeper-4.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 setup(
     name=NAME,
     # Versions should comply with PEP440. For a discussion on
     # single-sourcing the version across setup.py and the project code,
     # see http://packaging.python.org/en/latest/tutorial.html#version
-    version="4.5.0",
+    version="4.6.0",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     # What does your project relate to? Separate with spaces.
     keywords="housekeeper development",
     author=AUTHOR,
     author_email=EMAIL,
```

### Comparing `housekeeper-4.5.0/tests/cli/add/conftest.py` & `housekeeper-4.6.0/tests/cli/add/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/add/test_cli_add_bundle.py` & `housekeeper-4.6.0/tests/cli/add/test_cli_add_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/add/test_cli_add_file.py` & `housekeeper-4.6.0/tests/cli/add/test_cli_add_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from click import Context
 from click.testing import CliRunner
 from housekeeper.cli.add import file_cmd
 from housekeeper.store import Store
 from housekeeper.store.models import Bundle, Version
 
+NEW_FILE_ADDED: str = "new file added"
+
 
 def test_add_file_non_existing_bundle(
     base_context: Context,
     cli_runner: CliRunner,
     case_id: str,
     second_sample_vcf: Path,
     caplog,
@@ -69,27 +71,27 @@
 
 
 def test_add_non_existing_file(base_context: Context, cli_runner: CliRunner, caplog):
     """Test to add a file without specifying any input"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a empty store and a cli runner
     non_existing = Path("hello.txt")
-    assert non_existing.exists() is False
+    assert not non_existing.exists()
 
     # WHEN trying to add a bundle
     result = cli_runner.invoke(file_cmd, [str(non_existing)], obj=base_context)
 
     # THEN assert it fails since there is no valid input
     assert result.exit_code == 1
     # THEN check that the proper information is displayed
     assert f"File: {non_existing} does not exist" in caplog.text
 
 
 def test_add_file_existing_bundle_with_include(
-    populated_context: Context,
+    populated_context: dict,
     cli_runner: CliRunner,
     case_id: str,
     second_sample_vcf: Path,
     caplog,
     housekeeper_version_dir: Path,
     project_dir: Path,
 ):
@@ -108,15 +110,15 @@
         [str(second_sample_vcf), "-b", bundle_name],
         obj=populated_context,
     )
 
     # THEN assert it succedes
     assert result.exit_code == 0
     # THEN check that the proper information is displayed
-    assert "new file added" in caplog.text
+    assert NEW_FILE_ADDED in caplog.text
     # THEN check that the file has been included in the version and that the relative path is given
     assert Path(housekeeper_version_dir, second_sample_vcf.name).exists()
     assert Path(housekeeper_version_dir, second_sample_vcf.name).is_file()
     assert Path(version_obj.files[2].path) == Path(
         version_obj.relative_root_dir, second_sample_vcf.name
     )
 
@@ -140,15 +142,15 @@
         [str(second_sample_vcf), "-b", bundle_name, "-kip"],
         obj=populated_context,
     )
 
     # THEN assert the program exits with success
     assert result.exit_code == 0
     # THEN check that the proper information is displayed
-    assert "new file added" in caplog.text
+    assert NEW_FILE_ADDED in caplog.text
 
 
 def test_add_file_json(
     populated_context: Context,
     cli_runner: CliRunner,
     file_data_json: str,
     housekeeper_version_dir: Path,
@@ -160,8 +162,8 @@
 
     # WHEN trying to add a bundle
     result = cli_runner.invoke(file_cmd, ["--json", file_data_json], obj=populated_context)
 
     # THEN assert it fails
     assert result.exit_code == 0
     # THEN check that the proper information is displayed
-    assert "new file added" in caplog.text
+    assert NEW_FILE_ADDED in caplog.text
```

### Comparing `housekeeper-4.5.0/tests/cli/add/test_cli_add_tags.py` & `housekeeper-4.6.0/tests/cli/add/test_cli_add_tags.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/add/test_cli_add_version.py` & `housekeeper-4.6.0/tests/cli/add/test_cli_add_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/conftest.py` & `housekeeper-4.6.0/tests/cli/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Fixtures for CLI tests"""
 import datetime
+
 import pytest
 from click.testing import CliRunner
-from copy import deepcopy
-from pathlib import Path
 from housekeeper.store import Store
 from tests.helper_functions import Helpers
 
 
 @pytest.fixture(scope="function", name="store")
 def fixture_store(project_dir, db_uri):
     """Override the store fixture to get a controlled db path"""
@@ -16,64 +15,66 @@
     yield _store
     _store.drop_all()
 
 
 @pytest.fixture(scope="function", name="cli_runner")
 def fixture_cli_runner():
     """Return a cli runner for testing Click"""
-    runner = CliRunner()
-    return runner
+    return CliRunner()
 
 
 @pytest.fixture(scope="function", name="base_context")
-def fixture_base_context(db_uri, project_dir, store):
+def fixture_base_context(db_uri, project_dir, store) -> dict:
     """Return a context with initialized database"""
-    _ctx = {
+    return {
         "database": db_uri,
         "root": project_dir,
         "store": store,
     }
-    return _ctx
 
 
 @pytest.fixture(scope="function", name="populated_context")
-def fixture_populated_context(db_uri, project_dir, populated_store):
+def fixture_populated_context(db_uri, project_dir, populated_store) -> dict:
     """Return a context with initialized database with some data"""
-    _ctx = {
+    return {
         "database": db_uri,
         "root": project_dir,
         "store": populated_store,
     }
-    return _ctx
 
 
 @pytest.fixture(scope="function", name="populated_store_subsequent")
-def fixture_populated_store_subsequent(store: Store, bundle_data_subsequent: dict, helpers: Helpers) -> Store:
+def fixture_populated_store_subsequent(
+    store: Store, bundle_data_subsequent: dict, helpers: Helpers
+) -> Store:
     """Returns a populated store"""
     helpers.add_bundle(store, bundle_data_subsequent)
     return store
 
 
 @pytest.fixture(scope="function", name="populated_context_subsequent")
 def fixture_populated_context_subsequent(db_uri, project_dir, populated_store_subsequent):
     """Return a context with initialized database with some data"""
-    _ctx = {
+    return {
         "database": db_uri,
         "root": project_dir,
         "store": populated_store_subsequent,
     }
-    return _ctx
 
 
 @pytest.fixture(scope="function", name="bundle_data_subsequent")
 def fixture_bundle_data_subsequent(
-        case_id: str, family_data: dict, family2_data: dict, family3_data: dict, timestamp: datetime.datetime
+    case_id: str,
+    family_data: dict,
+    family2_data: dict,
+    family3_data: dict,
+    timestamp: datetime.datetime,
 ) -> dict:
     """Return a bundle."""
-    data = {
+    return {
         "name": case_id,
         "created_at": timestamp,
         "files": [
             {
                 "path": str(family_data["file"]),
                 "archive": False,
                 "tags": family_data["tags"],
@@ -83,11 +84,10 @@
                 "archive": False,
                 "tags": family2_data["tags"],
             },
             {
                 "path": str(family3_data["file"]),
                 "archive": True,
                 "tags": family3_data["tags"],
-            }
+            },
         ],
     }
-    return data
```

### Comparing `housekeeper-4.5.0/tests/cli/delete/test_cli_delete_bundle.py` & `housekeeper-4.6.0/tests/cli/delete/test_cli_delete_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/delete/test_cli_delete_file.py` & `housekeeper-4.6.0/tests/cli/delete/test_cli_delete_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/delete/test_cli_delete_files.py` & `housekeeper-4.6.0/tests/cli/delete/test_cli_delete_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/delete/test_cli_delete_version.py` & `housekeeper-4.6.0/tests/cli/delete/test_cli_delete_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/get/test_get_bundle.py` & `housekeeper-4.6.0/tests/cli/get/test_get_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/get/test_get_files.py` & `housekeeper-4.6.0/tests/cli/get/test_get_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/get/test_get_tag.py` & `housekeeper-4.6.0/tests/cli/get/test_get_tag.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/get/test_get_version.py` & `housekeeper-4.6.0/tests/cli/get/test_get_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/test_cli_core.py` & `housekeeper-4.6.0/tests/cli/test_cli_core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/cli/test_cli_include.py` & `housekeeper-4.6.0/tests/cli/test_cli_include.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Tests for include cli command"""
 import logging
 from datetime import datetime
 from pathlib import Path
 
-from click import Context
 from click.testing import CliRunner
-from housekeeper.cli.add import bundle_cmd
 from housekeeper.cli.include import include
 from housekeeper.constants import ROOT
 from housekeeper.store.api.core import Store
 from housekeeper.store.models import Bundle, Version
 
 
-def test_include_files_creates_bundle_dir(populated_context: Context, cli_runner: CliRunner):
+def test_include_files_creates_bundle_dir(populated_context: dict, cli_runner: CliRunner):
     """Test to include the files of a version for a bundle_name
 
     The bundle should not exist before and after command is run it should have been created
     """
     # GIVEN a context that is populated
     store: Store = populated_context["store"]
     bundle: Bundle = store._get_query(table=Bundle).first()
@@ -24,22 +22,22 @@
     # GIVEN that the latest version of the bundle is not included
     assert bundle.versions[0].included_at is None
     # GIVEN that no folder has been created since case is not included
     bundle_path = Path(populated_context[ROOT], bundle.name)
     assert not bundle_path.exists()
 
     # WHEN running the include files command
-    result = cli_runner.invoke(include, [bundle_name], obj=populated_context)
+    cli_runner.invoke(include, [bundle_name], obj=populated_context)
 
     # THEN assert that the bundle path was created
     assert bundle_path.exists()
 
 
 def test_include_files_creates_version_specific_bundle_dir(
-    populated_context: Context, cli_runner: CliRunner
+    populated_context: dict, cli_runner: CliRunner
 ):
     """Test to include the files of a version for a bundle_name
 
     The version bundle should not exist before and after command is run it should have been created
     """
     # GIVEN a context that is populated
     store: Store = populated_context["store"]
@@ -57,45 +55,39 @@
     # WHEN running the include files command
     cli_runner.invoke(include, [bundle_name], obj=populated_context)
 
     # THEN assert that the version path was created
     assert version_path.exists()
 
 
-def test_include_files_adds_version_specific_files(
-    populated_context: Context, cli_runner: CliRunner
-):
+def test_include_files_adds_version_specific_files(populated_context: dict, cli_runner: CliRunner):
     """Test to include the files of a version for a bundle_name
 
     The files should have been hard linked after command has been run
     """
     # GIVEN a context that is populated
     store: Store = populated_context["store"]
     bundle: Bundle = store._get_query(table=Bundle).first()
     version_obj = bundle.versions[0]
     bundle_name: str = bundle.name
     # GIVEN that the latest version of the bundle is not included
     assert version_obj.included_at is None
     # GIVEN that no version specific folder has been created since version is not included
-    version_path = populated_context[ROOT] / bundle.name / str(version_obj.created_at.date())
+    version_path = Path(populated_context[ROOT], bundle.name, str(version_obj.created_at.date()))
     assert not version_path.exists()
 
     # WHEN running the include files command
     cli_runner.invoke(include, [bundle_name], obj=populated_context)
 
-    # THEN assert that files are included in the folder
-    files_included = []
-    for file_path in version_path.iterdir():
-        files_included.append(file_path)
-
+    files_included = list(version_path.iterdir())
     assert files_included
     assert len(files_included) == len(version_obj.files)
 
 
-def test_include_files_specific_version(populated_context: Context, cli_runner: CliRunner):
+def test_include_files_specific_version(populated_context: dict, cli_runner: CliRunner):
     """Test to include the files of a version by specifying the version id
 
     The folder should have been created
     """
     # GIVEN a context that is populated
     store: Store = populated_context["store"]
     bundle: Bundle = store._get_query(table=Bundle).first()
@@ -111,24 +103,20 @@
 
     # WHEN running the include files command
     cli_runner.invoke(include, ["--version-id", version_id], obj=populated_context)
 
     # THEN assert that the folder was created
     assert version_path.exists()
 
-    # THEN assert that files are included in the folder
-    files_included = []
-    for file_path in version_path.iterdir():
-        files_included.append(file_path)
-
+    files_included = list(version_path.iterdir())
     assert files_included
     assert len(files_included) == len(version_obj.files)
 
 
-def test_include_version_no_args(populated_context: Context, cli_runner: CliRunner, caplog):
+def test_include_version_no_args(populated_context: dict, cli_runner: CliRunner, caplog):
     """Test to include the files of a version without specifying bundle name or version
 
     The command should exit since it needs to be specified
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context that is populated
 
@@ -137,15 +125,15 @@
 
     # THEN assert that the command exists with zero code 1
     assert result.exit_code == 1
     # THEN assert it was communicated that arguments are needed
     assert "use bundle name or version-id" in caplog.text
 
 
-def test_include_non_existing_version(populated_context: Context, cli_runner: CliRunner, caplog):
+def test_include_non_existing_version(populated_context: dict, cli_runner: CliRunner, caplog):
     """Test to include the files of a version that does not exist
 
     The command should exit since a valid version is needed
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context that is populated
     store: Store = populated_context["store"]
@@ -159,15 +147,15 @@
     # THEN assert that the command exists with zero code 1
     assert result.exit_code == 1
     # THEN assert it was communicated that version did not exist
     assert "version not found" in caplog.text
 
 
 def test_include_non_existing_bundle(
-    base_context: Context, cli_runner: CliRunner, timestamp: datetime, caplog
+    base_context: dict, cli_runner: CliRunner, timestamp: datetime, caplog
 ):
     """Test to include the files in the latest version of a bundle that does not exist
 
     The command should exit since a valid bundle is needed
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN context and a bundle_name that does not exist
@@ -181,15 +169,15 @@
     # THEN assert that the command exists with zero code 1
     assert result.exit_code == 1
     # THEN assert it was communicated that the bundle did not exist
     assert f"bundle {bundle_name} not found" in caplog.text
 
 
 def test_include_bundle_without_version(
-    base_context: Context, cli_runner: CliRunner, timestamp: datetime, caplog
+    base_context: dict, cli_runner: CliRunner, timestamp: datetime, caplog
 ):
     """Test to include the files in the latest version of a bundle that does not have versions
 
     The command should exit since a valid bundle with versions are needed
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN context with a bundle without versions
@@ -197,38 +185,36 @@
     bundle_name = "hello"
 
     new_bundle = store.new_bundle(name=bundle_name, created_at=timestamp)
     store.session.add(new_bundle)
     store.session.commit()
 
     bundle = store.get_bundle_by_name(bundle_name=bundle_name)
-    assert len(bundle.versions) == 0
+    assert not bundle.versions
 
     # WHEN running the include files specifying bundle without versions
     result = cli_runner.invoke(include, [bundle_name], obj=base_context)
 
     # THEN assert that the command exists with zero code 1
     assert result.exit_code == 1
     # THEN assert it was communicated that version did not exist
     assert f"Could not find any versions for bundle {bundle_name}" in caplog.text
 
 
-def test_include_version_already_included(
-    populated_context: Context, cli_runner: CliRunner, caplog
-):
+def test_include_version_already_included(populated_context: dict, cli_runner: CliRunner, caplog):
     """Test to include the files of a version that is already included
 
     The command should exit since the version can not be included again
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context that is populated and a version that is already included
     store: Store = populated_context["store"]
     version_obj = store._get_query(table=Version).first()
     version_id = version_obj.id
-    result = cli_runner.invoke(include, ["--version-id", version_id], obj=populated_context)
+    cli_runner.invoke(include, ["--version-id", version_id], obj=populated_context)
 
     # WHEN trying to include the version again
     result = cli_runner.invoke(include, ["--version-id", version_id], obj=populated_context)
 
     # THEN assert that the command exists with zero code 1
     assert result.exit_code == 1
     # THEN assert it was communicated that version did not exist
```

### Comparing `housekeeper-4.5.0/tests/conftest.py` & `housekeeper-4.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/helper_functions.py` & `housekeeper-4.6.0/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/store/conftest.py` & `housekeeper-4.6.0/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/store/filters/test_archive_filters.py` & `housekeeper-4.6.0/tests/store/filters/test_archive_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/store/filters/test_bundle_filters.py` & `housekeeper-4.6.0/tests/store/filters/test_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/store/filters/test_file_filters.py` & `housekeeper-4.6.0/tests/store/filters/test_file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/store/filters/test_tag_filters.py` & `housekeeper-4.6.0/tests/store/filters/test_tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/store/filters/test_version_bundle_filters.py` & `housekeeper-4.6.0/tests/store/filters/test_version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/store/filters/test_version_filters.py` & `housekeeper-4.6.0/tests/store/filters/test_version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/store/handlers/test_createhandler.py` & `housekeeper-4.6.0/tests/store/handlers/test_createhandler.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/store/handlers/test_updatehandler.py` & `housekeeper-4.6.0/tests/store/handlers/test_updatehandler.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/store/test_models.py` & `housekeeper-4.6.0/tests/store/test_models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/test_date.py` & `housekeeper-4.6.0/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.5.0/tests/test_include.py` & `housekeeper-4.6.0/tests/test_include.py`

 * *Files identical despite different names*

