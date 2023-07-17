# Comparing `tmp/m-abac-1.0.1.tar.gz` & `tmp/m-abac-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-1.0.1.tar", last modified: Mon May 15 09:22:41 2023, max compression
+gzip compressed data, was "m-abac-1.0.2.tar", last modified: Mon Jul 17 15:48:03 2023, max compression
```

## Comparing `m-abac-1.0.1.tar` & `m-abac-1.0.2.tar`

### file list

```diff
@@ -1,96 +1,104 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.854042 m-abac-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1741 2023-05-15 09:22:41.853042 m-abac-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 09:21:42.000000 m-abac-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.808041 m-abac-1.0.1/m_abac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1741 2023-05-15 09:22:41.000000 m-abac-1.0.1/m_abac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3674 2023-05-15 09:22:41.000000 m-abac-1.0.1/m_abac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 09:22:41.000000 m-abac-1.0.1/m_abac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-15 09:22:41.000000 m-abac-1.0.1/m_abac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 09:22:41.000000 m-abac-1.0.1/m_abac.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.799041 m-abac-1.0.1/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.799041 m-abac-1.0.1/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.811041 m-abac-1.0.1/mobio/libs/abac/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.813041 m-abac-1.0.1/mobio/libs/abac/adapter/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 root         (0) root         (0)     8305 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/call_api.py
--rw-r--r--   0 root         (0) root         (0)    12582 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/pdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.816041 m-abac-1.0.1/mobio/libs/abac/policy/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.818041 m-abac-1.0.1/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.820041 m-abac-1.0.1/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.826041 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.831041 m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.835042 m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/base.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.838042 m-abac-1.0.1/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.844042 m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.846042 m-abac-1.0.1/mobio/libs/abac/policy/conditions/others/
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/others/base.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/others/exists.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 root         (0) root         (0)     2126 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:41.853042 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/not_ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/not_starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5812 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 root         (0) root         (0)     5139 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-05-15 09:21:42.000000 m-abac-1.0.1/mobio/libs/abac/result_access.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 09:21:42.000000 m-abac-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 09:22:41.854042 m-abac-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9774 2023-05-15 09:22:41.000000 m-abac-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.577034 m-abac-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-17 15:48:03.576034 m-abac-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      659 2023-07-17 15:45:49.000000 m-abac-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.508032 m-abac-1.0.2/m_abac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-17 15:48:03.000000 m-abac-1.0.2/m_abac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4095 2023-07-17 15:48:03.000000 m-abac-1.0.2/m_abac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:48:03.000000 m-abac-1.0.2/m_abac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2023-07-17 15:48:03.000000 m-abac-1.0.2/m_abac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-17 15:48:03.000000 m-abac-1.0.2/m_abac.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.485031 m-abac-1.0.2/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.485031 m-abac-1.0.2/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.513032 m-abac-1.0.2/mobio/libs/abac/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.515032 m-abac-1.0.2/mobio/libs/abac/adapter/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 root         (0) root         (0)    15511 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7862 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/call_api.py
+-rw-r--r--   0 root         (0) root         (0)     3491 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/config.py
+-rw-r--r--   0 root         (0) root         (0)    22074 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/pdp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.518032 m-abac-1.0.2/mobio/libs/abac/policy/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.522032 m-abac-1.0.2/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.524032 m-abac-1.0.2/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.532033 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 root         (0) root         (0)      418 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/any_contains.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.539033 m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.546033 m-abac-1.0.2/mobio/libs/abac/policy/conditions/day/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/day/base.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.550033 m-abac-1.0.2/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.562034 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/base_list.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/list_gt.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/list_gte.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/list_lt.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/list_lte.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.565034 m-abac-1.0.2/mobio/libs/abac/policy/conditions/others/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/others/base.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-r--r--   0 root         (0) root         (0)      702 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:48:03.575034 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/not_ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/not_starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7259 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-07-17 15:45:49.000000 m-abac-1.0.2/mobio/libs/abac/result_access.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-17 15:45:49.000000 m-abac-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 15:48:03.578034 m-abac-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9805 2023-07-17 15:48:02.000000 m-abac-1.0.2/setup.py
```

### Comparing `m-abac-1.0.1/PKG-INFO` & `m-abac-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: m-abac
-Version: 1.0.1
+Version: 1.0.2
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: ### ABAC Engine
-        Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control).
-        
-        
-        ### Cài đặt:
-        ```bash
-         $ pip3 install m-abac
-         ```
-        
-        ### Sử dụng:
-        
-        ##### Kiểm tra user có quyền thao tác hay không:
-           ```python
-            from mobio.libs.abac import PolicyDecisionPoint
-            resource = "deal"
-            # action = "UpdateFromSale"
-            action = "ListFromSale"
-        
-            pdb = PolicyDecisionPoint(resource=resource, action=action)
-            result = pdb.is_allowed()
-            if not result.get_allow_access():
-                # trả về lỗi không có quyền truy cập 
-           ```
-        #### Log - 1.0.0
-            - release sdk
-            
 Keywords: mobio,mobio-engine,m-abac
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+### ABAC Engine
+Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control).
+
+
+### Cài đặt:
+```bash
+ $ pip3 install m-abac
+ ```
+
+### Sử dụng:
+
+##### Kiểm tra user có quyền thao tác hay không:
+   ```python
+    from mobio.libs.abac import PolicyDecisionPoint
+    resource = "deal"
+    # action = "UpdateFromSale"
+    action = "ListFromSale"
+
+    pdb = PolicyDecisionPoint(resource=resource, action=action)
+    result = pdb.is_allowed()
+    if not result.get_allow_access():
+        # trả về lỗi không có quyền truy cập 
+   ```
+#### Log - 1.0.0
+    - release sdk
+#### Log - 1.0.2
+    - update sdk
+    
+
```

### Comparing `m-abac-1.0.1/README.md` & `m-abac-1.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -19,8 +19,11 @@
     pdb = PolicyDecisionPoint(resource=resource, action=action)
     result = pdb.is_allowed()
     if not result.get_allow_access():
         # trả về lỗi không có quyền truy cập 
    ```
 #### Log - 1.0.0
     - release sdk
+#### Log - 1.0.2
+    - update sdk
+
```

### Comparing `m-abac-1.0.1/m_abac.egg-info/PKG-INFO` & `m-abac-1.0.2/m_abac.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: m-abac
-Version: 1.0.1
+Version: 1.0.2
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: ### ABAC Engine
-        Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control).
-        
-        
-        ### Cài đặt:
-        ```bash
-         $ pip3 install m-abac
-         ```
-        
-        ### Sử dụng:
-        
-        ##### Kiểm tra user có quyền thao tác hay không:
-           ```python
-            from mobio.libs.abac import PolicyDecisionPoint
-            resource = "deal"
-            # action = "UpdateFromSale"
-            action = "ListFromSale"
-        
-            pdb = PolicyDecisionPoint(resource=resource, action=action)
-            result = pdb.is_allowed()
-            if not result.get_allow_access():
-                # trả về lỗi không có quyền truy cập 
-           ```
-        #### Log - 1.0.0
-            - release sdk
-            
 Keywords: mobio,mobio-engine,m-abac
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+### ABAC Engine
+Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control).
+
+
+### Cài đặt:
+```bash
+ $ pip3 install m-abac
+ ```
+
+### Sử dụng:
+
+##### Kiểm tra user có quyền thao tác hay không:
+   ```python
+    from mobio.libs.abac import PolicyDecisionPoint
+    resource = "deal"
+    # action = "UpdateFromSale"
+    action = "ListFromSale"
+
+    pdb = PolicyDecisionPoint(resource=resource, action=action)
+    result = pdb.is_allowed()
+    if not result.get_allow_access():
+        # trả về lỗi không có quyền truy cập 
+   ```
+#### Log - 1.0.0
+    - release sdk
+#### Log - 1.0.2
+    - update sdk
+    
+
```

### Comparing `m-abac-1.0.1/m_abac.egg-info/SOURCES.txt` & `m-abac-1.0.2/m_abac.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 m_abac.egg-info/PKG-INFO
 m_abac.egg-info/SOURCES.txt
 m_abac.egg-info/dependency_links.txt
 m_abac.egg-info/requires.txt
 m_abac.egg-info/top_level.txt
 mobio/libs/abac/__init__.py
 mobio/libs/abac/call_api.py
+mobio/libs/abac/config.py
 mobio/libs/abac/pdp.py
 mobio/libs/abac/result_access.py
 mobio/libs/abac/adapter/__init__.py
 mobio/libs/abac/adapter/adapter.py
 mobio/libs/abac/adapter/elasticsearch_adapter.py
 mobio/libs/abac/policy/__init__.py
 mobio/libs/abac/policy/exceptions.py
@@ -22,15 +23,17 @@
 mobio/libs/abac/policy/conditions/schema.py
 mobio/libs/abac/policy/conditions/boolean/__init__.py
 mobio/libs/abac/policy/conditions/boolean/base.py
 mobio/libs/abac/policy/conditions/boolean/check_bool.py
 mobio/libs/abac/policy/conditions/collection/__init__.py
 mobio/libs/abac/policy/conditions/collection/all_in.py
 mobio/libs/abac/policy/conditions/collection/all_not_in.py
+mobio/libs/abac/policy/conditions/collection/any_contains.py
 mobio/libs/abac/policy/conditions/collection/any_in.py
+mobio/libs/abac/policy/conditions/collection/any_not_contains.py
 mobio/libs/abac/policy/conditions/collection/any_not_in.py
 mobio/libs/abac/policy/conditions/collection/base.py
 mobio/libs/abac/policy/conditions/collection/is_empty.py
 mobio/libs/abac/policy/conditions/collection/is_in.py
 mobio/libs/abac/policy/conditions/collection/is_not_empty.py
 mobio/libs/abac/policy/conditions/collection/is_not_in.py
 mobio/libs/abac/policy/conditions/date_time/__init__.py
@@ -51,17 +54,22 @@
 mobio/libs/abac/policy/conditions/day/day_neq.py
 mobio/libs/abac/policy/conditions/ip_address/__init__.py
 mobio/libs/abac/policy/conditions/ip_address/base.py
 mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
 mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
 mobio/libs/abac/policy/conditions/numeric/__init__.py
 mobio/libs/abac/policy/conditions/numeric/base.py
+mobio/libs/abac/policy/conditions/numeric/base_list.py
 mobio/libs/abac/policy/conditions/numeric/eq.py
 mobio/libs/abac/policy/conditions/numeric/gt.py
 mobio/libs/abac/policy/conditions/numeric/gte.py
+mobio/libs/abac/policy/conditions/numeric/list_gt.py
+mobio/libs/abac/policy/conditions/numeric/list_gte.py
+mobio/libs/abac/policy/conditions/numeric/list_lt.py
+mobio/libs/abac/policy/conditions/numeric/list_lte.py
 mobio/libs/abac/policy/conditions/numeric/lt.py
 mobio/libs/abac/policy/conditions/numeric/lte.py
 mobio/libs/abac/policy/conditions/numeric/neq.py
 mobio/libs/abac/policy/conditions/others/__init__.py
 mobio/libs/abac/policy/conditions/others/base.py
 mobio/libs/abac/policy/conditions/others/exists.py
 mobio/libs/abac/policy/conditions/others/not_exists.py
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-1.0.2/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/call_api.py` & `m-abac-1.0.2/mobio/libs/abac/call_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,94 +1,78 @@
-from mobio.libs.caching import LruCache
-import os, requests
-
-
-class StoreCacheType:
-    LOCAL = 1
-    REDIS = 2
-
-class Cache:
-    REDIS_URI = "{}?health_check_interval=30".format(os.environ.get("ADMIN_REDIS_URI", os.environ.get("REDIS_URI")))
-    PREFIX = "m_abac"
-
-lru_cache_redis = LruCache(
-    store_type=StoreCacheType.REDIS,
-    redis_uri=Cache.REDIS_URI,
-    cache_prefix=Cache.PREFIX,
-)
-
-class Mobio:
-    ADMIN_HOST = os.environ.get("ADMIN_HOST")
-    MOBIO_TOKEN = "Basic {}".format(os.environ.get('YEK_REWOP', ''))
+import requests
 
+from .config import lru_cache_redis, Mobio
 
 
 class APIRequest:
     TimeOut = 10
     ADMIN_GET_FULL_INFO_ACCOUNT = "{domain}/adm/api/v2.1/accounts/{account_id}/full-info"
-    ADMIN_GET_LIST_ACTION_FOR_MERCHANT = "{domain}/adm/api/v2.1/policies/actions"
+    ADMIN_GET_LIST_ACTION_FOR_MERCHANT = "{domain}/adm/api/v2.1/policies/actions/sdk"
     ADMIN_GET_LIST_STATEMENT = "{domain}/adm/api/v2.1/statements"
 
+
 class CallAPI:
 
-    @lru_cache_redis.add()
+    # TODO: thay expiration cho production 15p
+    @lru_cache_redis.add(expiration=600)
     @staticmethod
     def admin_get_account_info(merchant_id, account_id):
-        try:
-            url = APIRequest.ADMIN_GET_FULL_INFO_ACCOUNT.format(domain=Mobio.ADMIN_HOST, account_id=account_id)
-            authorization = Mobio.MOBIO_TOKEN
-            data_res = requests.get(
-                url,
-                headers={
-                    "Authorization": authorization,
-                    "X-Merchant-ID": merchant_id,
-                },
-                timeout=APIRequest.TimeOut,
-            )
-            data = None
-            if data_res.status_code == 200:
-                if data_res.json().get("data"):
-                    data = data_res.json().get("data")
-            # print("admin_get_account_info: {}".format(data))
-            return data
-        except Exception as er:
-            err_msg = "admin_get_account_info err: {}".format(er)
-            print(err_msg)
-            return {}
+        # try:
+        url = APIRequest.ADMIN_GET_FULL_INFO_ACCOUNT.format(domain=Mobio.ADMIN_HOST, account_id=account_id)
+        authorization = Mobio.MOBIO_TOKEN
+        data_res = requests.get(
+            url,
+            headers={
+                "Authorization": authorization,
+                "X-Merchant-ID": merchant_id,
+            },
+            timeout=APIRequest.TimeOut,
+        )
+        data = None
+        if data_res.status_code == 200:
+            if data_res.json().get("data"):
+                data = data_res.json().get("data")
+        # print("abac_sdk admin_get_account_info: {}".format(data))
+        return data
+        # except Exception as er:
+        #     err_msg = "abac_sdk admin_get_account_info err: {}".format(er)
+        #     print(err_msg)
+        #     return {}
 
     @lru_cache_redis.add()
     @staticmethod
     def admin_get_json_action(merchant_id):
-        try:
-            url = APIRequest.ADMIN_GET_LIST_ACTION_FOR_MERCHANT.format(domain=Mobio.ADMIN_HOST)
-            authorization = Mobio.MOBIO_TOKEN
-            data_res = requests.get(
-                url,
-                headers={
-                    "Authorization": authorization,
-                    "X-Merchant-ID": merchant_id,
-                },
-                timeout=APIRequest.TimeOut,
-                params={"page": "-1"}
-            )
-            data = {}
-            if data_res.status_code == 200:
-                if data_res.json().get("data"):
-                    list_data = data_res.json().get("data")
-                    for i in list_data:
-                        data[i.get("key")] = i
-            # print("admin_get_json_action: {}".format(data))
-            return data
-        except Exception as er:
-            err_msg = "admin_get_json_action err: {}".format(er)
-            print(err_msg)
-            return {}
+        # try:
+        url = APIRequest.ADMIN_GET_LIST_ACTION_FOR_MERCHANT.format(domain=Mobio.ADMIN_HOST)
+        authorization = Mobio.MOBIO_TOKEN
+        data_res = requests.get(
+            url,
+            headers={
+                "Authorization": authorization,
+                "X-Merchant-ID": merchant_id,
+            },
+            timeout=APIRequest.TimeOut,
+            params={"page": "-1"}
+        )
+        data = {}
+        if data_res.status_code == 200:
+            if data_res.json().get("data"):
+                list_data = data_res.json().get("data")
+                for i in list_data:
+                    data[i.get("resource") + ":" + i.get("key")] = i
+        # print("abac_sdk admin_get_json_action: {}".format(data))
+        return data
+        # except Exception as er:
+        #     err_msg = "abac_sdk admin_get_json_action err: {}".format(er)
+        #     print(err_msg)
+        #     return {}
 
+    # TODO: thay expiration cho production 15p
     @staticmethod
-    @lru_cache_redis.add(expiration=900)
+    @lru_cache_redis.add(expiration=600)
     def admin_get_list_statement(merchant_id, account_id, resource, action, service):
         """
         :param merchant_id:
         :param account_id:
         :param resource:
         :param action:
         :return: [{
@@ -129,39 +113,40 @@
                     "qualifier": "ForAnyValue",
                     "if_exists": False,
                     "ignore_case": False
                 }
             ]
         }]
         """
-        try:
-            url = APIRequest.ADMIN_GET_LIST_STATEMENT.format(domain=Mobio.ADMIN_HOST)
-            authorization = Mobio.MOBIO_TOKEN
-            body_req = {
-                'user_ids': [account_id],
-                'team_ids': [],
-                'merchant_ids': [merchant_id],
-                'resources': [service + ":" + resource],
-                'actions': [resource + ":" + action]
-            }
-            data_res = requests.post(
-                url,
-                json=body_req,
-                headers={
-                    "Authorization": authorization,
-                    "X-Merchant-ID": merchant_id,
-                },
-                timeout=APIRequest.TimeOut,
-            )
-            data = None
-            if data_res.status_code == 200:
-                if data_res.json().get("statements"):
-                    data = data_res.json().get("statements")
-            # print("admin_get_list_statement: {}".format(data))
-            return data
+        # try:
+        url = APIRequest.ADMIN_GET_LIST_STATEMENT.format(domain=Mobio.ADMIN_HOST)
+        authorization = Mobio.MOBIO_TOKEN
+        body_req = {
+            'user_ids': [account_id],
+            'team_ids': [],
+            'merchant_ids': [merchant_id],
+            'resources': service + ":" + resource,
+            'actions': resource + ":" + action
+        }
+        data_res = requests.post(
+            url,
+            json=body_req,
+            headers={
+                "Authorization": authorization,
+                "X-Merchant-ID": merchant_id,
+            },
+            timeout=APIRequest.TimeOut,
+        )
+        data = None
+        if data_res.status_code == 200:
+            if data_res.json().get("statements"):
+                data = data_res.json().get("statements")
+        # TODO: comment log khi len prod
+        print("abac_sdk admin_get_list_statement: {}".format(data))
+        return data
 
             # return [
             #     {
             #         "effect": "allow",
             #         "action": [
             #             "ListFromSale"
             #         ],
@@ -220,11 +205,11 @@
             #                         "if_exists": False,
             #                         "ignore_case": False
             #                     }
             #                 ]
             #             }
             # ]
 
-        except Exception as er:
-            err_msg = "admin_get_list_statement err: {}".format(er)
-            print(err_msg)
-            return []
+        # except Exception as er:
+        #     err_msg = "abac_sdk admin_get_list_statement err: {}".format(er)
+        #     print(err_msg)
+        #     return []
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/base.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     Operation base class
 """
 
 from abc import ABCMeta, abstractmethod
 
 # from py_abac.context import EvaluationContext
-
+# what is value of field, values is list value policy
 MapAnyValue = ""
 
 class ConditionBase(metaclass=ABCMeta):
     """
         Base class for conditions
     """
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 class AllIn(CollectionCondition):
     """
         Condition for all values of `what` in `values`
     """
 
     def _is_satisfied(self) -> bool:
-        return set(self.what).issubset(self.values)
+        if not self.what:
+            return False
+        return set(self.values).issubset(self.what)
 
 
 class AllInSchema(CollectionConditionSchema):
     """
         JSON schema for all in collection condition
     """
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 class AllNotIn(CollectionCondition):
     """
         Condition for all values of `what` not in `values`
     """
 
     def _is_satisfied(self) -> bool:
-        return not set(self.what).issubset(self.values)
+        if not self.what:
+            return False
+        return not set(self.values).issubset(self.what)
 
 
 class AllNotInSchema(CollectionConditionSchema):
     """
         JSON schema for all not in collection condition
     """
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
-    Any of the values in collection conditions
+    Value is in collection conditions
 """
 
 from marshmallow import post_load
 
 from .base import CollectionCondition, CollectionConditionSchema
 
 
-class AnyIn(CollectionCondition):
+class IsIn(CollectionCondition):
     """
-        Condition for any value of `what` in `values`
+        Condition for `what` is a member of `values`
     """
 
     def _is_satisfied(self) -> bool:
-        return bool(set(self.what).intersection(self.values))
+        return self.what in self.values
 
 
-class AnyInSchema(CollectionConditionSchema):
+class IsInSchema(CollectionConditionSchema):
     """
-        JSON schema for any in collection condition
+        JSON schema for is in collection condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return AnyIn(**data)
+        return IsIn(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 class AnyNotIn(CollectionCondition):
     """
         Condition for any values of `what` not in `values`
     """
 
     def _is_satisfied(self) -> bool:
+        if not self.what:
+            return False
         return not bool(set(self.what).intersection(self.values))
 
 
 class AnyNotInSchema(CollectionConditionSchema):
     """
         JSON schema for any not in collection condition
     """
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
-    Value is in collection conditions
+    Any of the values in collection conditions
 """
 
 from marshmallow import post_load
 
 from .base import CollectionCondition, CollectionConditionSchema
 
 
-class IsIn(CollectionCondition):
+class AnyIn(CollectionCondition):
     """
-        Condition for `what` is a member of `values`
+        Condition for any value of `what` in `values`
     """
 
     def _is_satisfied(self) -> bool:
-        return self.what in self.values
+        if not self.what:
+            return False
+        return bool(set(self.what).intersection(self.values))
 
 
-class IsInSchema(CollectionConditionSchema):
+class AnyInSchema(CollectionConditionSchema):
     """
-        JSON schema for is in collection condition
+        JSON schema for any in collection condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return IsIn(**data)
+        return AnyIn(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class DateCondition(ConditionBase, metaclass=ABCMeta):
     """
         Base class for string conditions
     """
 
     class DateFormat:
-        ISO_FORMAT = "%Y-%m-%d %H:%M:%S"
+        ISO_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
     def __init__(self, values, what, date_format=DateFormat.ISO_FORMAT, qualifier=ConditionBase.Qualifier.ForAnyValue, **kwargs):
         self.values = values
         self.what = what
         self.qualifier = qualifier
         self.date_format = date_format
 
@@ -33,47 +33,47 @@
 
             :param what: string value to check
             :return: True if satisfied else False
         """
         raise NotImplementedError()
 
     def convert_string_to_timestamp(self, date_str):
-        return round(datetime.datetime.strptime(date_str, self.date_format).replace(
-            tzinfo=datetime.timezone.utc
-        ).timestamp())
+        return round(datetime.datetime.strptime(date_str, self.date_format).timestamp())
 
     def convert_date_to_timestamp(self, d):
-        return d.timestamp()
+        return round(d.timestamp())
 
     def convert_timestamp_to_date(self, timestamp):
         # try:
-        return datetime.datetime.utcfromtimestamp(timestamp).replace(
-            tzinfo=datetime.timezone.utc
-        )
+        return datetime.datetime.fromtimestamp(timestamp)
         # except:
         #     return None
 
     def convert_timestamp_from_any(self, i):
-        if isinstance(i, int):
+        if isinstance(i, int) or isinstance(i, float):
             if not self.convert_timestamp_to_date(i) or self.convert_timestamp_to_date(i).year == 1970:
                 return False
-            timestamp_i = i
+            timestamp_i = round(i)
         elif isinstance(i, str):
             timestamp_i = self.convert_string_to_timestamp(i)
         elif isinstance(i, datetime.datetime):
             timestamp_i = self.convert_date_to_timestamp(i)
         else:
             return False
-        return timestamp_i
+        return self.convert_timestamp_to_round_minute(timestamp_i)
+
+    def convert_timestamp_to_round_minute(self, value_timestamp):
+        round_timestamp = round(value_timestamp)
+        return round_timestamp - (round_timestamp % 60)
 
 class DateConditionSchema(Schema):
     """
         Base JSON schema for string conditions
     """
     values = fields.List(fields.Raw(required=True, allow_none=False), required=True, allow_none=False)
     what = fields.Raw(required=True, allow_none=False)
     qualifier = fields.String(allow_none=False, load_default=ConditionBase.Qualifier.ForAnyValue,
-                            validate=validate.OneOf([ConditionBase.Qualifier.ALL]))
+                            validate=validate.OneOf(ConditionBase.Qualifier.ALL))
     date_format = fields.String(allow_none=False, load_default=DateCondition.DateFormat.ISO_FORMAT,)
 
     class Meta:
         unknown = EXCLUDE
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 
 class DateEq(DateCondition):
     """
         Condition for number `what` equals `value`
     """
 
     def _is_satisfied(self) -> bool:
+        timestamp_what = self.convert_timestamp_from_any(self.what)
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
                 timestamp_i = self.convert_timestamp_from_any(i)
                 if not timestamp_i or not timestamp_what:
                     return False
                 if timestamp_what == timestamp_i:
                     return True
             return False
         else:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
                 timestamp_i = self.convert_timestamp_from_any(i)
                 if not timestamp_i or not timestamp_what:
                     return False
                 if timestamp_what != timestamp_i:
                     return False
             return True
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 
 class DateGt(DateCondition):
     """
         Condition for number `what` greater than `value`
     """
 
     def _is_satisfied(self) -> bool:
+        timestamp_what = self.convert_timestamp_from_any(self.what)
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
                 timestamp_i = self.convert_timestamp_from_any(i)
                 if not timestamp_i or not timestamp_what:
                     return False
                 if timestamp_what > timestamp_i:
                     return True
             return False
         else:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
                 timestamp_i = self.convert_timestamp_from_any(i)
                 if not timestamp_i or not timestamp_what:
                     return False
                 if timestamp_what <= timestamp_i:
                     return False
             return True
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 
 class DateGte(DateCondition):
     """
         Condition for number `what` greater than equals `value`
     """
 
     def _is_satisfied(self) -> bool:
+        timestamp_what = self.convert_timestamp_from_any(self.what)
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
                 timestamp_i = self.convert_timestamp_from_any(i)
                 if not timestamp_i or not timestamp_what:
                     return False
                 if timestamp_what >= timestamp_i:
                     return True
             return False
         else:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
                 timestamp_i = self.convert_timestamp_from_any(i)
                 if not timestamp_i or not timestamp_what:
                     return False
                 if timestamp_what < timestamp_i:
                     return False
             return True
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 
 class DateLt(DateCondition):
     """
         Condition for number `what` less than `value`
     """
 
     def _is_satisfied(self) -> bool:
+        timestamp_what = self.convert_timestamp_from_any(self.what)
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
                 timestamp_i = self.convert_timestamp_from_any(i)
                 if not timestamp_i or not timestamp_what:
                     return False
                 if timestamp_what < timestamp_i:
                     return True
             return False
         else:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
                 timestamp_i = self.convert_timestamp_from_any(i)
                 if not timestamp_i or not timestamp_what:
                     return False
                 if timestamp_what >= timestamp_i:
                     return False
             return True
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 """
-    Numeric less than equal conditions
+    Numeric greater than equal conditions
 """
 
 from marshmallow import post_load
 
-from .base import DateCondition, DateConditionSchema
+from .base import NumericCondition, NumericConditionSchema
 
 
-class DateLte(DateCondition):
+class Gte(NumericCondition):
     """
-        Condition for number `what` less than equals `value`
+        Condition for number `what` greater than equals `value`
     """
 
     def _is_satisfied(self) -> bool:
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
-                timestamp_i = self.convert_timestamp_from_any(i)
-                if not timestamp_i or not timestamp_what:
-                    return False
-                if timestamp_what <= timestamp_i:
+                if self.what >= i:
                     return True
             return False
         else:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
-                timestamp_i = self.convert_timestamp_from_any(i)
-                if not timestamp_i or not timestamp_what:
-                    return False
-                if timestamp_what > timestamp_i:
+                if self.what < i:
                     return False
             return True
 
 
-class DateLteSchema(DateConditionSchema):
+class GteSchema(NumericConditionSchema):
     """
-        JSON schema for less than equals numeric condition
+        JSON schema for greater than equals numeric condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return DateLte(**data)
+        return Gte(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 
 class DateNeq(DateCondition):
     """
         Condition for number `what` not equals `value`
     """
 
     def _is_satisfied(self) -> bool:
+        timestamp_what = self.convert_timestamp_from_any(self.what)
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
                 timestamp_i = self.convert_timestamp_from_any(i)
                 if not timestamp_i or not timestamp_what:
                     return False
                 if timestamp_what != timestamp_i:
                     return True
             return False
         else:
             for i in self.values:
-                timestamp_what = self.convert_timestamp_from_any(self.what)
                 timestamp_i = self.convert_timestamp_from_any(i)
                 if not timestamp_i or not timestamp_what:
                     return False
                 if timestamp_what == timestamp_i:
                     return False
             return True
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/base_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,54 @@
 """
-    String conditions base class
+    Numeric conditions base class
 """
 
 import logging
-import datetime
+
 from marshmallow import Schema, fields, EXCLUDE, validate
 
 from ..base import ConditionBase, ABCMeta, abstractmethod
 
 LOG = logging.getLogger(__name__)
 
 
-class DayCondition(ConditionBase, metaclass=ABCMeta):
+def is_number(value) -> bool:
     """
-        Base class for string conditions
+        Check if value is a number
     """
+    return isinstance(value, (float, int))
+
 
-    class DateFormat:
-        ISO_FORMAT = "%Y-%m-%d"
+class NumericListCondition(ConditionBase, metaclass=ABCMeta):
+    """
+        Base class for numeric conditions
+    """
 
-    def __init__(self, values, what, date_format=DateFormat.ISO_FORMAT, qualifier=ConditionBase.Qualifier.ForAnyValue, **kwargs):
-        self.values = values
-        self.what = what
+    def __init__(self, values, what, qualifier=ConditionBase.Qualifier.ForAnyValue, **kwargs):
+        values_format = [float(i) for i in values]
+        what_format = [float(i) for i in what]
+        self.values = values_format
+        self.what = what_format
         self.qualifier = qualifier
-        self.date_format = date_format
 
 
     @abstractmethod
     def _is_satisfied(self) -> bool:
         """
-            Is string conditions satisfied
+            Is numeric conditions satisfied
 
-            :param what: string value to check
+            :param what: numeric value to check
             :return: True if satisfied else False
         """
         raise NotImplementedError()
 
-    def convert_str_to_date(self, d_str):
-        try:
-            return datetime.datetime.strptime(d_str, self.DateFormat.ISO_FORMAT)
-        except:
-            return None
 
-    def check_format_input_day(self, i):
-        if isinstance(i, str):
-            if self.convert_str_to_date(i):
-                return True
-        return False
-
-
-class DayConditionSchema(Schema):
+class NumericListConditionSchema(Schema):
     """
-        Base JSON schema for string conditions
+        Base JSON schema for numeric conditions
     """
-    values = fields.List(fields.Raw(required=True, allow_none=False), required=True, allow_none=False)
-    what = fields.String(required=True, allow_none=False)
+    values = fields.List(fields.Number(required=True, allow_none=False), required=True, allow_none=False)
+    what = fields.List(fields.Number(required=True, allow_none=False), required=True, allow_none=False)
     qualifier = fields.String(allow_none=False, load_default=ConditionBase.Qualifier.ForAnyValue,
-                            validate=validate.OneOf([ConditionBase.Qualifier.ALL]))
-    date_format = fields.String(allow_none=False, load_default=DayCondition.DateFormat.ISO_FORMAT,)
-
+                              validate=validate.OneOf(ConditionBase.Qualifier.ALL))
     class Meta:
         unknown = EXCLUDE
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 """
-    Date equal conditions
+    Numeric less than equal conditions
 """
 
 from marshmallow import post_load
-from .base import DayCondition, DayConditionSchema
 
+from .base import NumericCondition, NumericConditionSchema
 
-class DayEq(DayCondition):
+
+class Lte(NumericCondition):
+    """
+        Condition for number `what` less than equals `value`
+    """
 
     def _is_satisfied(self) -> bool:
-        if not self.check_format_input_day(self.what):
-            return False
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                if self.check_format_input_day(i):
-                    if self.what == i:
-                        return True
+                if self.what <= i:
+                    return True
             return False
         else:
             for i in self.values:
-                if not self.check_format_input_day(i):
-                    return False
-                if self.what != i:
+                if self.what > i:
                     return False
             return True
 
 
-class DayEqSchema(DayConditionSchema):
+class LteSchema(NumericConditionSchema):
     """
-        JSON schema for equals datetime condition
+        JSON schema for less than equals numeric condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return DayEq(**data)
+        return Lte(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-
 from marshmallow import post_load
 from .base import DayCondition, DayConditionSchema
 
 
-class DayGt(DayCondition):
+class DayLt(DayCondition):
 
     def _is_satisfied(self) -> bool:
-        if not self.check_format_input_day(self.what):
-            return False
+        day_what = self.convert_day_format_from_any(self.what)
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                if self.check_format_input_day(i):
-                    if self.what > i:
-                        return True
+                day_i = self.convert_day_format_from_any(i)
+                if day_what < day_i:
+                    return True
             return False
         else:
             for i in self.values:
-                if not self.check_format_input_day(i):
-                    return False
-                if self.what <= i:
+                day_i = self.convert_day_format_from_any(i)
+                if day_what >= day_i:
                     return False
             return True
 
 
-class DayGtSchema(DayConditionSchema):
+class DayLtSchema(DayConditionSchema):
     """
         JSON schema for greater than datetime condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return DayGt(**data)
+        return DayLt(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,44 @@
+"""
+    String not equals conditions
+"""
+
 from marshmallow import post_load
-from .base import DayCondition, DayConditionSchema
 
+from .base import StringCondition, StringConditionSchema
 
-class DayLt(DayCondition):
+
+class NotEquals(StringCondition):
+    """
+        Condition for string `self.what` not equals `value`
+    """
 
     def _is_satisfied(self) -> bool:
-        if not self.check_format_input_day(self.what):
-            return False
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                if self.check_format_input_day(i):
-                    if self.what < i:
-                        return True
-            return False
+                if self.case_insensitive:
+                    if self.what.lower() == i.lower():
+                        return False
+                else:
+                    if self.what == i:
+                        return False
+            return True
         else:
             for i in self.values:
-                if not self.check_format_input_day(i):
-                    return False
-                if self.what >= i:
-                    return False
+                if self.case_insensitive:
+                    if self.what.lower() == i.lower():
+                        return False
+                else:
+                    if self.what == i:
+                        return False
             return True
 
 
-class DayLtSchema(DayConditionSchema):
+class NotEqualsSchema(StringConditionSchema):
     """
-        JSON schema for greater than datetime condition
+        JSON schema for not equals string condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return DayLt(**data)
+        return NotEquals(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,13 +41,13 @@
         raise NotImplementedError()
 
 
 class NumericConditionSchema(Schema):
     """
         Base JSON schema for numeric conditions
     """
-    values = fields.List(fields.Raw(required=True, allow_none=False), required=True, allow_none=False)
+    values = fields.List(fields.Number(required=True, allow_none=False), required=True, allow_none=False)
     what = fields.Number(required=True, allow_none=False)
     qualifier = fields.String(allow_none=False, load_default=ConditionBase.Qualifier.ForAnyValue,
-                              validate=validate.OneOf([ConditionBase.Qualifier.ALL]))
+                              validate=validate.OneOf(ConditionBase.Qualifier.ALL))
     class Meta:
         unknown = EXCLUDE
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Numeric greater than equal conditions
+    Numeric less than conditions
 """
 
 from marshmallow import post_load
 
 from .base import NumericCondition, NumericConditionSchema
 
 
-class Gte(NumericCondition):
+class Lt(NumericCondition):
     """
-        Condition for number `what` greater than equals `value`
+        Condition for number `what` less than `value`
     """
 
     def _is_satisfied(self) -> bool:
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                if self.what >= i:
+                if self.what < i:
                     return True
             return False
         else:
             for i in self.values:
-                if self.what < i:
+                if self.what >= i:
                     return False
             return True
 
 
-class GteSchema(NumericConditionSchema):
+class LtSchema(NumericConditionSchema):
     """
-        JSON schema for greater than equals numeric condition
+        JSON schema for less than numeric condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return Gte(**data)
+        return Lt(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Numeric less than conditions
+    Numeric not equal conditions
 """
 
 from marshmallow import post_load
 
 from .base import NumericCondition, NumericConditionSchema
 
 
-class Lt(NumericCondition):
+class Neq(NumericCondition):
     """
-        Condition for number `what` less than `value`
+        Condition for number `what` not equals `value`
     """
 
     def _is_satisfied(self) -> bool:
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                if self.what < i:
+                if self.what != i:
                     return True
             return False
         else:
             for i in self.values:
-                if self.what >= i:
+                if self.what == i:
                     return False
             return True
 
 
-class LtSchema(NumericConditionSchema):
+class NeqSchema(NumericConditionSchema):
     """
-        JSON schema for less than numeric condition
+        JSON schema for not equals numeric condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return Lt(**data)
+        return Neq(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 """
-    Numeric less than equal conditions
+    Others conditions base class
 """
 
-from marshmallow import post_load
+import logging
 
-from .base import NumericCondition, NumericConditionSchema
+from marshmallow import Schema, fields, EXCLUDE, validate
 
+from ..base import ConditionBase, ABCMeta, abstractmethod
 
-class Lte(NumericCondition):
+LOG = logging.getLogger(__name__)
+
+
+
+class OthersCondition(ConditionBase, metaclass=ABCMeta):
     """
-        Condition for number `what` less than equals `value`
+        Base class for numeric conditions
     """
 
+    def __init__(self, values, what, **kwargs):
+        self.values = values
+        self.what = what
+
+
+    @abstractmethod
     def _is_satisfied(self) -> bool:
-        if self.qualifier == self.Qualifier.ForAnyValue:
-            for i in self.values:
-                if self.what <= i:
-                    return True
-            return False
-        else:
-            for i in self.values:
-                if self.what > i:
-                    return False
-            return True
+        """
+            Is numeric conditions satisfied
+
+            :param what: numeric value to check
+            :return: True if satisfied else False
+        """
+        raise NotImplementedError()
 
 
-class LteSchema(NumericConditionSchema):
+class OthersConditionSchema(Schema):
     """
-        JSON schema for less than equals numeric condition
+        Base JSON schema for numeric conditions
     """
+    values = fields.Dict(default={}, missing={}, allow_none=False)
+    what = fields.String(required=True, allow_none=False)
 
-    @post_load
-    def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
-        # self.validate(data)
-        return Lte(**data)
+    class Meta:
+        unknown = EXCLUDE
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/list_lte.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """
-    Numeric not equal conditions
+    Numeric greater than conditions
 """
 
 from marshmallow import post_load
 
-from .base import NumericCondition, NumericConditionSchema
+from .base_list import NumericListCondition, NumericListConditionSchema
 
 
-class Neq(NumericCondition):
+class ListLte(NumericListCondition):
     """
-        Condition for number `what` not equals `value`
+        Condition for number `what` greater than `value`
     """
 
     def _is_satisfied(self) -> bool:
         if self.qualifier == self.Qualifier.ForAnyValue:
-            for i in self.values:
-                if self.what != i:
-                    return True
+            for w in self.what:
+                for v in self.values:
+                    if w <= v:
+                        return True
             return False
         else:
-            for i in self.values:
-                if self.what == i:
-                    return False
+            for w in self.what:
+                for v in self.values:
+                    if w > v:
+                        return False
             return True
 
-
-class NeqSchema(NumericConditionSchema):
+class ListLteSchema(NumericListConditionSchema):
     """
-        JSON schema for not equals numeric condition
+        JSON schema for greater than numeric condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return Neq(**data)
+        return ListLte(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class Exists(OthersCondition):
     """
         Condition for attribute value exists
     """
 
-    def is_satisfied(self) -> bool:
+    def _is_satisfied(self) -> bool:
         if self.values.get(self.what) or self.values.get(self.what) in [0, False]:
             return True
         else:
             return False
 
 
 class ExistsSchema(OthersConditionSchema):
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class NotExists(OthersCondition):
     """
         Condition for attribute value not exists
     """
 
-    def is_satisfied(self) -> bool:
+    def _is_satisfied(self) -> bool:
         if self.values.get(self.what) or self.values.get(self.what) in [0, False]:
             return False
         else:
             return True
 
 
 class NotExistsSchema(OthersConditionSchema):
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -31,14 +31,19 @@
         "NumericEquals": EqSchema,
         "NumericNotEquals": NeqSchema,
         "NumericLessThan": LtSchema,
         "NumericLessThanEquals": LteSchema,
         "NumericGreaterThan": GtSchema,
         "NumericGreaterThanEquals": GteSchema,
 
+        "NumericListLessThan": ListLtSchema,
+        "NumericListLessThanEquals": ListLteSchema,
+        "NumericListGreaterThan": ListGtSchema,
+        "NumericListGreaterThanEquals": ListGteSchema,
+
         "DateEquals": DateEqSchema,
         "DateNotEquals": DateNeqSchema,
         "DateLessThan": DateLtSchema,
         "DateLessThanEquals": DateLteSchema,
         "DateGreaterThan": DateGtSchema,
         "DateGreaterThanEquals": DateGteSchema,
 
@@ -51,14 +56,16 @@
         "ListAllNotIn": AllNotInSchema,
         "ListAnyIn": AnyInSchema,
         "ListAnyNotIn": AnyNotInSchema,
         "ListIsEmpty": IsEmptySchema,
         "ListIsIn": IsInSchema,
         "ListIsNotEmpty": IsNotEmptySchema,
         "ListIsNotIn": IsNotInSchema,
+        "ListAnyContains": AnyContainsSchema,
+        "ListAnyNotContains": AnyNotContainsSchema,
 
         "DayEquals": DayEqSchema,
         "DayNotEquals": DayNeqSchema,
         "DayLessThan": DayLtSchema,
         "DayLessThanEquals": DayLteSchema,
         "DayGreaterThan": DayGtSchema,
         "DayGreaterThanEquals": DayGteSchema,
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 
 
 class StringCondition(ConditionBase, metaclass=ABCMeta):
     """
         Base class for string conditions
     """
 
-    def __init__(self, values, what, qualifier=ConditionBase.Qualifier.ForAnyValue, ignore_case=False, **kwargs):
+    def __init__(self, values, what, qualifier=ConditionBase.Qualifier.ForAnyValue, ignore_case=False,
+                 delimiter="", **kwargs):
         self.case_insensitive = ignore_case
         self.values = values
         self.what = what
         self.qualifier = qualifier
+        self.delimiter = delimiter
 
 
     @abstractmethod
     def _is_satisfied(self) -> bool:
         """
             Is string conditions satisfied
 
@@ -46,10 +48,11 @@
         Base JSON schema for string conditions
     """
     values = fields.List(fields.String(required=True, allow_none=False), required=True, allow_none=False)
     ignore_case = fields.Bool(default=False, missing=False)
     what = fields.String(required=True, allow_none=False)
     qualifier = fields.String(allow_none=False, load_default=ConditionBase.Qualifier.ForAnyValue,
                             validate=validate.OneOf(ConditionBase.Qualifier.ALL))
+    delimiter = fields.String(required=False, default="", missing="")
 
     class Meta:
         unknown = EXCLUDE
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """
-    String contains conditions
+    String equals conditions
 """
 
-from marshmallow import post_load
+from marshmallow import post_load, EXCLUDE
 
 from .base import StringCondition, StringConditionSchema
 
 
-class Contains(StringCondition):
+class Equals(StringCondition):
     """
-        Condition for string `self.what` contains `value`
+        Condition for string `self.what` equals `value`
     """
 
     def _is_satisfied(self) -> bool:
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
                 if self.case_insensitive:
-                    if self.what.lower() in i.lower():
+                    if self.what.lower() == i.lower():
                         return True
                 else:
-                    if self.what in i:
+                    if self.what == i:
                         return True
             return False
         else:
             for i in self.values:
                 if self.case_insensitive:
-                    if self.what.lower() not in i.lower():
+                    if self.what.lower() != i.lower():
                         return False
                 else:
-                    if self.what not in i:
+                    if self.what != i:
                         return False
             return True
 
-class ContainsSchema(StringConditionSchema):
+
+class EqualsSchema(StringConditionSchema):
     """
-        JSON schema for contains string conditions
+        JSON schema for equals string condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return Contains(**data)
+        return Equals(**data)
+
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/numeric/list_lt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 """
-    String ends with conditions
+    Numeric greater than conditions
 """
 
 from marshmallow import post_load
 
-from .base import StringCondition, StringConditionSchema
+from .base_list import NumericListCondition, NumericListConditionSchema
 
 
-class EndsWith(StringCondition):
+class ListLt(NumericListCondition):
     """
-        Condition for string `self.what` ends with `value`
+        Condition for number `what` greater than `value`
     """
 
-    def _is_satisfied(self,) -> bool:
+    def _is_satisfied(self) -> bool:
         if self.qualifier == self.Qualifier.ForAnyValue:
-            for i in self.values:
-                if self.case_insensitive:
-                    if self.what.lower().endswith(i.lower()):
-                        return True
-                else:
-                    if self.what.endswith(i):
+            for w in self.what:
+                for v in self.values:
+                    if w < v:
                         return True
             return False
         else:
-            for i in self.values:
-                if self.case_insensitive:
-                    if not self.what.lower().endswith(i.lower()):
-                        return False
-                else:
-                    if not self.what.endswith(i):
+            for w in self.what:
+                for v in self.values:
+                    if w >= v:
                         return False
             return True
 
-
-class EndsWithSchema(StringConditionSchema):
+class ListLtSchema(NumericListConditionSchema):
     """
-        JSON schema for ends with string condition
+        JSON schema for greater than numeric condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return EndsWith(**data)
+        return ListLt(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/not_ends_with.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 """
-    String not ends with conditions
+    String starts with conditions
 """
 
 from marshmallow import post_load
 
 from .base import StringCondition, StringConditionSchema
 
 
-class NotEndsWith(StringCondition):
+class StartsWith(StringCondition):
     """
-        Condition for string `self.what` ends with `value`
+        Condition for string `self.what` starts with `value`
     """
 
-    def _is_satisfied(self,) -> bool:
+    def _is_satisfied(self) -> bool:
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
                 if self.case_insensitive:
-                    if not self.what.lower().endswith(i.lower()):
-                        return True
+                    if self.delimiter:
+                        if self.what.lower().startswith(i.lower() + self.delimiter) or i.lower() == self.what.lower():
+                            return True
+                    else:
+                        if self.what.lower().startswith(i.lower()):
+                            return True
                 else:
-                    if not self.what.endswith(i):
-                        return True
+                    if self.delimiter:
+                        if self.what.startswith(i + self.delimiter) or i == self.what:
+                            return True
+                    else:
+                        if self.what.startswith(i):
+                            return True
             return False
         else:
             for i in self.values:
                 if self.case_insensitive:
-                    if self.what.lower().endswith(i.lower()):
-                        return False
+                    if self.delimiter:
+                        if self.what.lower().startswith(i.lower() + self.delimiter) or i.lower() == self.what.lower():
+                            pass
+                        else:
+                            return False
+                    else:
+                        if not self.what.lower().startswith(i.lower()):
+                            return False
                 else:
-                    if self.what.endswith(i):
-                        return False
+                    if self.delimiter:
+                        if self.what.startswith(i + self.delimiter) or i == self.what:
+                            pass
+                        else:
+                            return False
+                    else:
+                        if not self.what.startswith(i):
+                            return False
             return True
 
 
-class NotEndsWithSchema(StringConditionSchema):
+class StartsWithSchema(StringConditionSchema):
     """
-        JSON schema for ends with string condition
+        JSON schema for starts with string condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return NotEndsWith(**data)
+        return StartsWith(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/not_starts_with.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/not_starts_with.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,28 +12,44 @@
         Condition for string `self.what` starts with `value`
     """
 
     def _is_satisfied(self) -> bool:
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
                 if self.case_insensitive:
-                    if not self.what.lower().startswith(i.lower()):
-                        return True
+                    if self.delimiter:
+                        if self.what.lower().startswith(i.lower() + self.delimiter) or i.lower() == self.what.lower():
+                            return False
+                    else:
+                        if self.what.lower().startswith(i.lower()):
+                            return False
                 else:
-                    if not self.what.startswith(i):
-                        return True
-            return False
+                    if self.delimiter:
+                        if self.what.startswith(i + self.delimiter) or i == self.what:
+                            return False
+                    else:
+                        if self.what.startswith(i):
+                            return False
+            return True
         else:
             for i in self.values:
                 if self.case_insensitive:
-                    if self.what.lower().startswith(i.lower()):
-                        return False
+                    if self.delimiter:
+                        if self.what.lower().startswith(i.lower() + self.delimiter) or i.lower() == self.what.lower():
+                            return False
+                    else:
+                        if self.what.lower().startswith(i.lower()):
+                            return False
                 else:
-                    if self.what.startswith(i):
-                        return False
+                    if self.delimiter:
+                        if self.what.startswith(i + self.delimiter) or i == self.what:
+                            return False
+                    else:
+                        if self.what.startswith(i):
+                            return False
             return True
 
 
 class NotStartsWithSchema(StringConditionSchema):
     """
         JSON schema for starts with string condition
     """
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 """
-    String starts with conditions
+    Numeric less than equal conditions
 """
 
 from marshmallow import post_load
 
-from .base import StringCondition, StringConditionSchema
+from .base import DateCondition, DateConditionSchema
 
 
-class StartsWith(StringCondition):
+class DateLte(DateCondition):
     """
-        Condition for string `self.what` starts with `value`
+        Condition for number `what` less than equals `value`
     """
 
     def _is_satisfied(self) -> bool:
+        timestamp_what = self.convert_timestamp_from_any(self.what)
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
-                if self.case_insensitive:
-                    if self.what.lower().startswith(i.lower()):
-                        return True
-                else:
-                    if self.what.startswith(i):
-                        return True
+                timestamp_i = self.convert_timestamp_from_any(i)
+                if not timestamp_i or not timestamp_what:
+                    return False
+                if timestamp_what <= timestamp_i:
+                    return True
             return False
         else:
             for i in self.values:
-                if self.case_insensitive:
-                    if not self.what.lower().startswith(i.lower()):
-                        return False
-                else:
-                    if not self.what.startswith(i):
-                        return False
+                timestamp_i = self.convert_timestamp_from_any(i)
+                if not timestamp_i or not timestamp_what:
+                    return False
+                if timestamp_what > timestamp_i:
+                    return False
             return True
 
 
-class StartsWithSchema(StringConditionSchema):
+class DateLteSchema(DateConditionSchema):
     """
-        JSON schema for starts with string condition
+        JSON schema for less than equals numeric condition
     """
 
     @post_load
     def post_load(self, data, **_):  # pylint: disable=missing-docstring,no-self-use
         # self.validate(data)
-        return StartsWith(**data)
+        return DateLte(**data)
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/exceptions.py` & `m-abac-1.0.2/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/policy.py` & `m-abac-1.0.2/mobio/libs/abac/policy/policy.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,51 +4,58 @@
 import json
 from marshmallow import Schema, fields, post_load, ValidationError, validate, EXCLUDE
 from .conditions.schema import ConditionSchema
 from .utils import Utils
 from .conditions.base import ConditionBase
 from .exceptions import *
 
+
 class AccessType:
     DENY_ACCESS = "deny"
     ALLOW_ACCESS = "allow"
 
+
 class Policy(object):
     """
         Policy class containing rules and targets
     """
 
     def __init__(
             self,
             effect: str,
-            action: list,
-            resource: list,
+            # action: list,
+            # resource: list,
             condition: dict,
             request_access: dict, **kwargs
     ):
         self.effect = effect
-        self.action = action
-        self.resource = resource
+        # self.action = action
+        # self.resource = resource
         self.condition = condition
+        self.condition_convert = None
         self.request_access = request_access
 
     def is_allowed(self):
         conditions = self.convert_condition()
+        self.condition_convert = conditions
         for condition in conditions:
-            # print("condition: ", condition)
+            # print("abac_sdk condition: ", condition)
             if condition.get("operator") == "Null":
                 what_check = self.get_value_from_field(condition.get("field"))
                 if what_check is not None:
                     return False
             else:
                 cond_schema = ConditionSchema().load(condition)
                 if not cond_schema._is_satisfied():
                     return False
         return True
 
+    def get_condition_convert(self):
+        return self.condition_convert
+
     def convert_condition(self):
         """
             {
                 "operator": "StringEquals",
                 "field": "user:staff_code",
                 "values": ["A123456"],
                 "qualifier": "ForAnyValue",
@@ -57,51 +64,71 @@
             }
         :return:
         """
         list_condition = []
         have_condition_exclude = False
         for item in self.condition:
             cond_schema = self.validate_item_condition(item)
-            # print("cond_schema: {}".format(json.dumps(cond_schema)))
+            # print("abac_sdk cond_schema: {}".format(json.dumps(cond_schema)))
             if cond_schema.get("operator") == "Null":
                 list_condition.append({**item})
+            elif cond_schema.get("operator") in ["Exists", "NotExists"]:
+                resource_name, resource_key = Utils.split_delemiter_resource(cond_schema.get("field"))
+                data_resource = {}
+                if resource_name:
+                    if self.request_access.get(resource_name) and isinstance(self.request_access.get(resource_name),
+                                                                             dict):
+                        data_resource = self.request_access.get(resource_name)
+                list_condition.append({
+                    **item,
+                    "values": data_resource,
+                    "what": resource_key,
+                })
             else:
                 if_exists = cond_schema.get("if_exists")
                 what_check = self.get_value_from_field(cond_schema.get("field"))
                 if what_check is None:
                     if if_exists:
                         have_condition_exclude = True
                         continue
                     raise GetValueNoneException("{} get value is None".format(cond_schema.get("field")))
                 values = []
                 for v in cond_schema.get("values"):
-                    values.append(self.get_value_from_variable(v))
+                    value_from_variable = self.get_value_from_variable(v)
+                    if isinstance(value_from_variable, list):
+                        values.extend(value_from_variable)
+                    else:
+                        values.append(value_from_variable)
                 list_condition.append({
                     **item,
                     "values": values,
                     "what": what_check,
                 })
         # if len(list_condition) == 0 and not have_condition_exclude:
         #     raise EmptyConditionException("no condition found")
         return list_condition
 
     def get_value_from_variable(self, str_variable):
-        variables = Utils.get_field_key_from_variable(str_variable)
-        if variables:
-            if len(variables) == 1 and Utils.check_field_is_variable(variables[0]):
-                field_value = self.get_value_from_field(variables[0])
-                if field_value is None:
-                    raise GetValueNoneException("{} get value is None".format(variables[0]))
-                return field_value
-            for field_key in variables:
-                field_value = self.get_value_from_field(field_key)
-                if field_value is None:
-                    raise GetValueNoneException("{} get value is None".format(field_key))
-                field_value = str(field_value)
-                str_variable = Utils.replace_variable_to_value(field_key, field_value, str_variable)
+        if isinstance(str_variable, str) and Utils.check_field_is_variable(str_variable):
+            variables = Utils.get_field_key_from_variable(str_variable)
+            if variables:
+                if len(variables) == 1:
+                    field_value = self.get_value_from_field(variables[0])
+                    if field_value is None:
+                        raise GetValueNoneException("{} get value is None".format(variables[0]))
+                    if isinstance(field_value, str):
+                        field_value_format = Utils.replace_variable_to_value(variables[0], field_value, str_variable)
+                        return field_value_format
+                    return field_value
+                for field_key in variables:
+                    field_value = self.get_value_from_field(field_key)
+                    if field_value is None:
+                        raise GetValueNoneException("{} get value is None".format(field_key))
+                    field_value = str(field_value)
+                    str_variable = Utils.replace_variable_to_value(field_key, field_value, str_variable)
         return str_variable
 
     def get_value_from_field(self, field_key):
         resource_name, resource_key = Utils.split_delemiter_resource(field_key)
         if resource_name and resource_key:
             if self.request_access.get(resource_name) and isinstance(self.request_access.get(resource_name), dict):
                 data_resource = self.request_access.get(resource_name)
@@ -111,33 +138,35 @@
 
     def validate_item_condition(self, obj):
         try:
             return ConditionValidateSchema().load(obj)
         except Exception as err:
             raise InvalidConditionException("validate_item_condition: {}".format(err))
 
+
 class ConditionValidateSchema(Schema):
     operator = fields.String(required=True, allow_none=False)
     field = fields.String(required=True, allow_none=False)
     values = fields.List(fields.Raw(required=True, allow_none=False), required=True, allow_none=False)
-    qualifier = fields.String(default=ConditionBase.Qualifier.ForAnyValue,  validate=validate.OneOf(ConditionBase.Qualifier.ALL))
+    qualifier = fields.String(default=ConditionBase.Qualifier.ForAnyValue,
+                              validate=validate.OneOf(ConditionBase.Qualifier.ALL))
     if_exists = fields.Boolean(default=False)
     ignore_case = fields.Boolean(default=False)
 
     class Meta:
         unknown = EXCLUDE
 
 
 class PolicySchema(Schema):
     """
         JSON schema for policy
     """
     effect = fields.String(required=True, validate=validate.OneOf([AccessType.DENY_ACCESS, AccessType.ALLOW_ACCESS]))
-    action = fields.List(fields.String(required=True, allow_none=False),required=True, allow_none=False)
-    resource = fields.List(fields.String(required=True, allow_none=False),required=True, allow_none=False)
+    # action = fields.List(fields.String(required=True, allow_none=False),required=True, allow_none=False)
+    # resource = fields.List(fields.String(required=True, allow_none=False),required=True, allow_none=False)
     condition = fields.List(fields.Raw(required=True, allow_none=False), required=True, allow_none=False)
     request_access = fields.Dict(default={}, missing={}, allow_none=False)
 
     class Meta:
         unknown = EXCLUDE
 
     @post_load
```

### Comparing `m-abac-1.0.1/mobio/libs/abac/policy/utils.py` & `m-abac-1.0.2/mobio/libs/abac/policy/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from datetime import datetime
 from user_agents import parse
 from flask import request
 import base64
 
 
 class Utils:
+    ISO_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
+
+    @classmethod
+    def convert_string_to_format(cls, date_str, date_format):
+        try:
+            return datetime.strptime(date_str, cls.ISO_FORMAT).strftime(date_format)
+        except:
+            return date_str
 
     @staticmethod
     def split_delemiter_resource(str_value):
         resource_name, resource_key = None, None
         if ":" in str_value:
             values = str_value.split(":")
             resource_name, resource_key = values[0], values[1]
@@ -36,25 +44,28 @@
     def get_field_key_from_variable(str_text) -> list:
         key_regex = "\${(.*?)}"
         try:
             if isinstance(str_text, int):
                 return []
             return re.findall(key_regex, str_text)
         except Exception as er:
-            print("get_field_key_from_variable key: {}, err: {}".format(key_regex, er))
+            print("abac_sdk get_field_key_from_variable key: {}, err: {}".format(key_regex, er))
             return []
 
     @staticmethod
     def replace_variable_to_value(field_key, field_value, str_origin):
         key_regex = "\${" + field_key + "}"
         return re.sub(fr'{key_regex}', field_value, str_origin)
 
     @staticmethod
     def check_field_is_variable(field_key):
-        if field_key.startswith("${") and field_key.endswith("}"):
+        # if field_key.startswith("${") and field_key.endswith("}"):
+        #     return True
+        # return False
+        if Utils.get_field_key_from_variable(field_key):
             return True
         return False
 
     @staticmethod
     def get_date_utcnow():
         return datetime.utcnow()
 
@@ -79,19 +90,19 @@
     def get_info_from_header_request():
         try:
             header_data = request.headers
             user_agent = header_data.get('User-Agent')
             current_ip = request.remote_addr
             if header_data.get("X-Real-Ip"):
                 current_ip = header_data.get("X-Real-Ip")
-            device_type = header_data.get('x-device-type')
+            device_type = header_data.get('mobio-device-type')
             return {
-                "env:source_ip": current_ip,
-                "env:user_agent": user_agent,
-                "env:device_type": device_type if device_type else "web"
+                "source_ip": current_ip,
+                "user_agent": user_agent,
+                "device_type": device_type if device_type else "web"
             }
         except:
             return {}
 
     @staticmethod
     def get_fields_of_resource(full_resource):
         fields = {}
@@ -107,14 +118,37 @@
         if list_field and body_request:
             for field in list_field:
                 if field in body_request:
                     return True
         return False
 
     @staticmethod
+    def add_field_in_body_request(list_field, body_request):
+        if list_field and body_request:
+            for field in list_field:
+                # if isinstance(body_request.get(field), bool) or isinstance(body_request.get(field), int) \
+                #         or isinstance(body_request.get(field), float):
+                #     return True
+                # if not body_request.get(field):
+                #     continue
+                # return True
+                if Utils.check_value_valid_check_action_add(body_request.get(field)):
+                    return True
+        return False
+
+    @staticmethod
+    def check_value_valid_check_action_add(value_check):
+        if isinstance(value_check, bool) or isinstance(value_check, int) \
+                or isinstance(value_check, float):
+            return True
+        if not value_check:
+            return False
+        return True
+
+    @staticmethod
     def base64_encode(data):
         try:
             byte_string = data.encode('utf-8')
             encoded_data = base64.b64encode(byte_string)
             return encoded_data.decode(encoding='UTF-8')
         except:
             return ""
```

### Comparing `m-abac-1.0.1/setup.py` & `m-abac-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,23 +38,24 @@
             "marshmallow-oneofschema",
             "ipaddress",
             "objectpath",
             "redis",
             "m-caching",
             "user-agents",
             "Flask",
+            "m-kafka-sdk-v2",
         ]
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
-version_dev='1.0.1'
-version_prod='1.0.1'
+version_dev='1.0.32'
+version_prod='1.0.2'
 
 run_mode=''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -70,15 +71,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.1',  # Required
+    version='1.0.2',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

