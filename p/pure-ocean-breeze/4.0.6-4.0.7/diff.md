# Comparing `tmp/pure_ocean_breeze-4.0.6.tar.gz` & `tmp/pure_ocean_breeze-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-4.0.6.tar", last modified: Fri Jul 14 07:14:28 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-4.0.7.tar", last modified: Mon Jul 17 07:00:36 2023, max compression
```

## Comparing `pure_ocean_breeze-4.0.6.tar` & `pure_ocean_breeze-4.0.7.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.041613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.041613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    66752 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.041613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   268911 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.041613 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-14 07:14:28.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-14 07:14:28.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:14:28.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-14 07:14:28.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 07:14:28.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.964776 pure_ocean_breeze-4.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-17 07:00:36.964776 pure_ocean_breeze-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.948775 pure_ocean_breeze-4.0.7/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.952776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66752 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.952776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.952776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.952776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   271094 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.952776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.952776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.952776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.956776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.956776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.956776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.956776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.956776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.956776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.956776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.956776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.956776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.956776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.960776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.960776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.960776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.960776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.960776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.960776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.960776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.960776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.960776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.964776 pure_ocean_breeze-4.0.7/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:00:36.952776 pure_ocean_breeze-4.0.7/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-17 07:00:36.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-17 07:00:36.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:00:36.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-17 07:00:36.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 07:00:36.000000 pure_ocean_breeze-4.0.7/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:00:36.964776 pure_ocean_breeze-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-17 07:00:23.000000 pure_ocean_breeze-4.0.7/setup.py
```

### Comparing `pure_ocean_breeze-4.0.6/LICENSE` & `pure_ocean_breeze-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/PKG-INFO` & `pure_ocean_breeze-4.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 4.0.6
+Version: 4.0.7
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.0.6/README.md` & `pure_ocean_breeze-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-07-13 08:36:22"
-__version__ = "4.0.6"
+__updated__ = "2023-07-17 14:36:04"
+__version__ = "4.0.7"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/labor/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-07-13 12:17:42"
+__updated__ = "2023-07-17 14:55:20"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -3359,14 +3359,15 @@
         dates: List[pd.Timestamp],
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
         show_time: bool = 0,
         many_days: int = 1,
         n_jobs: int = 1,
+        use_mpire: bool = 0,
     ) -> None:
         the_func = partial(func)
         factor_new = []
         dates = [int(datetime.datetime.strftime(i, "%Y%m%d")) for i in dates]
         if many_days == 1:
             # 将需要更新的日子分块，每200天一组，一起运算
             dates_new_len = len(dates)
@@ -3409,25 +3410,36 @@
                 to_save.columns = ["date", "code", "fac"]
                 self.factor_steps.write_via_df(
                     to_save, self.factor_file_pinyin, tuple_col="fac"
                 )
                 return df
 
             if n_jobs > 1:
-                with concurrent.futures.ThreadPoolExecutor(
-                    max_workers=n_jobs
-                ) as executor:
-                    factor_new_more = list(
-                        tqdm.auto.tqdm(
-                            executor.map(
-                                cal_one, cut_points[:-many_days], cut_points[many_days:]
-                            ),
-                            total=len(cut_points[many_days:]),
+                if use_mpire:
+                    with WorkerPool(n_jobs=n_jobs) as pool:
+                        factor_new_more = pool.map(
+                            cal_one,
+                            cut_points[:-many_days],
+                            cut_points[many_days:],
+                            progress_bar=True,
+                        )
+                else:
+                    with concurrent.futures.ThreadPoolExecutor(
+                        max_workers=n_jobs
+                    ) as executor:
+                        factor_new_more = list(
+                            tqdm.auto.tqdm(
+                                executor.map(
+                                    cal_one,
+                                    cut_points[:-many_days],
+                                    cut_points[many_days:],
+                                ),
+                                total=len(cut_points[many_days:]),
+                            )
                         )
-                    )
                 factor_new = factor_new + factor_new_more
             else:
                 # 开始计算因子值
                 for date1, date2 in tqdm.auto.tqdm(cuts, desc="不知乘月几人归，落月摇情满江树。"):
                     df = cal_one(date1, date2)
                     factor_new.append(df)
         else:
@@ -3465,25 +3477,29 @@
                         to_save, self.factor_file_pinyin, tuple_col="fac"
                     )
                     return df
 
             pairs = self.forward_dates(dates, many_days=many_days)
             cuts2 = tuple(zip(pairs, dates))
             if n_jobs > 1:
-                with concurrent.futures.ThreadPoolExecutor(
-                    max_workers=n_jobs
-                ) as executor:
-                    factor_new_more = list(
-                        tqdm.auto.tqdm(
-                            executor.map(
-                                cal_two, pairs, dates
-                            ),
-                            total=len(pairs),
+                if use_mpire:
+                    with WorkerPool(n_jobs=n_jobs) as pool:
+                        factor_new_more = pool.map(
+                            cal_two, pairs, dates, progress_bar=True
+                        )
+                else:
+                    with concurrent.futures.ThreadPoolExecutor(
+                        max_workers=n_jobs
+                    ) as executor:
+                        factor_new_more = list(
+                            tqdm.auto.tqdm(
+                                executor.map(cal_two, pairs, dates),
+                                total=len(pairs),
+                            )
                         )
-                    )
                 factor_new = factor_new + factor_new_more
             else:
                 # 开始计算因子值
                 for date1, date2 in tqdm.auto.tqdm(cuts2, desc="知不可乎骤得，托遗响于悲风。"):
                     df = cal_two(date1, date2)
                     factor_new.append(df)
 
@@ -3498,14 +3514,15 @@
         dates: List[pd.Timestamp],
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
         show_time: bool = 0,
         many_days: int = 1,
         n_jobs: int = 1,
+        use_mpire: bool = 0,
     ) -> None:
         if len(dates) == 1 and many_days == 1:
             res = self.select_one_calculate(
                 dates[0],
                 func=func,
                 fields=fields,
                 show_time=show_time,
@@ -3515,14 +3532,15 @@
                 dates=dates,
                 func=func,
                 fields=fields,
                 chunksize=chunksize,
                 show_time=show_time,
                 many_days=many_days,
                 n_jobs=n_jobs,
+                use_mpire=use_mpire,
             )
         if res is not None:
             self.factor_new.append(res)
         return res
 
     @staticmethod
     def for_cross_via_str(func):
@@ -3589,25 +3607,27 @@
         self,
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
         show_time: bool = 0,
         many_days: int = 1,
         n_jobs: int = 1,
+        use_mpire: bool = 0,
     ):
         if len(self.dates_new) > 0:
             for interval in self.dates_new_intervals:
                 df = self.select_any_calculate(
                     dates=interval,
                     func=func,
                     fields=fields,
                     chunksize=chunksize,
                     show_time=show_time,
                     many_days=many_days,
                     n_jobs=n_jobs,
+                    use_mpire=use_mpire,
                 )
             if len(self.factor_new) > 0:
                 self.factor_new = pd.concat(self.factor_new)
                 # 拼接新的和旧的
                 self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
                 self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
                 new_end_date = datetime.datetime.strftime(
@@ -5652,15 +5672,15 @@
             else:
                 # raise NotImplementedError(f"{date}这一期的优化失败，请检查")
                 logger.warning(f"{name}在{date}这一期的优化失败，请检查")
                 return None
         else:
             return None
 
-    def optimize_many_days(self, startdate: int = STATES['START']):
+    def optimize_many_days(self, startdate: int = STATES["START"]):
         dates = [i for i in self.facs.index if i >= pd.Timestamp(str(startdate))]
         for date in tqdm.auto.tqdm(dates):
             fac = self.facs[self.facs.index == date].T.dropna()
             total_cap = self.total_caps[self.total_caps.index == date].T.dropna()
             indu_dummy = self.indu_dummys[self.indu_dummys.date <= date]
             indu_dummy = (
                 indu_dummy[indu_dummy.date == indu_dummy.date.max()]
@@ -5698,15 +5718,15 @@
         rets = pd.concat([ret, index, abret], axis=1).dropna()
         rets.columns = [f"{name}增强组合净值", f"{name}指数净值", f"{name}增强组合超额净值"]
         rets = (rets + 1).cumprod()
         rets = rets.apply(lambda x: x / x.iloc[0])
         comments = comments_on_twins(rets[f"{name}增强组合超额净值"], abret.dropna())
         return comments, rets
 
-    def run(self, startdate: int = STATES['START']) -> pd.DataFrame:
+    def run(self, startdate: int = STATES["START"]) -> pd.DataFrame:
         """运行规划求解
 
         Parameters
         ----------
         startdate : int, optional
             起始日期, by default 20130101
 
@@ -6757,39 +6777,42 @@
                 df = df[["fac"]]
         df = df.reset_index()
         df.columns = ["code", "fac"]
         df.insert(
             0, "date", pd.Timestamp(year=date.year, month=date.month, day=date.day)
         )
         if (df is not None) and (df.shape[0] > 0):
+            df1 = df.pivot(columns="code", index="date", values="fac")
             self.factor_steps.write_via_df(df, self.factor_file_pinyin, tuple_col="fac")
-            df = df.pivot(columns="code", index="date", values="fac")
-            return df
+            return df1
 
     def get_daily_factors(
         self,
         func: Callable,
         n_jobs: int = 1,
         fields: str = "*",
         resample_frequency: str = None,
         opens_in: bool = 0,
         highs_in: bool = 0,
         lows_in: bool = 0,
         amounts_in: bool = 0,
         merge_them: bool = 0,
+        use_mpire: bool = 0,
     ) -> None:
         """每次抽取chunksize天的截面上全部股票的分钟数据
         对每天的股票的数据计算因子值
 
         Parameters
         ----------
         func : Callable
             用于计算因子值的函数
         n_jobs : int, optional
             并行数量, by default 1
+        fields : str, optional
+            要读取的字段，可选包含`date,code,price,amount,saleamount,buyamount,action,saleid,saleprice,buyid,buyprice`，其中date,code必须包含, by default `'*'`
         resample_frequency : str, optional
             将逐笔数据转化为秒级或分钟频数据，可以填写要转化的频率，如'3s'（3秒数据），'1m'（1分钟数据），
             指定此参数后，将自动生成一个self.closes的收盘价矩阵(index为时间,columns为股票代码,values为收盘价)，
             可在循环计算的函数中使用`self.closes`来调用计算好的值, by default None
         opens_in : bool, optional
             在resample_frequency不为None的情况下，可以使用此参数，提前计算好开盘价矩阵(index为时间,columns为股票代码,values为开盘价)，
             可在循环计算的函数中使用`self.opens`来调用计算好的值，by default 0
@@ -6800,39 +6823,59 @@
             在resample_frequency不为None的情况下，可以使用此参数，提前计算好最低价矩阵(index为时间,columns为股票代码,values为最低价)，
             可在循环计算的函数中使用`self.lows`来调用计算好的值，by default 0
         amounts_in : bool, optional
             在resample_frequency不为None的情况下，可以使用此参数，提前计算好成交额矩阵(index为时间,columns为股票代码,values为成交量)，
             可在循环计算的函数中使用`self.amounts`来调用计算好的值，by default 0
         merge_them : bool, optional
             在resample_frequency不为None的情况下，可以使用此参数，将计算好的因子值合并到一起，生成类似于分钟数据的sql形式，by default 0
+        use_mpire : bool, optional
+            并行是否使用mpire，默认使用concurrent，by default 0
         """
         if len(self.dates_new) > 0:
             if n_jobs > 1:
-                with concurrent.futures.ThreadPoolExecutor(
-                    max_workers=n_jobs
-                ) as executor:
-                    self.factor_new = list(
-                        tqdm.auto.tqdm(
-                            executor.map(
-                                lambda x: self.select_one_calculate(
-                                    date=x,
-                                    func=func,
-                                    fields=fields,
-                                    resample_frequency=resample_frequency,
-                                    opens_in=opens_in,
-                                    highs_in=highs_in,
-                                    lows_in=lows_in,
-                                    amounts_in=amounts_in,
-                                    merge_them=merge_them,
-                                ),
-                                self.dates_new,
+                if use_mpire:
+                    with WorkerPool(n_jobs=n_jobs) as pool:
+                        self.factor_new = pool.map(
+                            lambda x: self.select_one_calculate(
+                                date=x,
+                                func=func,
+                                fields=fields,
+                                resample_frequency=resample_frequency,
+                                opens_in=opens_in,
+                                highs_in=highs_in,
+                                lows_in=lows_in,
+                                amounts_in=amounts_in,
+                                merge_them=merge_them,
                             ),
-                            total=len(self.dates_new),
+                            self.dates_new,
+                            progress_bar=True,
+                        )
+                else:
+                    with concurrent.futures.ThreadPoolExecutor(
+                        max_workers=n_jobs
+                    ) as executor:
+                        self.factor_new = list(
+                            tqdm.auto.tqdm(
+                                executor.map(
+                                    lambda x: self.select_one_calculate(
+                                        date=x,
+                                        func=func,
+                                        fields=fields,
+                                        resample_frequency=resample_frequency,
+                                        opens_in=opens_in,
+                                        highs_in=highs_in,
+                                        lows_in=lows_in,
+                                        amounts_in=amounts_in,
+                                        merge_them=merge_them,
+                                    ),
+                                    self.dates_new,
+                                ),
+                                total=len(self.dates_new),
+                            )
                         )
-                    )
             else:
                 for date in tqdm.auto.tqdm(self.dates_new, "您现在处于单核运算状态，建议仅在调试时使用单核"):
                     df = self.select_one_calculate(
                         date=date,
                         func=func,
                         resample_frequency=resample_frequency,
                         opens_in=opens_in,
@@ -6844,15 +6887,15 @@
                     self.factor_new.append(df)
             # 拼接新的和旧的
             if self.factor_old is not None:
                 self.factor = pd.concat(
                     [self.factor_old] + self.factor_new
                 ).sort_index()
             else:
-                self.factor = self.factor_new.sort_index()
+                self.factor = pd.concat(self.factor_new).sort_index()
             self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
             new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
             # 存入本地
             self.factor.to_parquet(self.factor_file)
             logger.info(f"截止到{new_end_date}的因子值计算完了")
             # 删除存储在questdb的中途备份数据
             try:
```

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 4.0.6
+Version: 4.0.7
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-4.0.7/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.6/setup.py` & `pure_ocean_breeze-4.0.7/setup.py`

 * *Files identical despite different names*

