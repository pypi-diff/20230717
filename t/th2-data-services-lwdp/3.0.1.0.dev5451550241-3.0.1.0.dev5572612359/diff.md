# Comparing `tmp/th2_data_services_lwdp-3.0.1.0.dev5451550241.tar.gz` & `tmp/th2_data_services_lwdp-3.0.1.0.dev5572612359.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-3.0.1.0.dev5451550241.tar", last modified: Tue Jul  4 06:33:38 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-3.0.1.0.dev5572612359.tar", last modified: Mon Jul 17 06:49:29 2023, max compression
```

## Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241.tar` & `th2_data_services_lwdp-3.0.1.0.dev5572612359.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9661 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7683 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-04 06:33:25.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      651 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    61689 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14524 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     4354 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9661 2023-07-04 06:33:37.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 06:33:37.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-04 06:33:37.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-04 06:33:37.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9661 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7683 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-17 06:49:16.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    62500 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14524 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4354 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-17 06:48:22.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9661 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-17 06:49:29.000000 th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/PKG-INFO` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2_data_services_lwdp
-Version: 3.0.1.0.dev5451550241
+Name: th2-data-services-lwdp
+Version: 3.0.1.0.dev5572612359
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/README.md` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/setup.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from abc import abstractmethod
 from typing import List, Optional, Union, Generator, Any
 from datetime import datetime
 from functools import partial
 from shutil import copyfileobj
+from deprecated.classic import deprecated
 
 from th2_data_services.data import Data
 from th2_data_services.exceptions import EventNotFound, MessageNotFound
 from th2_data_services.utils.converters import DatetimeConverter, ProtobufTimestampConverter
 
 from th2_data_services.data_source.lwdp import Page
 from th2_data_services.data_source.lwdp.interfaces.command import IHTTPCommand
@@ -947,14 +948,20 @@
                 response_formats=self._response_formats,
             ).handle(data_source)
             result.append(message)
 
         return result
 
 
+@deprecated(
+    """This is depricated command because LwDP3 was developed for th2-transport (intead of protobuf transport). 
+To speed up the whole chain, all messages are stored in DB by groups but not by session alias.
+It means that you'll get nothing by your alias, because the data in DB is in another table (for groups).
+Use the commands that get messages by Groups instead."""
+)
 class GetMessagesByBookByStreams(SSEHandlerClassBase):
     """A Class-Command for request to lw-data-provider.
 
     It searches messages stream by options.
 
     Returns:
         Iterable[dict]: Stream of Th2 messages.
@@ -1481,15 +1488,20 @@
                 char_enc=self._char_enc,
                 decode_error_handler=self._decode_error_handler,
                 cache=self._cache,
                 buffer_limit=self._buffer_limit,
             )
         )
 
-
+@deprecated(
+    """This is depricated command because LwDP3 was developed for th2-transport (intead of protobuf transport). 
+To speed up the whole chain, all messages are stored in DB by groups but not by session alias.
+It means that you'll get nothing by your alias, because the data in DB is in another table (for groups).
+Use the commands that get messages by Groups instead."""
+)
 class GetMessagesByPageByStreams(SSEHandlerClassBase):
     def __init__(
         self,
         page: Union[Page, str],
         stream: List[str],
         book_id: str = None,
         message_ids: List[None] = None,
```

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/_misc.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2-data-services-lwdp
-Version: 3.0.1.0.dev5451550241
+Name: th2_data_services_lwdp
+Version: 3.0.1.0.dev5572612359
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-3.0.1.0.dev5572612359/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

