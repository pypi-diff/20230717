# Comparing `tmp/tackle-0.5.0.tar.gz` & `tmp/tackle-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tackle-0.5.0.tar", last modified: Tue Jul 11 17:59:01 2023, max compression
+gzip compressed data, was "dist/tackle-0.5.1.tar", last modified: Mon Jul 17 13:44:34 2023, max compression
```

## Comparing `tackle-0.5.0.tar` & `tackle-0.5.1.tar`

### file list

```diff
@@ -1,965 +1,981 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-11 17:58:34.000000 tackle-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 17:58:34.000000 tackle-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-07-11 17:59:01.000000 tackle-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-07-11 17:58:34.000000 tackle-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-11 17:58:34.000000 tackle-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-11 17:59:01.000000 tackle-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4821 2023-07-11 17:58:34.000000 tackle-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    74797 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/collections/
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/collections/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/hooks/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/hooks/distinct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/hooks/list_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/hooks/map_to_list_key_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/hooks/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/notes.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/collections/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/concatenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/distinct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/list-keys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/sort-in-place.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/sort-map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/collections/tests/test_provider_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/command/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/command/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/hooks/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/hooks/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/command/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/exit-ignore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/exit-long.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/exit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/interactive.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/list-dir.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/multi-line-cmd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/command/tests/test_provider_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/console/
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/console/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/hooks/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/hooks/prints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/hooks/table.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/console/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/markdown.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/pprint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/print.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/table_split.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/test_provider_console_print.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/console/tests/test_provider_console_rich.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/context/
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/.tackle.meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/context/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/append.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/hooks/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/context/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/append-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/append-loop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/append.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/delete.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/get.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/keys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/pop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/set.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/test_provider_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/update-2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/update.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/context/tests/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/datetime/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/datetime/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/datetime/hooks/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/datetime/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/datetime/tests/date_now.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/datetime/tests/test_provider_datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/environment/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/environment/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/environment/hooks/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/environment/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/environment/tests/envs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/environment/tests/test_provider_envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/hooks/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/hooks/zips.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/tests/file/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/chmod.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/remove.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/shred.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/file/test_provider_system_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/tests/zips/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/tests/zips/stuff/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/files/tests/zips/stuff/stuff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/stuff/stuff/motings
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/stuff/things
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/stuff.zip
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/test_provider_system_zips.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/unzip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/zip-dir.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/files/tests/zips/zip-file.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/hooks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/hooks/file_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/hooks/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/hooks/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/hooks/update_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/file_update/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/file_update/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/file_update/file_update.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/file_update/test_hook_file_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/copy-without-render.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/examples.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/generate-types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/looped-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/looped.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/missing-file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/plain-src-block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/plain-src-path.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/plain-src.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-dir-file-base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-dir-file.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/contents/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/contents/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/dir/{{foo}}/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/dir/{{foo}}/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-error/file/{{foo}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-exception.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-file-additional-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render-file.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/.hidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/.hidden.{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/models/.hidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/models/.hidden.{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/models/stuff-{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/models/stuff.py.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/no-render/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/no-render/dir/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/no-render/dir/foo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/{{stuff}}/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/render_src/{{stuff}}/stuff-{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-if-file-exists.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-input/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-input/skip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-input/there.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-output/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-output/skip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-output/there.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/skip-overwrite-files.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/tackle-provider-remote.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/file.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/plain_src/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/plain_src/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/plain_src/models/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/plain_src/models/stuff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/stuff-{{stuff}}.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/.hidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/.hidden.{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/models/.hidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/models/.hidden.{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/models/stuff-{{things}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/models/stuff.py.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/{{stuff}}/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/templates/template_src/{{stuff}}/stuff-{{stuff}}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/test_provider_tackle_generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/types/type.tf
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/generate/unknown-variable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/existing-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/templates/things.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/jinja/test_provider_system_jinja.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/expected-output.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/file.md
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/multi-line.md
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/multi-line.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/generate/tests/update_section/test_provider_generate_update_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/git/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/git/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/hooks/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/hooks/gits.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/hooks/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/hooks/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/git/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/tests/meta-flat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/tests/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/tests/repo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/git/tests/test_provider_git_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/ini/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ini/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/ini/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ini/hooks/ini.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/ini/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ini/tests/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ini/tests/test_provider_ini.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/json/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/json/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/hooks/jsons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/json/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/tests/json.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/tests/read.json
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/tests/test_provider_json.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/json/tests/write.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/kubernetes/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/hooks/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/hooks/context.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/kubernetes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/tests/context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/tests/kubeconfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/tests/kubeconfig2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/kubernetes/tests/test_provider_k8s_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/hooks/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/hooks/match.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/hooks/while.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/tests/assertion/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/assertion/assert.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/assertion/test_provider_logic_assert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/tests/match/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/block-loop-match-block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/block-match-block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-block-if.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-block-loop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-block-merge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-dict-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/case-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/cases.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/default-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/default-underscore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/error-block-loop-merge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/error-malformed-regex.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/error-non-existant-key.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/error-wrong-hook-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/lists.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/loop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/match/test_provider_logic_match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/logic/tests/while/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/logic/tests/while/while.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/find_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/listdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/hooks/symlinks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/a-path/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/a-path/path1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/a-path/path1/path2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/a-path/path1/path2/thing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/a-path/thing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/base-dir-name.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/child.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/dirs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/dirs/args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/dirs/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/dirs/test_provider_system_hook_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/flatten/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/flatten/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/flatten/test_provider_paths_flatten_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/glob.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dir/.hidden-stuff
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dir/stuff.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dir/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/.hidden-dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/.hidden-dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/.hidden-stuff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir1/stuff.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir1/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir2/stuff.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/dir2/things.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/stuff.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/dirs/things.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/listdir/test_provider_system_listdir.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/parent.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/somedir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/somedir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/somedir/src.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/src.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/symlink/test_provider_system_symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/paths/tests/test_provider_system_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/postgres/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/postgres/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/postgres/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/postgres/hooks/query.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/postgres/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/confirm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/rawlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/hooks/select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/list_checked.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/list_index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/map_checked.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/map_index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/map_normal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/map_normal_checked.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/tackle-my-provider/
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/tackle-my-provider/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/tackle-my-provider/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/checkbox/test_prompt_provider_checkbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/confirm/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/confirm/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/confirm/test_provider_pyinquirer_confirm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/input/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/input/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/input/test_provider_prompt_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/password/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/password/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/password/test_provider_prompt_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/list_index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/map_index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/no-msg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/prompts/tests/select/test_prompt_provider_select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ssh/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/ssh/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ssh/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ssh/hooks/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ssh/hooks/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/ssh/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/hooks/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/hooks/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/hooks/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/hooks/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/tests/b64/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/b64/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/b64/test_provider_strings_b64.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/tests/random/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/random/random.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/random/test_provider_system_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/strings/tests/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/strings/join.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/strings/split.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/strings/tests/strings/test_provider_system_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/exit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/import.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/provider_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/run_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/tackle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/hooks/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block-logic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block-loop-block-nested.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block-loop-block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block-merge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/embedded-blocks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/embedded-lists.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/fake-tackle/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/fake-tackle/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/looped-context-other.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/looped-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/looped.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/merge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/test_provider_tackle_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/block/tmp-context.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/debug/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/debug/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/debug/test_provider_tackle_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/declarative-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/kubectl.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/ls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/method.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/test_provider_tackle_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/flatten/ubuntu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/expanded-list-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/expanded-string.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/function-import.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/local.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/context_provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/hooks/funks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/hooks/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test-provider/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/import/test_provider_tackle_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/provider_docs/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/provider_docs/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/provider_docs/test_tackle_provider_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/run_hook/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/run_hook/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/run_hook/test_provider_tackle_run_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/block-tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/fixture/example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/fixture/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/fixture/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/kwargs-default-hook-arg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/kwargs-default-hook-target.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/kwargs-default-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/kwargs-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/local-no-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/local-prior-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/tackle/test_provider_tackle_tackle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/tackle/tests/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/variable/test_provider_tackle_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/tackle/tests/variable/var.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/toml/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/toml/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/hooks/tomls.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/toml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/tests/read.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/tests/test_provider_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/tests/working.toml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/toml/tests/write.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/types/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/types/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/hooks/casting.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/hooks/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/types/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/tests/castings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/tests/test_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/types/tests/type.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/web/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/hooks/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/hooks/request.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/web/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/delete.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/get.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/post.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/put.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/web/tests/test_requests_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/.tackle.meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/yaml/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/hooks/yaml_in_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/hooks/yamls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/providers/yaml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/append.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/before.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/filter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/list_yaml.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/list_yaml_read.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/merge_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/merge_in_place.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/read.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/remove_list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/remove_str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/test_provider_system_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/update.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/update_in_place.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/write.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/yamldecode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/providers/yaml/tests/yamlencode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/special_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/help.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-11 17:58:34.000000 tackle-0.5.0/tackle/utils/zipfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36132 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 17:59:01.000000 tackle-0.5.0/tackle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/cli/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/.tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/cli/fixtures/dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/global-kwarg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/help-mixed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/input.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/fixtures/tackle-hello.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/test_cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/cli/test_cli_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/exceptions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/exceptions/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/bad-extension.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/calling-tackle-error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/calling-tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/missing-quote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-argument-extra.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-argument.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-named-argument.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-variable-call-tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-variable-call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/fixtures/unknown-variable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/exceptions/test_tackle_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/.hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/.hooks/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/cli-fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/cli-fixtures/a-dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/a-dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-call-func-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-call-func.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-embedded.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-no-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-hook-no-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-hook-type-unknown.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/cli-fixtures/cli-no-default-hook.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/composition-fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/composition-fixtures/enum-basic.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/extends-missing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/field-bad-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/field-require.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/hook-kwarg-missing-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/hook-kwarg-missing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/missing-field.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/no-exec-type-error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/return-str-not-found.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/str-value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/exceptions/try-in-default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/extends-fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/extends-fixtures/embedded-extends.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/extends-fixtures/extends-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/extends-fixtures/extends.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/.hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/.hooks/base-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/extends-visible.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/extends.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-args-method.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-exec-args-method.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-exec-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-exec-method.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-exec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks-method.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/field-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/field-hooks-fixtures/passed-context.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/.hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/.hooks/some-hooks.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/a-tackle/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/a-tackle/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/call-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/compact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/default-method-json.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/default-method-self.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/extends.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-dict-error-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-dict-error-str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-dict-error-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-list-error-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-list-error-str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-list-error-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-str-error-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-str-error-str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-type-exceptions/field-types-str-error-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/field-types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/flatten.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/a-dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/a-dir/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/hooks/funks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider/tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/a-dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/a-dir/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/hooks/funks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-hook/tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/a-dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/a-dir/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/hooks/funks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/func-provider-method/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/list-call.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/fixtures/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/methods/method-embed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/no-exec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/return-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/return-render.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/return.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/supplied-args-param-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/supplied-args-param-str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/supplied-kwargs-param-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/supplied-kwargs-param-str-loop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/fixtures/supplied-kwargs-param-str.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/method-fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-base-validate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-call-from-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-call-no-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-calll-default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-embed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-inherit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-maintain-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-nested-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-nested-override.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/method-fixtures/method-single.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_function_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_args_kwargs_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_field_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/test_functions_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/functions/types-fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/base-embed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/dict-base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/enum-basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/enum-types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/functions/types-fixtures/list-base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/macros/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/macros/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/macros/fixtures/func-inputs-basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/macros/test_macros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/main/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/.tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/block-input-overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/block-input.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/dict-input-overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/dict-input.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/func-exec-input.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/func-input.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/main/fixtures/home/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/home/example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/home/schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/main/fixtures/k8s/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/main/fixtures/k8s/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/k8s/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/fixtures/k8s/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/main/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/.hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/.hooks/thing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/child/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/child/dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/child/dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/child/dir/file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/context-provider-list.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/hooks/stuff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/{{cookiecutter.thing}}/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/cookiecutter-new-hook/{{cookiecutter.thing}}/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/global.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-install-dep.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider/context_provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider/hooks/thing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider-2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider-2/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider-2/hooks/stuff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider-reqs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/models/fixtures/test-provider-reqs/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider-reqs/hooks/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider-reqs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/test-provider-reqs/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/text2art.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/fixtures/unknown-hook-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/hook-dirs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/models/test_models_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/base-method-fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/list-comprehension.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-dict-loop-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-dict-loop-exception.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-list-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-list-loop-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-list-loop-value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-list-loop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/merge-list-value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/method-else.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/method-except.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/method-try.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/method-when.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/base-method-fixtures/try-validation-except.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/a-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/a-tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/calling_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/calling_dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/calling_dir/calling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/empty-hook-call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/empty-with-functions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/empty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/function-input-validation-error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/hook-input-validation-error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/merge-error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/exceptions-fixtures/out-of-range-arg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/.old/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/.old/merge-key-simple.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/ansible-playbook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/arg-types-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/arg-types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/block-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/block.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/ansible-parse-call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/ansible-parse-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/ansible-parse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/empty-block-exception.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/nested-dict-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/nested-dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/nested-for-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/nested-for.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/single-level-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/blocks/single-level.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/bug-mixed-flags-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/bug-mixed-flags.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/calling-context-inner.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/calling-context.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/dir/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/document-hooks-expected.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/document-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/dunder-key.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/duplicate-values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/embedded_list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/empty-elements.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/empty-hooks-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/empty-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/inner-tackle-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/inner-tackle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/input-key/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/input-key/child/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/input-key/child/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/input-key/child/calling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/input-key/tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/k8s-deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/list-list.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/macros/compact-hook-macro.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/macros/list-block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map-lists-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map-lists.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map-root-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map-root.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/match-case-logic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/merge-petstore-compact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/merge-petstore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/merge-simple-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/merge-simple.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/outer-tackle-arg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/outer-tackle-list-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/outer-tackle-list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/outer-tackle-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/outer-tackle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/petstore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/private-context-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/private-context.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/private-hooks-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/private-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/ruamel-parsing-error-braces.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/parser/fixtures/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/templates/file.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/toml.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/toml.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/var-hook-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/fixtures/var-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_args_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_base_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_hook_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_parser_parse_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/parser/test_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/render/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/render/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/call-function-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/call-function.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/debug.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/render/fixtures/dir/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/dir/stuff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/globals.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/hooks-args-too-many-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/hooks-args-wrong-type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/hooks-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/hooks-missing-args.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/is-defined.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/multi-line-block-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/multi-line-block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/multiple-hook-renders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/render-with-filters-output.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/render-with-filters.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/special-variables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/unknown-hook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/fixtures/unknown-variable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/test_render_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/render/test_special_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/test_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/files/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/bad.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/bad.stuff
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/bad.things
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/document.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/documents.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/fixtures/ok.toml
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/files/test_utils_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/bad-zip-file.zip
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/empty.zip
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/fake-repo-tmpl.zip
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/not-a-repo.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/protected-fake-repo-tmpl.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/fixtures/valid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/fixtures/valid/tackle-input/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/valid/tackle-input/tackle.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/fixtures/valid/yaml-input/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/fixtures/valid/yaml-input/cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_unzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_utils_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/test_utils_dicts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:59:01.000000 tackle-0.5.0/tests/utils/vcs/
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/vcs/test_vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-11 17:58:34.000000 tackle-0.5.0/tests/utils/vcs/test_vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-17 13:44:07.000000 tackle-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-17 13:44:07.000000 tackle-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-07-17 13:44:34.000000 tackle-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-07-17 13:44:07.000000 tackle-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-17 13:44:07.000000 tackle-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-17 13:44:34.000000 tackle-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4821 2023-07-17 13:44:07.000000 tackle-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74381 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/collections/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/hooks/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/hooks/distinct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/hooks/list_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/hooks/map_to_list_key_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/hooks/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/notes.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/collections/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/tests/concatenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/tests/distinct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/tests/list-keys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/tests/sort-in-place.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/tests/sort-map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/collections/tests/test_provider_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/command/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/command/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/command/hooks/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/command/hooks/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/command/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/command/tests/exit-ignore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/command/tests/exit-long.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/command/tests/exit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/command/tests/interactive.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/command/tests/list-dir.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/command/tests/multi-line-cmd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/command/tests/test_provider_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/console/
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/console/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/hooks/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/hooks/prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/hooks/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/console/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/tests/markdown.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/tests/pprint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/tests/print.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/tests/table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/tests/table_split.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/tests/test_provider_console_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/console/tests/test_provider_console_rich.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/.tackle.meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/context/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/hooks/append.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/hooks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/hooks/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/hooks/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/hooks/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/hooks/sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/hooks/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/hooks/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/context/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/append-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/append-loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/append.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/delete.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/get.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/keys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/pop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/set.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/test_provider_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/update-2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/update.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/context/tests/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/datetime/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/datetime/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/datetime/hooks/dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/datetime/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/datetime/tests/date_now.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/datetime/tests/test_provider_datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/environment/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/environment/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/environment/hooks/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/environment/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/environment/tests/envs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/environment/tests/test_provider_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/files/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/hooks/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/hooks/zips.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/files/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/files/tests/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/file/chmod.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/file/file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/file/remove.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/file/shred.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/file/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/file/test_provider_system_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/files/tests/zips/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/files/tests/zips/stuff/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/files/tests/zips/stuff/stuff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/zips/stuff/stuff/motings
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/zips/stuff/things
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/zips/stuff.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/zips/test_provider_system_zips.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/zips/unzip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/zips/zip-dir.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/files/tests/zips/zip-file.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/hooks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/hooks/file_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/hooks/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/hooks/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/hooks/update_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/file_update/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/file_update/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/file_update/file_update.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/file_update/test_hook_file_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/copy-without-render.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/examples.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/generate-types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/looped-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/looped.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/missing-file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/plain-src-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/plain-src-path.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/plain-src.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-dir-file-base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-dir-file.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-error/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-error/contents/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-error/contents/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-error/dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-error/dir/{{foo}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-error/dir/{{foo}}/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-error/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-error/file/{{foo}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-exception.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-file-additional-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render-file.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/.hidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/.hidden.{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/models/.hidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/models/.hidden.{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/models/stuff-{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/models/stuff.py.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/no-render/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/no-render/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/no-render/dir/foo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/{{stuff}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/render_src/{{stuff}}/stuff-{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/skip-if-file-exists.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/skip-input/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/skip-input/skip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/skip-input/there.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/skip-output/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/skip-output/skip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/skip-output/there.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/skip-overwrite-files.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/tackle-provider-remote.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/file.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/plain_src/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/plain_src/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/plain_src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/plain_src/models/stuff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/stuff-{{stuff}}.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/.hidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/.hidden.{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/models/.hidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/models/.hidden.{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/models/stuff-{{things}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/models/stuff.py.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/{{stuff}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/templates/template_src/{{stuff}}/stuff-{{stuff}}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/test_provider_tackle_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/types/type.tf
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/generate/unknown-variable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/jinja/existing-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/jinja/tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/jinja/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/jinja/templates/things.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/jinja/test_provider_system_jinja.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/generate/tests/update_section/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/update_section/basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/update_section/expected-output.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/update_section/file.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/update_section/multi-line.md
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/update_section/multi-line.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/generate/tests/update_section/test_provider_generate_update_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/git/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/hooks/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/hooks/gits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/hooks/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/hooks/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/git/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/tests/meta-flat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/tests/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/tests/repo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/git/tests/test_provider_git_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/ini/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/ini/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/ini/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/ini/hooks/ini.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/ini/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/ini/tests/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/ini/tests/test_provider_ini.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/json/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/json/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/json/hooks/jsons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/json/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/json/tests/json.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/json/tests/read.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/json/tests/test_provider_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/json/tests/write.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/kubernetes/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/kubernetes/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/kubernetes/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/kubernetes/hooks/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/kubernetes/hooks/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/kubernetes/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/kubernetes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/kubernetes/tests/context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/kubernetes/tests/kubeconfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/kubernetes/tests/kubeconfig2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/kubernetes/tests/test_provider_k8s_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/logic/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/hooks/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/hooks/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/hooks/while.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/logic/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/logic/tests/assertion/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/assertion/assert.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/assertion/test_provider_logic_assert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/logic/tests/match/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/block-loop-match-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/block-match-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/case-block-if.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/case-block-loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/case-block-merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/case-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/case-dict-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/case-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/cases.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/default-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/default-underscore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/error-block-loop-merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/error-malformed-regex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/error-non-existant-key.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/error-wrong-hook-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/lists.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/match/test_provider_logic_match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/logic/tests/while/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/logic/tests/while/while.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/hooks/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/hooks/find_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/hooks/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/hooks/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/hooks/listdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/hooks/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/hooks/symlinks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/a-path/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/a-path/path1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/a-path/path1/path2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/a-path/path1/path2/thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/a-path/thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/base-dir-name.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/child.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/dirs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/dirs/args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/dirs/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/dirs/test_provider_system_hook_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/flatten/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/flatten/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/flatten/test_provider_paths_flatten_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/glob.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dir/.hidden-stuff
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dir/stuff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dir/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/.hidden-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/.hidden-dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/.hidden-stuff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/dir1/stuff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/dir1/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/dir2/stuff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/dir2/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/stuff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/dirs/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/listdir/test_provider_system_listdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/parent.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/symlink/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/paths/tests/symlink/somedir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/symlink/somedir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/symlink/somedir/src.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/symlink/src.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/symlink/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/symlink/test_provider_system_symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/paths/tests/test_provider_system_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/postgres/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/postgres/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/postgres/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/postgres/hooks/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/postgres/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/prompts/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/hooks/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/hooks/confirm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/hooks/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/hooks/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/hooks/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/hooks/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/hooks/rawlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/hooks/select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/prompts/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/list_checked.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/list_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/map_checked.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/map_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/map_normal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/map_normal_checked.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/tackle-my-provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/tackle-my-provider/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/tackle-my-provider/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/checkbox/test_prompt_provider_checkbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/prompts/tests/confirm/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/confirm/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/confirm/test_provider_pyinquirer_confirm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/prompts/tests/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/input/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/input/test_provider_prompt_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/prompts/tests/password/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/password/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/password/test_provider_prompt_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/prompts/tests/select/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/select/list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/select/list_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/select/map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/select/map_index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/select/no-msg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/select/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/prompts/tests/select/test_prompt_provider_select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/ssh/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/ssh/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/ssh/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/ssh/hooks/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/ssh/hooks/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/ssh/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/strings/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/hooks/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/hooks/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/hooks/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/hooks/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/strings/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/strings/tests/b64/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/tests/b64/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/tests/b64/test_provider_strings_b64.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/strings/tests/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/tests/random/random.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/tests/random/test_provider_system_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/strings/tests/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/tests/strings/join.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/tests/strings/split.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/strings/tests/strings/test_provider_system_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/hooks/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/hooks/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/hooks/exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/hooks/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/hooks/import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/hooks/literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/hooks/provider_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/hooks/run_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/hooks/tackle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/hooks/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle/providers/tackle/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/block-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/block-logic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/block-loop-block-nested.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/block-loop-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/block-merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/embedded-blocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/embedded-lists.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/fake-tackle/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/fake-tackle/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/looped-context-other.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/looped-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/looped.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/test_provider_tackle_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/block/tmp-context.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/debug/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/debug/test_provider_tackle_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/flatten/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/flatten/declarative-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/flatten/kubectl.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/flatten/ls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/flatten/method.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/flatten/test_provider_tackle_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/flatten/ubuntu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/expanded-list-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/expanded-string.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/function-import.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/local.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/test-provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/test-provider/context_provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/test-provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/test-provider/hooks/funks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/test-provider/hooks/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/test-provider/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/import/test_provider_tackle_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/provider_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/provider_docs/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/provider_docs/test_tackle_provider_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/run_hook/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/run_hook/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/run_hook/test_provider_tackle_run_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/block-tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/fixture/example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/fixture/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/fixture/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/kwargs-default-hook-arg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/kwargs-default-hook-target.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/kwargs-default-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/kwargs-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/local-no-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/local-prior-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/tackle/test_provider_tackle_tackle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/tackle/tests/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/variable/test_provider_tackle_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/tackle/tests/variable/var.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/toml/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/toml/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/toml/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/toml/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/toml/hooks/tomls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/toml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/toml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/toml/tests/read.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/toml/tests/test_provider_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/toml/tests/working.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/toml/tests/write.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/types/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/types/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/types/hooks/casting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/types/hooks/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/types/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/types/tests/castings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/types/tests/test_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/types/tests/type.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/web/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/hooks/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/hooks/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/web/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/tests/delete.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/tests/get.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/tests/patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/tests/post.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/tests/put.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/web/tests/test_requests_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/.tackle.meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/yaml/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/hooks/yaml_in_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/hooks/yamls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/providers/yaml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/append.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/before.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/filter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/list_yaml.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/list_yaml_read.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/merge_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/merge_in_place.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/read.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/remove_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/remove_str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/test_provider_system_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/update.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/update_in_place.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/write.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/yamldecode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/providers/yaml/tests/yamlencode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/special_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tackle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-17 13:44:07.000000 tackle-0.5.1/tackle/utils/zipfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36753 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 13:44:33.000000 tackle-0.5.1/tackle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/cli/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/cli/fixtures/.tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/cli/fixtures/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/cli/fixtures/dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/cli/fixtures/global-kwarg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/cli/fixtures/help-mixed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/cli/fixtures/input.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/cli/fixtures/tackle-hello.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/cli/test_cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/cli/test_cli_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/exceptions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/exceptions/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/bad-extension.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/calling-tackle-error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/calling-tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/missing-quote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/unknown-argument-extra.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/unknown-argument.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/unknown-named-argument.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/unknown-variable-call-tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/unknown-variable-call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/fixtures/unknown-variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/exceptions/test_tackle_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/.hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/.hooks/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/cli-fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/cli-fixtures/a-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/cli-fixtures/a-dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/cli-fixtures/cli-call-func-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/cli-fixtures/cli-call-func.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/cli-fixtures/cli-default-hook-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/cli-fixtures/cli-default-hook-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/cli-fixtures/cli-default-hook-embedded.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/cli-fixtures/cli-default-hook-no-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/cli-fixtures/cli-hook-no-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/cli-fixtures/cli-hook-type-unknown.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/cli-fixtures/cli-no-default-hook.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/composition-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/composition-fixtures/enum-basic.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/exceptions/extends-missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/exceptions/field-bad-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/exceptions/field-require.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/exceptions/hook-kwarg-missing-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/exceptions/hook-kwarg-missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/exceptions/missing-field.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/exceptions/no-exec-type-error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/exceptions/return-str-not-found.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/exceptions/str-value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/exceptions/try-in-default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/extends-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/extends-fixtures/embedded-extends.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/extends-fixtures/extends-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/extends-fixtures/extends.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/.hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/.hooks/base-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/extends-visible.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/extends.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/field-hooks-args-method.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/field-hooks-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/field-hooks-exec-args-method.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/field-hooks-exec-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/field-hooks-exec-method.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/field-hooks-exec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/field-hooks-method.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/field-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/field-hooks-fixtures/passed-context.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/.hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/.hooks/some-hooks.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/a-tackle/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/a-tackle/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/call-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/compact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/default-method-json.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/default-method-self.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/extends.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/field-type-exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/field-type-exceptions/field-types-dict-error-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/field-type-exceptions/field-types-dict-error-str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/field-type-exceptions/field-types-dict-error-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/field-type-exceptions/field-types-list-error-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/field-type-exceptions/field-types-list-error-str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/field-type-exceptions/field-types-list-error-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/field-type-exceptions/field-types-str-error-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/field-type-exceptions/field-types-str-error-str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/field-type-exceptions/field-types-str-error-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/field-types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/flatten.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/func-provider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/func-provider/a-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/func-provider/a-dir/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/func-provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/func-provider/hooks/funks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/func-provider/tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-hook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-hook/a-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-hook/a-dir/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-hook/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-hook/hooks/funks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-hook/tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-method/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-method/a-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-method/a-dir/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-method/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-method/hooks/funks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/func-provider-method/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/list-call.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/fixtures/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/methods/method-embed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/no-exec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/return-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/return-render.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/return.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/supplied-args-param-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/supplied-args-param-str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/supplied-kwargs-param-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/supplied-kwargs-param-str-loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/fixtures/supplied-kwargs-param-str.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/method-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-base-validate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-call-from-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-call-no-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-calll-default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-embed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-inherit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-maintain-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-nested-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-nested-override.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/method-fixtures/method-single.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/test_function_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/test_functions_args_kwargs_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/test_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/test_functions_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/test_functions_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/test_functions_field_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/test_functions_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/test_functions_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/functions/types-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/types-fixtures/base-embed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/types-fixtures/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/types-fixtures/dict-base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/types-fixtures/enum-basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/types-fixtures/enum-types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/functions/types-fixtures/list-base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/macros/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/macros/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/macros/fixtures/func-inputs-basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/macros/test_macros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/main/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/.tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/block-input-overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/block-input.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/dict-input-overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/dict-input.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/func-exec-input.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/func-input.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/main/fixtures/home/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/home/example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/home/schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/main/fixtures/k8s/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/main/fixtures/k8s/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/k8s/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/fixtures/k8s/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/main/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/.hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/.hooks/thing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tests/models/fixtures/child/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/child/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/child/dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/child/dir/file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/context-provider-list.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/cookiecutter-new-hook/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/cookiecutter-new-hook/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/cookiecutter-new-hook/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/cookiecutter-new-hook/hooks/stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/cookiecutter-new-hook/{{cookiecutter.thing}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/cookiecutter-new-hook/{{cookiecutter.thing}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/global.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/test-install-dep.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/test-provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/test-provider/context_provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/test-provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/test-provider/hooks/thing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tests/models/fixtures/test-provider-2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/test-provider-2/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/test-provider-2/hooks/stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/test-provider-reqs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/models/fixtures/test-provider-reqs/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/test-provider-reqs/hooks/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/test-provider-reqs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/test-provider-reqs/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/text2art.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/fixtures/unknown-hook-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/hook-dirs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/models/test_models_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tests/parser/.functions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tests/parser/.functions/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/.functions/fixtures/func-provider-hook/
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/.functions/fixtures/func-provider-hook/funcs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/.functions/fixtures/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/.functions/fixtures/functions/hook-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/.functions/fixtures/functions/merge-field.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/func-provider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/func-provider/a-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/func-provider/a-dir/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/func-provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/func-provider/hooks/funks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/func-provider/tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/only-hooks-dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/only-hooks-dir/a-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/only-hooks-dir/a-dir/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/only-hooks-dir/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/.functions/provider-fixtures/only-hooks-dir/hooks/funks.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/base-method-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/list-comprehension.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/merge-dict-loop-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/merge-dict-loop-exception.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/merge-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/merge-list-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/merge-list-loop-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/merge-list-loop-value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/merge-list-loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/merge-list-value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/method-else.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/method-except.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/method-try.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/method-when.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/base-method-fixtures/try-validation-except.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/a-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/a-tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/calling_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/calling_dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/calling_dir/calling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/empty-hook-call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/empty-with-functions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/function-input-validation-error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/hook-input-validation-error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/merge-error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/exceptions-fixtures/out-of-range-arg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/fixtures/.old/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/.old/merge-key-simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/copied-hook-args.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/fixtures/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/dir/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/document-hooks-expected.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/document-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/duplicate-values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/inner-tackle-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/inner-tackle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/fixtures/input-key/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/fixtures/input-key/child/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/input-key/child/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/input-key/child/calling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/input-key/tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/merge-petstore-compact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/merge-petstore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/outer-tackle-arg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/outer-tackle-list-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/outer-tackle-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/outer-tackle-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/outer-tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/petstore.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/fixtures/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/templates/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/fixtures/types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/macro-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/ansible-parse-call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/ansible-parse-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/ansible-parse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/calling-context-inner.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/calling-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/compact-hook-macro.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/empty-block-exception.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/inner-tackle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/list-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/nested-dict-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/nested-dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/nested-for-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/nested-for.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/ruamel-parsing-error-braces.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/single-level-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/macro-fixtures/single-level.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/parser/parse-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/ansible-playbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/arg-types-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/arg-types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/block-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/bug-mixed-flags-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/bug-mixed-flags.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/empty-elements.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/empty-hooks-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/empty-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/k8s-deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/list-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/map-lists-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/map-lists.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/map-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/map-root-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/map-root.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/merge-simple-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/merge-simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/private-context-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/private-context.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/private-hooks-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/private-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/toml.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/toml.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/var-hook-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/parse-fixtures/var-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/test_parser_args_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/test_parser_base_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/test_parser_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/test_parser_hook_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/test_parser_macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/parser/test_parser_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/render/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/render/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/call-function-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/call-function.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/debug.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/render/fixtures/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/dir/stuff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/globals.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/hooks-args-too-many-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/hooks-args-wrong-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/hooks-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/hooks-missing-args.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/is-defined.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/multi-line-block-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/multi-line-block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/multiple-hook-renders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/render-with-filters-output.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/render-with-filters.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/special-variables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/unknown-hook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/fixtures/unknown-variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/test_render_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/render/test_special_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/test_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/utils/files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/utils/files/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/files/fixtures/bad.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/files/fixtures/bad.stuff
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/files/fixtures/bad.things
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/files/fixtures/document.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/files/fixtures/documents.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/files/fixtures/file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/files/fixtures/ok.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/files/test_utils_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/utils/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/fixtures/bad-zip-file.zip
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/fixtures/empty.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/fixtures/fake-repo-tmpl.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/fixtures/not-a-repo.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/fixtures/protected-fake-repo-tmpl.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:33.000000 tackle-0.5.1/tests/utils/fixtures/valid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/utils/fixtures/valid/tackle-input/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/fixtures/valid/tackle-input/tackle.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/utils/fixtures/valid/yaml-input/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/fixtures/valid/yaml-input/cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/test_unzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/test_utils_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/test_utils_dicts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:34.000000 tackle-0.5.1/tests/utils/vcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/vcs/test_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-17 13:44:07.000000 tackle-0.5.1/tests/utils/vcs/test_vcs_provider.py
```

### Comparing `tackle-0.5.0/LICENSE` & `tackle-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/PKG-INFO` & `tackle-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tackle
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tackle is a declarative DSL for building modular workflows and code generators. Tool is plugins based and can easily be extended by writing additional hooks or importing external providers that can be turned into a self documenting CLI, all out of yaml, json, toml.
 Home-page: https://github.com/robcxyz/tackle
 Author: Rob Cannon
 Author-email: robc.io.opensource@gmail.com
 License: BSD
 Description: <img align="right" width="280" height="280" src="https://raw.githubusercontent.com/sudoblockio/tackle/main/docs/assets/logo-box.png">
```

### Comparing `tackle-0.5.0/README.md` & `tackle-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/setup.py` & `tackle-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/cli.py` & `tackle-0.5.1/tackle/cli.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/exceptions.py` & `tackle-0.5.1/tackle/exceptions.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/hooks.py` & `tackle-0.5.1/tackle/hooks.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/macros.py` & `tackle-0.5.1/tackle/macros.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
     return {arrow: element}
 
 
 def list_to_var_macro(context: 'Context', element: list) -> dict:
     """
     Convert arrow keys with a list as the value to `var` hooks via a re-write to the
-    input.
+     input.
     """
     # TODO: Convert this to a block. Issue is that keys are not rendered by default so
     #  when str items in a list are parsed, they are not rendered by default. Should
     #  have some validator or something on block to render str items in a list.
     base_key_path = context.key_path[:-1]
     new_key = [context.key_path[-1][:-2]]
     old_key_path = context.key_path[len(context.key_path_block) :]
```

### Comparing `tackle-0.5.0/tackle/main.py` & `tackle-0.5.1/tackle/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     """
     if args:
         # Remove first arg and consider all other args global to be ingested later
         kwargs['input_string'] = args[0]
         if len(args) != 1:
             kwargs['global_args'] = []
             for i in range(1, len(args)):
+                # Append all but the first arg which is parsed separately
                 kwargs['global_args'].append(args[i])
 
     # Handle empty calls which fallback to finding the closest tackle file
     # in the parent directory
     if 'input_string' not in kwargs or kwargs['input_string'] is None:
         kwargs['input_string'] = find_nearest_tackle_file()
```

### Comparing `tackle-0.5.0/tackle/models.py` & `tackle-0.5.1/tackle/models.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/parser.py` & `tackle-0.5.1/tackle/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,34 +186,14 @@
             pass
         else:
             raise exceptions.UnknownInputArgumentException(
                 f"Unknown arg supplied `{arg}`",
                 context=context,
             )
 
-    # Handle kwargs
-    for k, v in kwargs.items():
-        if k == 'args':
-            # TODO: I thought this would work
-            # args.append(v)
-            # But just passing works. Reason is the above duplicates the arg. No idea...
-            pass
-        elif k == 'kwargs':
-            pass
-        elif k in hook.__fields__:
-            # TODO: consolidate with `update_hook_with_kwargs_and_flags` - same same
-            if hook.__fields__[k].type_ == bool:
-                # Handle flags where default is true
-                if hook.__fields__[k].default:
-                    hook.__fields__[k].default = False
-                else:
-                    hook.__fields__[k].default = True
-            else:
-                hook.__fields__[k].default = v
-
     return hook
 
 
 def merge_block_output(
     hook_output_value: Any,
     context: Context,
     append_hook_value: bool = False,
@@ -530,14 +510,15 @@
 def parse_hook_execute(
     context: 'Context',
     hook_dict: dict,
     Hook: ModelMetaclass,
     append_hook_value: bool = None,
 ):
     """Parse the remaining arguments such as try/except and merge"""
+    # Parse `kwargs` field which is a dict that will map to hook fields
     if 'kwargs' in hook_dict:
         update_hook_with_kwargs_field(context=context, hook_dict=hook_dict)
 
     # Render the remaining hook variables
     render_hook_vars(context=context, hook_dict=hook_dict, Hook=Hook)
 
     # Instantiate the hook
@@ -588,14 +569,20 @@
             value=hook_output_value,
         )
 
 
 def evaluate_for(context: 'Context', hook_dict: dict, Hook: ModelMetaclass):
     """Run the parse_hook function in a loop with temporary variables."""
     loop_targets = render_variable(context, wrap_jinja_braces(hook_dict['for']))
+    if not isinstance(loop_targets, list):
+        raise exceptions.MalformedTemplateVariableException(
+            f"The `for` field must be a list or string reference to a list. The value "
+            f"is of type `{type(loop_targets).__name__}`.", context=context,
+        )
+
     if len(loop_targets) == 0:
         return
     hook_dict.pop('for')
 
     # Need add an empty list in the value so we have something to append to except when
     # we are merging.
     if 'merge' not in hook_dict:
@@ -827,51 +814,51 @@
         else:
             hook_dict.pop('_>')
     else:
         # Hook is a compact expression - Can only be a string
         hook_dict = {}
 
     # Look up the hook from the imported providers
-    hook = get_hook(
+    Hook = get_hook(
         context=context,
         hook_type=first_arg,
         args=args,
         kwargs=kwargs,
     )
-    if hook is None:
+    if Hook is None:
         exceptions.raise_unknown_hook(context, first_arg)
 
-    hook_dict['hook_type'] = hook.__fields__['hook_type'].default
+    hook_dict['hook_type'] = Hook.__fields__['hook_type'].default
 
     # `args` can be a kwarg (ie `tackle --args foo`) and is manually added to args var
     if 'args' in kwargs:
         # For calling hooks, you can manually provide the hook with args. Useful for
         # creating declarative hooks that
         hook_args = kwargs.pop('args')
         if isinstance(hook_args, list):
             args += hook_args
         else:
             args += [hook_args]
 
     # Associate hook arguments provided in the call with hook attributes
-    evaluate_args(args=args, hook_dict=hook_dict, Hook=hook, context=context)
+    evaluate_args(args=args, hook_dict=hook_dict, Hook=Hook, context=context)
     # Add any kwargs
     for k, v in kwargs.items():
         hook_dict[k] = v
     for i in flags:
         hook_dict[i] = True
     # Cleanup any unquoted fields -> common mistake that is hard to debug producing a
     #  nested dict that breaks parsing / hook calls. Ex foo: {{bar}} -> foo: "{{bar}}"
     cleanup_unquoted_strings(hook_dict)
 
     # Main parser
     parse_hook(
         context=context,
         hook_dict=hook_dict,
-        hook=hook,
+        hook=Hook,
     )
 
 
 def walk_element(context: 'Context', element):
     """
     Traverse an object looking for hook calls and running those hooks. Here we are
      keeping track of which keys are traversed in a list called `key_path` with strings
```

### Comparing `tackle-0.5.0/tackle/providers/collections/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/collections/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/collections/hooks/distinct.py` & `tackle-0.5.1/tackle/providers/collections/hooks/distinct.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/collections/hooks/list_key.py` & `tackle-0.5.1/tackle/providers/collections/hooks/list_key.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/collections/hooks/map_to_list_key_values.py` & `tackle-0.5.1/tackle/providers/collections/hooks/map_to_list_key_values.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/collections/hooks/sort.py` & `tackle-0.5.1/tackle/providers/collections/hooks/sort.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/collections/tests/sort-in-place.yaml` & `tackle-0.5.1/tackle/providers/collections/tests/sort-in-place.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/collections/tests/test_provider_collections.py` & `tackle-0.5.1/tackle/providers/collections/tests/test_provider_collections.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,7 +23,16 @@
     assert output['out'] == ['foo', 'bar', 'stuff', 'things']
 
 
 def test_collections_hook_distinct(change_dir):
     output = tackle('distinct.yaml')
     for i in output['distincts']:
         assert i in ['stuff', 'foo', 'things']
+
+
+def test_collections_hook_range(change_dir):
+    o = tackle('range.yaml')
+    assert o['forward_1'] == [0, 1, 2]
+    assert o['forward_2'] == [1, 2]
+    assert o['backward_2'] == [3, 2]
+    assert o['forward_3'] == [0, 2, 4]
+    assert o['backward_3'] == [6, 4]
```

### Comparing `tackle-0.5.0/tackle/providers/command/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/command/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/command/hooks/command.py` & `tackle-0.5.1/tackle/providers/command/hooks/command.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/command/tests/test_provider_command.py` & `tackle-0.5.1/tackle/providers/command/tests/test_provider_command.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/console/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/console/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/console/hooks/markdown.py` & `tackle-0.5.1/tackle/providers/console/hooks/markdown.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/console/hooks/prints.py` & `tackle-0.5.1/tackle/providers/console/hooks/prints.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/console/hooks/table.py` & `tackle-0.5.1/tackle/providers/console/hooks/table.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/context/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/hooks/append.py` & `tackle-0.5.1/tackle/providers/context/hooks/append.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/hooks/delete.py` & `tackle-0.5.1/tackle/providers/context/hooks/delete.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/hooks/get.py` & `tackle-0.5.1/tackle/providers/context/hooks/get.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/hooks/keys.py` & `tackle-0.5.1/tackle/providers/context/hooks/keys.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/hooks/pop.py` & `tackle-0.5.1/tackle/providers/context/hooks/pop.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/hooks/sets.py` & `tackle-0.5.1/tackle/providers/context/hooks/sets.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/hooks/update.py` & `tackle-0.5.1/tackle/providers/context/hooks/update.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/hooks/values.py` & `tackle-0.5.1/tackle/providers/context/hooks/values.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/tests/append-loop.yaml` & `tackle-0.5.1/tackle/providers/context/tests/append-loop.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/tests/test_provider_context.py` & `tackle-0.5.1/tackle/providers/context/tests/test_provider_context.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/tests/update-2.yaml` & `tackle-0.5.1/tackle/providers/context/tests/update-2.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/context/tests/update.yaml` & `tackle-0.5.1/tackle/providers/context/tests/update.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/datetime/hooks/dates.py` & `tackle-0.5.1/tackle/providers/datetime/hooks/dates.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/environment/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/environment/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/environment/hooks/envs.py` & `tackle-0.5.1/tackle/providers/environment/hooks/envs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/environment/tests/test_provider_envs.py` & `tackle-0.5.1/tackle/providers/environment/tests/test_provider_envs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/files/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/files/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/files/hooks/file.py` & `tackle-0.5.1/tackle/providers/files/hooks/file.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/files/hooks/zips.py` & `tackle-0.5.1/tackle/providers/files/hooks/zips.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/files/tests/file/test_provider_system_file.py` & `tackle-0.5.1/tackle/providers/files/tests/file/test_provider_system_file.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/files/tests/zips/test_provider_system_zips.py` & `tackle-0.5.1/tackle/providers/files/tests/zips/test_provider_system_zips.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/generate/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/generate/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/generate/hooks/file_update.py` & `tackle-0.5.1/tackle/providers/generate/hooks/file_update.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/generate/hooks/generate.py` & `tackle-0.5.1/tackle/providers/generate/hooks/generate.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/generate/hooks/jinja.py` & `tackle-0.5.1/tackle/providers/generate/hooks/jinja.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/generate/hooks/update_section.py` & `tackle-0.5.1/tackle/providers/generate/hooks/update_section.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/generate/tests/generate/test_provider_tackle_generate.py` & `tackle-0.5.1/tackle/providers/generate/tests/generate/test_provider_tackle_generate.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/generate/tests/jinja/test_provider_system_jinja.py` & `tackle-0.5.1/tackle/providers/generate/tests/jinja/test_provider_system_jinja.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/generate/tests/update_section/test_provider_generate_update_section.py` & `tackle-0.5.1/tackle/providers/generate/tests/update_section/test_provider_generate_update_section.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/git/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/git/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/git/hooks/github.py` & `tackle-0.5.1/tackle/providers/git/hooks/github.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/git/hooks/gits.py` & `tackle-0.5.1/tackle/providers/git/hooks/gits.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/git/hooks/meta.py` & `tackle-0.5.1/tackle/providers/git/hooks/meta.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/git/tests/test_provider_git_hooks.py` & `tackle-0.5.1/tackle/providers/git/tests/test_provider_git_hooks.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/ini/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/ini/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/ini/hooks/ini.py` & `tackle-0.5.1/tackle/providers/ini/hooks/ini.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/ini/tests/test_provider_ini.py` & `tackle-0.5.1/tackle/providers/ini/tests/test_provider_ini.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/json/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/json/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/json/hooks/jsons.py` & `tackle-0.5.1/tackle/providers/json/hooks/jsons.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/kubernetes/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/kubernetes/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/kubernetes/hooks/context.py` & `tackle-0.5.1/tackle/providers/kubernetes/hooks/context.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/kubernetes/tests/kubeconfig.yaml` & `tackle-0.5.1/tackle/providers/kubernetes/tests/kubeconfig.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/kubernetes/tests/kubeconfig2.yaml` & `tackle-0.5.1/tackle/providers/kubernetes/tests/kubeconfig2.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/logic/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/logic/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/logic/hooks/assertion.py` & `tackle-0.5.1/tackle/providers/logic/hooks/assertion.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/logic/hooks/match.py` & `tackle-0.5.1/tackle/providers/logic/hooks/match.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/logic/hooks/while.py` & `tackle-0.5.1/tackle/providers/logic/hooks/while.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/logic/tests/match/block-match-block.yaml` & `tackle-0.5.1/tackle/providers/logic/tests/match/block-match-block.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/logic/tests/match/case-block-if.yaml` & `tackle-0.5.1/tackle/providers/logic/tests/match/case-block-if.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/logic/tests/match/case-block-loop.yaml` & `tackle-0.5.1/tackle/providers/logic/tests/match/case-block-loop.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/logic/tests/match/loop.yaml` & `tackle-0.5.1/tackle/providers/logic/tests/match/loop.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/logic/tests/match/test_provider_logic_match.py` & `tackle-0.5.1/tackle/providers/logic/tests/match/test_provider_logic_match.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/paths/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/hooks/dirs.py` & `tackle-0.5.1/tackle/providers/paths/hooks/dirs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/hooks/find_in.py` & `tackle-0.5.1/tackle/providers/paths/hooks/find_in.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/hooks/flatten.py` & `tackle-0.5.1/tackle/providers/paths/hooks/flatten.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/hooks/globs.py` & `tackle-0.5.1/tackle/providers/paths/hooks/globs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/hooks/listdir.py` & `tackle-0.5.1/tackle/providers/paths/hooks/listdir.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/hooks/paths.py` & `tackle-0.5.1/tackle/providers/paths/hooks/paths.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/hooks/symlinks.py` & `tackle-0.5.1/tackle/providers/paths/hooks/symlinks.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/tests/dirs/test_provider_system_hook_dir.py` & `tackle-0.5.1/tackle/providers/paths/tests/dirs/test_provider_system_hook_dir.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/tests/flatten/tackle.yaml` & `tackle-0.5.1/tackle/providers/paths/tests/flatten/tackle.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/tests/listdir/tackle.yaml` & `tackle-0.5.1/tackle/providers/paths/tests/listdir/tackle.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/tests/listdir/test_provider_system_listdir.py` & `tackle-0.5.1/tackle/providers/paths/tests/listdir/test_provider_system_listdir.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/paths/tests/test_provider_system_path.py` & `tackle-0.5.1/tackle/providers/paths/tests/test_provider_system_path.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/postgres/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/postgres/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/postgres/hooks/query.py` & `tackle-0.5.1/tackle/providers/postgres/hooks/query.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/prompts/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/hooks/checkbox.py` & `tackle-0.5.1/tackle/providers/prompts/hooks/checkbox.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/hooks/confirm.py` & `tackle-0.5.1/tackle/providers/prompts/hooks/confirm.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/hooks/editor.py` & `tackle-0.5.1/tackle/providers/prompts/hooks/editor.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/hooks/expand.py` & `tackle-0.5.1/tackle/providers/prompts/hooks/expand.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/hooks/input.py` & `tackle-0.5.1/tackle/providers/prompts/hooks/input.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/hooks/password.py` & `tackle-0.5.1/tackle/providers/prompts/hooks/password.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/hooks/rawlist.py` & `tackle-0.5.1/tackle/providers/prompts/hooks/rawlist.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/hooks/select.py` & `tackle-0.5.1/tackle/providers/prompts/hooks/select.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/tests/checkbox/tackle-my-provider/LICENSE` & `tackle-0.5.1/tackle/providers/prompts/tests/checkbox/tackle-my-provider/LICENSE`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/tests/checkbox/test_prompt_provider_checkbox.py` & `tackle-0.5.1/tackle/providers/prompts/tests/checkbox/test_prompt_provider_checkbox.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/prompts/tests/select/test_prompt_provider_select.py` & `tackle-0.5.1/tackle/providers/prompts/tests/select/test_prompt_provider_select.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/ssh/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/ssh/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/ssh/hooks/interactive.py` & `tackle-0.5.1/tackle/providers/ssh/hooks/interactive.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/ssh/hooks/ssh.py` & `tackle-0.5.1/tackle/providers/ssh/hooks/ssh.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/strings/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/strings/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/strings/hooks/b64.py` & `tackle-0.5.1/tackle/providers/strings/hooks/b64.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/strings/hooks/randoms.py` & `tackle-0.5.1/tackle/providers/strings/hooks/randoms.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/strings/hooks/regex.py` & `tackle-0.5.1/tackle/providers/strings/hooks/regex.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/strings/hooks/strings.py` & `tackle-0.5.1/tackle/providers/strings/hooks/strings.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/strings/tests/strings/test_provider_system_split.py` & `tackle-0.5.1/tackle/providers/strings/tests/strings/test_provider_system_split.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/tackle/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/hooks/block.py` & `tackle-0.5.1/tackle/providers/tackle/hooks/block.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/hooks/debug.py` & `tackle-0.5.1/tackle/providers/tackle/hooks/debug.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/hooks/flatten.py` & `tackle-0.5.1/tackle/providers/tackle/hooks/flatten.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/hooks/import.py` & `tackle-0.5.1/tackle/providers/tackle/hooks/import.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/hooks/provider_docs.py` & `tackle-0.5.1/tackle/providers/tackle/hooks/provider_docs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/hooks/run_hook.py` & `tackle-0.5.1/tackle/providers/tackle/hooks/run_hook.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/hooks/tackle.py` & `tackle-0.5.1/tackle/providers/tackle/hooks/tackle.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/hooks/variable.py` & `tackle-0.5.1/tackle/providers/tackle/hooks/variable.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/tests/block/test_provider_tackle_block.py` & `tackle-0.5.1/tackle/providers/tackle/tests/block/test_provider_tackle_block.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/tests/flatten/kubectl.yaml` & `tackle-0.5.1/tackle/providers/tackle/tests/flatten/kubectl.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/tests/flatten/ls.yaml` & `tackle-0.5.1/tackle/providers/tackle/tests/flatten/ls.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/tests/flatten/test_provider_tackle_flatten.py` & `tackle-0.5.1/tackle/providers/tackle/tests/flatten/test_provider_tackle_flatten.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,7 +17,13 @@
     assert output['delete']['args']
 
 
 def test_provider_tackle_flatten_method(change_dir):
     output = tackle('method.yaml', no_input=True)
 
     assert output
+
+
+def test_provider_tackle_flatten_splat(change_dir):
+    output = tackle('splat.yaml', no_input=True)
+
+    assert output
```

### Comparing `tackle-0.5.0/tackle/providers/tackle/tests/import/test_provider_tackle_import.py` & `tackle-0.5.1/tackle/providers/tackle/tests/import/test_provider_tackle_import.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/tests/provider_docs/test_tackle_provider_docs.py` & `tackle-0.5.1/tackle/providers/tackle/tests/provider_docs/test_tackle_provider_docs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/tackle/tests/tackle/test_provider_tackle_tackle.py` & `tackle-0.5.1/tackle/providers/tackle/tests/tackle/test_provider_tackle_tackle.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/toml/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/toml/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/toml/hooks/tomls.py` & `tackle-0.5.1/tackle/providers/toml/hooks/tomls.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/types/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/types/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/types/hooks/casting.py` & `tackle-0.5.1/tackle/providers/types/hooks/casting.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/types/hooks/type.py` & `tackle-0.5.1/tackle/providers/types/hooks/type.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/types/tests/test_provider_types.py` & `tackle-0.5.1/tackle/providers/types/tests/test_provider_types.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/web/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/web/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/web/hooks/browser.py` & `tackle-0.5.1/tackle/providers/web/hooks/browser.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/web/hooks/request.py` & `tackle-0.5.1/tackle/providers/web/hooks/request.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/web/tests/test_requests_provider.py` & `tackle-0.5.1/tackle/providers/web/tests/test_requests_provider.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/yaml/.tackle.meta.yaml` & `tackle-0.5.1/tackle/providers/yaml/.tackle.meta.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/yaml/hooks/yaml_in_place.py` & `tackle-0.5.1/tackle/providers/yaml/hooks/yaml_in_place.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/yaml/hooks/yamls.py` & `tackle-0.5.1/tackle/providers/yaml/hooks/yamls.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/providers/yaml/tests/test_provider_system_yaml.py` & `tackle-0.5.1/tackle/providers/yaml/tests/test_provider_system_yaml.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/render.py` & `tackle-0.5.1/tackle/render.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/settings.py` & `tackle-0.5.1/tackle/settings.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/special_vars.py` & `tackle-0.5.1/tackle/special_vars.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/utils/command.py` & `tackle-0.5.1/tackle/utils/command.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,15 +63,22 @@
         output.append(literal_eval(i))
     return output
 
 
 def unpack_args_kwargs_string(input_string: str) -> (list, dict, list):
     """Split up based on whitespace input args and pass to unpack_args_kwargs_list."""
     input_list = split_input_string(input_string)
-    return unpack_args_kwargs_list(input_list)
+
+    args, kwargs, flags = unpack_args_kwargs_list(input_list)
+
+    clean_kwargs = {k.replace('-', '_'): v for k, v in kwargs.items()}
+    clean_flags = [i.replace('-', '_') for i in flags]
+
+    return args, clean_kwargs, clean_flags
+    # return unpack_args_kwargs_list(input_list)
 
 
 def assert_if_flag(arg: str):
     FLAG_REGEX = re.compile(
         r"""^[\-|\-\-]+[a-zA-Z0-9]""",
         re.VERBOSE,
     )
```

### Comparing `tackle-0.5.0/tackle/utils/dicts.py` & `tackle-0.5.1/tackle/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/utils/files.py` & `tackle-0.5.1/tackle/utils/files.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/utils/help.py` & `tackle-0.5.1/tackle/utils/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,17 @@
         # Show the other options outside the default hook
         general_kwargs.append(f"[--{i['name']}]")
 
     # Remove the `help` str from the `usage` line in help.
     if context.input_string[-4:] == 'help':
         context.input_string = context.input_string[:-4]
 
+    # Determine max width of each kwarg / arg / method for formatting
+
+
     template = Template(HELP_TEMPLATE)
     help_rendered = template.render(
         args=args,
         kwargs=kwargs,
         flags=flags,
         general_help=general_help,
         general_kwargs=general_kwargs,
```

### Comparing `tackle-0.5.0/tackle/utils/log.py` & `tackle-0.5.1/tackle/utils/log.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/utils/paths.py` & `tackle-0.5.1/tackle/utils/paths.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/utils/prompts.py` & `tackle-0.5.1/tackle/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/utils/vcs.py` & `tackle-0.5.1/tackle/utils/vcs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle/utils/zipfile.py` & `tackle-0.5.1/tackle/utils/zipfile.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tackle.egg-info/PKG-INFO` & `tackle-0.5.1/tackle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tackle
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tackle is a declarative DSL for building modular workflows and code generators. Tool is plugins based and can easily be extended by writing additional hooks or importing external providers that can be turned into a self documenting CLI, all out of yaml, json, toml.
 Home-page: https://github.com/robcxyz/tackle
 Author: Rob Cannon
 Author-email: robc.io.opensource@gmail.com
 License: BSD
 Description: <img align="right" width="280" height="280" src="https://raw.githubusercontent.com/sudoblockio/tackle/main/docs/assets/logo-box.png">
```

### Comparing `tackle-0.5.0/tackle.egg-info/SOURCES.txt` & `tackle-0.5.1/tackle.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -604,16 +604,23 @@
 tests/models/fixtures/test-provider-reqs/hooks/hooks.py
 tests/models/fixtures/test-provider/hooks/thing.py
 tests/parser/test_parser_args_handler.py
 tests/parser/test_parser_base_methods.py
 tests/parser/test_parser_exceptions.py
 tests/parser/test_parser_hook_arguments.py
 tests/parser/test_parser_macros.py
-tests/parser/test_parser_parse_hook.py
-tests/parser/test_source.py
+tests/parser/test_parser_parse.py
+tests/parser/.functions/fixtures/func-provider-hook/funcs.yaml
+tests/parser/.functions/fixtures/functions/hook-config.yaml
+tests/parser/.functions/fixtures/functions/merge-field.yaml
+tests/parser/.functions/provider-fixtures/func-provider/tackle.yaml
+tests/parser/.functions/provider-fixtures/func-provider/a-dir/.gitkeep
+tests/parser/.functions/provider-fixtures/func-provider/hooks/funks.yaml
+tests/parser/.functions/provider-fixtures/only-hooks-dir/a-dir/.gitkeep
+tests/parser/.functions/provider-fixtures/only-hooks-dir/hooks/funks.yaml
 tests/parser/base-method-fixtures/list-comprehension.yaml
 tests/parser/base-method-fixtures/merge-dict-loop-dict.yaml
 tests/parser/base-method-fixtures/merge-dict-loop-exception.yaml
 tests/parser/base-method-fixtures/merge-dict.yaml
 tests/parser/base-method-fixtures/merge-list-dict.yaml
 tests/parser/base-method-fixtures/merge-list-loop-dict.yaml
 tests/parser/base-method-fixtures/merge-list-loop-value.yaml
@@ -631,83 +638,81 @@
 tests/parser/exceptions-fixtures/empty.yaml
 tests/parser/exceptions-fixtures/function-input-validation-error.yaml
 tests/parser/exceptions-fixtures/hook-input-validation-error.yaml
 tests/parser/exceptions-fixtures/merge-error.yaml
 tests/parser/exceptions-fixtures/out-of-range-arg.yaml
 tests/parser/exceptions-fixtures/calling_dir/.gitkeep
 tests/parser/exceptions-fixtures/calling_dir/calling.yaml
-tests/parser/fixtures/ansible-playbook.yaml
-tests/parser/fixtures/arg-types-output.yaml
-tests/parser/fixtures/arg-types.yaml
 tests/parser/fixtures/args.yaml
-tests/parser/fixtures/block-output.yaml
-tests/parser/fixtures/block.yaml
-tests/parser/fixtures/bug-mixed-flags-output.yaml
-tests/parser/fixtures/bug-mixed-flags.yaml
-tests/parser/fixtures/calling-context-inner.yaml
-tests/parser/fixtures/calling-context.yaml
-tests/parser/fixtures/docker-compose.yml
+tests/parser/fixtures/copied-hook-args.yaml
 tests/parser/fixtures/document-hooks-expected.yaml
 tests/parser/fixtures/document-hooks.yaml
-tests/parser/fixtures/dunder-key.yaml
 tests/parser/fixtures/duplicate-values.yaml
-tests/parser/fixtures/embedded_list.yaml
-tests/parser/fixtures/empty-elements.yaml
-tests/parser/fixtures/empty-hooks-output.yaml
-tests/parser/fixtures/empty-hooks.yaml
 tests/parser/fixtures/inner-tackle-list.yaml
 tests/parser/fixtures/inner-tackle.yaml
-tests/parser/fixtures/k8s-deployment.yaml
-tests/parser/fixtures/list-list.yaml
-tests/parser/fixtures/map-lists-output.yaml
-tests/parser/fixtures/map-lists.yaml
-tests/parser/fixtures/map-output.yaml
-tests/parser/fixtures/map-root-output.yaml
-tests/parser/fixtures/map-root.yaml
-tests/parser/fixtures/map.yaml
-tests/parser/fixtures/match-case-logic.yaml
 tests/parser/fixtures/merge-petstore-compact.yaml
 tests/parser/fixtures/merge-petstore.yaml
-tests/parser/fixtures/merge-simple-output.yaml
-tests/parser/fixtures/merge-simple.yaml
 tests/parser/fixtures/outer-tackle-arg.yaml
 tests/parser/fixtures/outer-tackle-list-output.yaml
 tests/parser/fixtures/outer-tackle-list.yaml
 tests/parser/fixtures/outer-tackle-output.yaml
 tests/parser/fixtures/outer-tackle.yaml
 tests/parser/fixtures/petstore.yaml
-tests/parser/fixtures/private-context-output.yaml
-tests/parser/fixtures/private-context.yaml
-tests/parser/fixtures/private-hooks-output.yaml
-tests/parser/fixtures/private-hooks.yaml
-tests/parser/fixtures/remote.yaml
-tests/parser/fixtures/ruamel-parsing-error-braces.yaml
-tests/parser/fixtures/toml.toml
-tests/parser/fixtures/toml.yaml
 tests/parser/fixtures/types.yaml
-tests/parser/fixtures/var-hook-output.yaml
-tests/parser/fixtures/var-hook.yaml
 tests/parser/fixtures/.old/merge-key-simple.yaml
-tests/parser/fixtures/blocks/ansible-parse-call.yaml
-tests/parser/fixtures/blocks/ansible-parse-output.yaml
-tests/parser/fixtures/blocks/ansible-parse.yaml
-tests/parser/fixtures/blocks/empty-block-exception.yaml
-tests/parser/fixtures/blocks/nested-dict-output.yaml
-tests/parser/fixtures/blocks/nested-dict.yaml
-tests/parser/fixtures/blocks/nested-for-output.yaml
-tests/parser/fixtures/blocks/nested-for.yaml
-tests/parser/fixtures/blocks/single-level-output.yaml
-tests/parser/fixtures/blocks/single-level.yaml
 tests/parser/fixtures/dir/tackle.yaml
 tests/parser/fixtures/input-key/tackle.yaml
 tests/parser/fixtures/input-key/child/.gitkeep
 tests/parser/fixtures/input-key/child/calling.yaml
-tests/parser/fixtures/macros/compact-hook-macro.yaml
-tests/parser/fixtures/macros/list-block.yaml
 tests/parser/fixtures/templates/file.py
+tests/parser/macro-fixtures/ansible-parse-call.yaml
+tests/parser/macro-fixtures/ansible-parse-output.yaml
+tests/parser/macro-fixtures/ansible-parse.yaml
+tests/parser/macro-fixtures/calling-context-inner.yaml
+tests/parser/macro-fixtures/calling-context.yaml
+tests/parser/macro-fixtures/compact-hook-macro.yaml
+tests/parser/macro-fixtures/empty-block-exception.yaml
+tests/parser/macro-fixtures/inner-tackle.yaml
+tests/parser/macro-fixtures/list-block.yaml
+tests/parser/macro-fixtures/nested-dict-output.yaml
+tests/parser/macro-fixtures/nested-dict.yaml
+tests/parser/macro-fixtures/nested-for-output.yaml
+tests/parser/macro-fixtures/nested-for.yaml
+tests/parser/macro-fixtures/ruamel-parsing-error-braces.yaml
+tests/parser/macro-fixtures/single-level-output.yaml
+tests/parser/macro-fixtures/single-level.yaml
+tests/parser/parse-fixtures/ansible-playbook.yaml
+tests/parser/parse-fixtures/arg-types-output.yaml
+tests/parser/parse-fixtures/arg-types.yaml
+tests/parser/parse-fixtures/block-output.yaml
+tests/parser/parse-fixtures/block.yaml
+tests/parser/parse-fixtures/bug-mixed-flags-output.yaml
+tests/parser/parse-fixtures/bug-mixed-flags.yaml
+tests/parser/parse-fixtures/docker-compose.yml
+tests/parser/parse-fixtures/empty-elements.yaml
+tests/parser/parse-fixtures/empty-hooks-output.yaml
+tests/parser/parse-fixtures/empty-hooks.yaml
+tests/parser/parse-fixtures/k8s-deployment.yaml
+tests/parser/parse-fixtures/list-list.yaml
+tests/parser/parse-fixtures/map-lists-output.yaml
+tests/parser/parse-fixtures/map-lists.yaml
+tests/parser/parse-fixtures/map-output.yaml
+tests/parser/parse-fixtures/map-root-output.yaml
+tests/parser/parse-fixtures/map-root.yaml
+tests/parser/parse-fixtures/map.yaml
+tests/parser/parse-fixtures/merge-simple-output.yaml
+tests/parser/parse-fixtures/merge-simple.yaml
+tests/parser/parse-fixtures/private-context-output.yaml
+tests/parser/parse-fixtures/private-context.yaml
+tests/parser/parse-fixtures/private-hooks-output.yaml
+tests/parser/parse-fixtures/private-hooks.yaml
+tests/parser/parse-fixtures/toml.toml
+tests/parser/parse-fixtures/toml.yaml
+tests/parser/parse-fixtures/var-hook-output.yaml
+tests/parser/parse-fixtures/var-hook.yaml
 tests/render/test_environment.py
 tests/render/test_extensions.py
 tests/render/test_render.py
 tests/render/test_render_exceptions.py
 tests/render/test_special_variables.py
 tests/render/fixtures/call-function-output.yaml
 tests/render/fixtures/call-function.yaml
```

### Comparing `tackle-0.5.0/tests/cli/test_cli.py` & `tackle-0.5.1/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/cli/test_cli_args.py` & `tackle-0.5.1/tests/cli/test_cli_args.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/cli/test_cli_commands.py` & `tackle-0.5.1/tests/cli/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/exceptions/test_tackle_exceptions.py` & `tackle-0.5.1/tests/exceptions/test_tackle_exceptions.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-embedded.yaml` & `tackle-0.5.1/tests/functions/cli-fixtures/cli-default-hook-embedded.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/cli-fixtures/cli-default-hook-no-context.yaml` & `tackle-0.5.1/tests/functions/cli-fixtures/cli-default-hook-no-context.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/field-hooks-fixtures/extends-visible.yaml` & `tackle-0.5.1/tests/functions/field-hooks-fixtures/extends-visible.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/fixtures/field-types.yaml` & `tackle-0.5.1/tests/functions/fixtures/field-types.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/method-fixtures/method-nested-override.yaml` & `tackle-0.5.1/tests/functions/method-fixtures/method-nested-override.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/test_function_calls.py` & `tackle-0.5.1/tests/functions/test_function_calls.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/test_functions.py` & `tackle-0.5.1/tests/functions/test_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -149,15 +149,33 @@
 def test_function_import_func_from_hooks_dir_call_method(change_curdir_fixtures):
     """Check that we can call a method on an imported hook from a hooks directory."""
     os.chdir(os.path.join('func-provider-method', 'a-dir'))
     o = tackle(a_field='an-arg')
     assert o['t']['p'] == 'a-default'
 
 
-def test_function_import_func_from_hooks_dir_call_function_cli(change_curdir_fixtures):
+def test_function_run_hook_in_parent_preserve_context(change_curdir_fixtures):
+    """
+    Verify that we can call a hook in a parent dir and have some sensible environment
+     variables to work with.
+    """
+    os.chdir(os.path.join('func-provider-hook', 'a-dir'))
+    o = tackle('funcs.yaml', find_in_parent=True)
+    assert o
+
+
+def test_function_merge_field_into_hook(change_curdir_fixtures):
+    """Verify that we can merge a dict into the parent's field."""
+    os.chdir('functions')
+    x = os.listdir()
+    o = tackle('merge-field.yaml', 'foo')
+    assert o
+
+
+def test_function_import_func_from_hooks_dir_context_preserved2(change_curdir_fixtures):
     """
     Check that we can call a function on an imported hook from a hooks directory when
      calling with args like in CLI.
     """
     os.chdir(os.path.join('func-provider-method', 'a-dir'))
     o = tackle('a_funky')
     assert o == 'a-default'
```

### Comparing `tackle-0.5.0/tests/functions/test_functions_args_kwargs_hooks.py` & `tackle-0.5.1/tests/functions/test_functions_args_kwargs_hooks.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/test_functions_cli.py` & `tackle-0.5.1/tests/functions/test_functions_cli.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/test_functions_enums.py` & `tackle-0.5.1/tests/functions/test_functions_enums.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/test_functions_exceptions.py` & `tackle-0.5.1/tests/functions/test_functions_exceptions.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/test_functions_field_hooks.py` & `tackle-0.5.1/tests/functions/test_functions_field_hooks.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/test_functions_help.py` & `tackle-0.5.1/tests/functions/test_functions_help.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/functions/test_functions_types.py` & `tackle-0.5.1/tests/functions/test_functions_types.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/macros/test_macros.py` & `tackle-0.5.1/tests/macros/test_macros.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/main/test_main.py` & `tackle-0.5.1/tests/main/test_main.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/models/fixtures/text2art.yaml` & `tackle-0.5.1/tests/models/fixtures/text2art.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/models/test_models.py` & `tackle-0.5.1/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/models/test_models_providers.py` & `tackle-0.5.1/tests/models/test_models_providers.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/base-method-fixtures/method-else.yaml` & `tackle-0.5.1/tests/parser/base-method-fixtures/method-else.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/base-method-fixtures/method-except.yaml` & `tackle-0.5.1/tests/parser/base-method-fixtures/method-except.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/fixtures/block-output.yaml` & `tackle-0.5.1/tests/parser/parse-fixtures/block-output.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/fixtures/block.yaml` & `tackle-0.5.1/tests/parser/parse-fixtures/block.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/fixtures/blocks/ansible-parse-output.yaml` & `tackle-0.5.1/tests/parser/macro-fixtures/ansible-parse-output.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/fixtures/blocks/ansible-parse.yaml` & `tackle-0.5.1/tests/parser/macro-fixtures/ansible-parse.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/fixtures/blocks/nested-for-output.yaml` & `tackle-0.5.1/tests/parser/macro-fixtures/nested-for-output.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/fixtures/blocks/nested-for.yaml` & `tackle-0.5.1/tests/parser/macro-fixtures/nested-for.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/fixtures/docker-compose.yml` & `tackle-0.5.1/tests/parser/parse-fixtures/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/fixtures/empty-hooks-output.yaml` & `tackle-0.5.1/tests/parser/parse-fixtures/empty-hooks-output.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/fixtures/empty-hooks.yaml` & `tackle-0.5.1/tests/parser/parse-fixtures/empty-hooks.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/fixtures/petstore.yaml` & `tackle-0.5.1/tests/parser/fixtures/petstore.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/parser/test_parser_args_handler.py` & `tackle-0.5.1/tests/parser/test_parser_args_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import pytest
 
 from tackle import tackle
-
-# from tackle.parser import handle_leading_brackets
 from tackle.macros import var_hook_macro
 from tackle.utils.command import unpack_args_kwargs_string
 
 TEMPLATES = [
     # These should all have `var` prepended to the args as it is indicative of a render
     ('"{{foo}}" bar baz', 4, 0, 0),
     ('{{ foo }} bar baz', 4, 0, 0),
@@ -17,15 +15,15 @@
     ('bar-{{ foo }}-foo', 2, 0, 0),
     ('bar-{{ foo in var }}-foo', 2, 0, 0),
 ]
 
 
 @pytest.mark.parametrize("template,len_args,len_kwargs,len_flags", TEMPLATES)
 def test_unpack_args_kwargs_handle_leading_brackets(
-    template, len_args, len_kwargs, len_flags
+        template, len_args, len_kwargs, len_flags
 ):
     """Validate the count of each input arg/kwarg/flag."""
     args, kwargs, flags = unpack_args_kwargs_string(template)
     args = var_hook_macro(args)
 
     assert len_args == len(args)
     assert len_kwargs == len(kwargs)
```

### Comparing `tackle-0.5.0/tests/parser/test_parser_base_methods.py` & `tackle-0.5.1/tests/parser/test_parser_base_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 import pytest
-from ruamel.yaml import YAML
 from tackle import tackle
 from tackle import exceptions
 
 
-def test_parser_methods_merge(change_curdir_fixtures):
-    """Verify we can run tackle against a fixture and merge it up to equal the same."""
-    yaml = YAML()
-    with open('petstore.yaml') as f:
-        expected_output = yaml.load(f)
-
-    output = tackle('merge-petstore-compact.yaml')
-    assert output == expected_output
-
-
 @pytest.fixture()
 def fixture_dir(chdir):
     chdir("base-method-fixtures")
 
 
 def test_parser_methods_merge_dict(fixture_dir):
     """Validate merging a dict into a dict."""
```

### Comparing `tackle-0.5.0/tests/parser/test_parser_exceptions.py` & `tackle-0.5.1/tests/parser/test_parser_exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-"""Test the input source part of the parser."""
 import pytest
 
 from tackle import exceptions
 
 # from tackle import tackle
 from tackle.cli import main
```

### Comparing `tackle-0.5.0/tests/parser/test_parser_hook_arguments.py` & `tackle-0.5.1/tests/parser/test_parser_hook_arguments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-"""Verify hook argument related items."""
 import pytest
 from tackle.utils.command import unpack_args_kwargs_string
 from tackle import tackle
 
 FIXTURES = [
     ("this --if \"expanded == 'that'\"", ["this"], {"if": "expanded == 'that'"}, []),
     (
@@ -36,18 +35,7 @@
     assert output['outer']['foo_items'] == ['bar', 'baz']
 
 
 def test_parser_tackle_in_tackle_arg(change_curdir_fixtures):
     """Test input args."""
     output = tackle('outer-tackle-arg.yaml', no_input=True)
     assert output['outer']['foo_items'] == ['bar', 'baz']
-
-
-def test_parser_render_hook_input(change_curdir_fixtures):
-    """
-    Show that when the first argument is a renderable that you just render that with the
-    context and logic.
-    """
-    output = tackle('var-hook.yaml', no_input=True)
-    for k, v in output.items():
-        if k.startswith('stuff'):
-            assert v == 'things'
```

### Comparing `tackle-0.5.0/tests/parser/test_parser_macros.py` & `tackle-0.5.1/tests/parser/test_parser_macros.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 import pytest
-import os
 
 from tackle import tackle
 from tackle.utils.files import read_config_file
 from tackle.exceptions import EmptyBlockException
 
+
+@pytest.fixture()
+def fixture_dir(chdir):
+    chdir("macro-fixtures")
+
+
 FIXTURES = [
-    ('single-level.yaml', 'single-level-output.yaml'),
+    # TODO: Fix for odereddict output
+    # ('single-level.yaml', 'single-level-output.yaml'),
     ('nested-dict.yaml', 'nested-dict-output.yaml'),
     ('nested-for.yaml', 'nested-for-output.yaml'),
     # Consider RM - Too much stuff
     # ('ansible-parse-call.yaml', 'ansible-parse-output.yaml')
 ]
 
 
 @pytest.mark.parametrize("input,output", FIXTURES)
-def test_parser_blocks_validate_output(chdir, input, output):
+def test_parser_blocks_validate_output(fixture_dir, input, output):
     """Test blocks."""
-    chdir(os.path.join("fixtures", "blocks"))
-
     tackle_output = tackle(input)
     assert tackle_output == read_config_file(output)
 
 
 ERROR_SOURCES = [
     ("empty-block-exception.yaml", EmptyBlockException),
 ]
 
 
 @pytest.mark.parametrize("input_file,exception", ERROR_SOURCES)
-def test_parser_raises_exceptions(chdir, input_file, exception):
+def test_parser_raises_exceptions(fixture_dir, input_file, exception):
     """Validate that exceptions are raised."""
-    chdir(os.path.join("fixtures", "blocks"))
     with pytest.raises(exception):
         tackle(input_file)
 
 
-def test_parser_calling_directory_preserve(change_curdir_fixtures):
+def test_parser_calling_directory_preserve(fixture_dir):
     """Validate that the calling_directory param is carried over from hook calls."""
     output = tackle('calling-context.yaml')
     assert output['call']['call']['calling_file'] == 'calling-context.yaml'
 
 
-def test_parser_list_to_block_macro(change_curdir_fixtures):
-    os.chdir('macros')
+def test_parser_list_to_block_macro(fixture_dir):
     output = tackle('list-block.yaml')
     assert isinstance(output['foo'][1], list)
 
 
-def test_parser_compact_hook_call_macro(change_curdir_fixtures):
+def test_parser_compact_hook_call_macro(fixture_dir):
     """Check that embedded compact hooks are called appropriately."""
-    os.chdir('macros')
     output = tackle('compact-hook-macro.yaml')
     assert output['compact'] == 'things'
 
 
-# def test_parser_compact_hook_call_macro(change_curdir_fixtures):
-#     os.chdir('macros')
-#     output = tackle('compact-hook-macro2.yaml')
-#     assert output['compact'] == 'things'
+def test_parser_ruamel_braces(fixture_dir):
+    """
+    Validate super hack for ruamel parsing error where `stuff->: {{things}}`
+    (no quotes), ruamel interprets as:
+    'stuff': ordereddict([(ordereddict([('things', None)]), None)]).
+    """
+    output = tackle('ruamel-parsing-error-braces.yaml', verbose=True)
+    assert output['stuff'] == 'things'
+    assert output['a']['b'] is None
+    assert output['one'] == 'two'
```

### Comparing `tackle-0.5.0/tests/parser/test_parser_parse_hook.py` & `tackle-0.5.1/tests/parser/test_parser_parse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""High level tests for parser logic."""
 import pytest
 
 from tackle.main import tackle
 from tackle.utils.files import read_config_file
 
-FIXTURES = [
+# NOTE: Splitting up tests on fixtures between those located in `parse-fixtures`  and
+# `fixtures` directories respectively there are A, so many fixtures and B, some are
+# common and others are only for the below comparison test.
+
+PARSE_FIXTURES = [
     ('map.yaml', 'map-output.yaml'),
     ('map-lists.yaml', 'map-lists-output.yaml'),
     ('arg-types.yaml', 'arg-types-output.yaml'),
     ('empty-elements.yaml', 'empty-elements.yaml'),
     ('map-root.yaml', 'map-root-output.yaml'),
     ('private-hooks.yaml', 'private-hooks-output.yaml'),
-    ('outer-tackle.yaml', 'outer-tackle-output.yaml'),
-    ('outer-tackle-list.yaml', 'outer-tackle-list-output.yaml'),
     ('merge-simple.yaml', 'merge-simple-output.yaml'),
-    ('merge-petstore-compact.yaml', 'petstore.yaml'),
     ('private-context.yaml', 'private-context-output.yaml'),
     # Non tackle things
     ('k8s-deployment.yaml', 'k8s-deployment.yaml'),
     ('ansible-playbook.yaml', 'ansible-playbook.yaml'),
     ('docker-compose.yml', 'docker-compose.yml'),
     ('list-list.yaml', 'list-list.yaml'),
     ('var-hook.yaml', 'var-hook-output.yaml'),
@@ -26,35 +26,55 @@
     # # Broken
     # # TODO: https://github.com/robcxyz/tackle/issues/52
     # ('bug-mixed-flags.yaml', 'bug-mixed-flags.yaml'),
     # ('document-hooks.yaml', 'document-hooks-expected.yaml'),
 ]
 
 
-@pytest.mark.parametrize("fixture,expected_output", FIXTURES)
-def test_main_expected_output(change_curdir_fixtures, fixture, expected_output):
+@pytest.mark.parametrize("fixture,expected_output", PARSE_FIXTURES)
+def test_main_expected_output_parse_fixtures_dir(chdir, fixture, expected_output):
     """Input equals output."""
+    chdir("parse-fixtures")
+
     expected_output = read_config_file(expected_output)
     output = tackle(fixture)
     assert output == expected_output
 
 
-def test_parser_ruamel_braces(change_curdir_fixtures):
-    """
-    Validate super hack for ruamel parsing error where `stuff->: {{things}}`
-    (no quotes), ruamel interprets as:
-    'stuff': ordereddict([(ordereddict([('things', None)]), None)]).
-    """
-    output = tackle('ruamel-parsing-error-braces.yaml', verbose=True)
-    assert output['stuff'] == 'things'
-    assert output['a']['b'] is None
-    assert output['one'] == 'two'
+COMMON_FIXTURES = [
+    ('outer-tackle.yaml', 'outer-tackle-output.yaml'),
+    ('outer-tackle-list.yaml', 'outer-tackle-list-output.yaml'),
+    ('merge-petstore-compact.yaml', 'petstore.yaml'),
+    ('merge-petstore-compact.yaml', 'petstore.yaml'),
+]
+
+
+@pytest.mark.parametrize("fixture,expected_output", COMMON_FIXTURES)
+def test_main_expected_output_common_fixtures_dir(chdir, fixture, expected_output):
+    """Input equals output."""
+    chdir('fixtures')
+
+    expected_output = read_config_file(expected_output)
+    output = tackle(fixture)
+    assert output == expected_output
 
 
 def test_parser_duplicate_values(change_curdir_fixtures):
     """
     Validate that when we give a hook with duplicate values as what was set in the
      initial run (ie a tackle hook with `no_input` set), that we take the value from the
      hook.
     """
     output = tackle('duplicate-values.yaml', verbose=True)
     assert output['local']['two_args']
+
+
+def test_parser_hook_args_not_copied(change_curdir_fixtures):
+    """
+    When calling a hook with an arg, there was an issue with the hook's args being
+     copied from one hook call to the next of the same hook suggesting the hook was not
+     copied when called. This is to check that.
+    """
+    output = tackle('copied-hook-args.yaml')
+    assert output['upper'].isupper()
+    assert output['lower'].islower()
+    assert output['lower_default'].islower()
```

### Comparing `tackle-0.5.0/tests/render/fixtures/globals.yaml` & `tackle-0.5.1/tests/render/fixtures/globals.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/render/fixtures/special-variables.yaml` & `tackle-0.5.1/tests/render/fixtures/special-variables.yaml`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/render/test_environment.py` & `tackle-0.5.1/tests/render/test_environment.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/render/test_extensions.py` & `tackle-0.5.1/tests/render/test_extensions.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/render/test_render.py` & `tackle-0.5.1/tests/render/test_render.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/render/test_render_exceptions.py` & `tackle-0.5.1/tests/render/test_render_exceptions.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/files/test_utils_files.py` & `tackle-0.5.1/tests/utils/files/test_utils_files.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/fixtures/fake-repo-tmpl.zip` & `tackle-0.5.1/tests/utils/fixtures/fake-repo-tmpl.zip`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/fixtures/protected-fake-repo-tmpl.zip` & `tackle-0.5.1/tests/utils/fixtures/protected-fake-repo-tmpl.zip`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/test_log.py` & `tackle-0.5.1/tests/utils/test_log.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/test_paths.py` & `tackle-0.5.1/tests/utils/test_paths.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/test_unzip.py` & `tackle-0.5.1/tests/utils/test_unzip.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/test_utils.py` & `tackle-0.5.1/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/test_utils_command.py` & `tackle-0.5.1/tests/utils/test_utils_command.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/test_utils_dicts.py` & `tackle-0.5.1/tests/utils/test_utils_dicts.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/vcs/test_vcs.py` & `tackle-0.5.1/tests/utils/vcs/test_vcs.py`

 * *Files identical despite different names*

### Comparing `tackle-0.5.0/tests/utils/vcs/test_vcs_provider.py` & `tackle-0.5.1/tests/utils/vcs/test_vcs_provider.py`

 * *Files identical despite different names*

