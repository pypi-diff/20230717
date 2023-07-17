# Comparing `tmp/rdt_identity-1.6.0.dev0.tar.gz` & `tmp/rdt_identity-1.6.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt_identity-1.6.0.dev0.tar", last modified: Wed Jul 12 17:39:54 2023, max compression
+gzip compressed data, was "rdt_identity-1.6.1.dev0.tar", last modified: Mon Jul 17 20:29:39 2023, max compression
```

## Comparing `rdt_identity-1.6.0.dev0.tar` & `rdt_identity-1.6.1.dev0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.145932 rdt_identity-1.6.0.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    44576 2023-07-12 17:38:30.000000 rdt_identity-1.6.0.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7964 2023-07-12 17:39:54.146032 rdt_identity-1.6.0.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.133123 rdt_identity-1.6.0.dev0/rdt/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.133190 rdt_identity-1.6.0.dev0/rdt/transformers/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.133258 rdt_identity-1.6.0.dev0/rdt/transformers/addons/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.137372 rdt_identity-1.6.0.dev0/rdt/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/rdt/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/rdt/transformers/addons/identity/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-07-12 17:39:54.146575 rdt_identity-1.6.0.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4134 2023-07-12 17:39:40.000000 rdt_identity-1.6.0.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.138097 rdt_identity-1.6.0.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.133564 rdt_identity-1.6.0.dev0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.139350 rdt_identity-1.6.0.dev0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.139920 rdt_identity-1.6.0.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.141343 rdt_identity-1.6.0.dev0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.141668 rdt_identity-1.6.0.dev0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7106 2023-07-12 17:38:36.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-06-28 22:45:00.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-05 23:04:49.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-06-28 22:45:00.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.142190 rdt_identity-1.6.0.dev0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.6.0.dev0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.142516 rdt_identity-1.6.0.dev0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.6.0.dev0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.142983 rdt_identity-1.6.0.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-06-20 18:01:47.000000 rdt_identity-1.6.0.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.144869 rdt_identity-1.6.0.dev0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.145022 rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.145337 rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.145795 rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29367 2023-07-12 17:38:36.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-05 23:04:49.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-06-28 22:45:00.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.566109 rdt_identity-1.6.1.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.6.1.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt_identity-1.6.1.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    46119 2023-07-12 20:34:31.000000 rdt_identity-1.6.1.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.6.1.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7964 2023-07-17 20:29:39.566212 rdt_identity-1.6.1.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.6.1.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.553487 rdt_identity-1.6.1.dev0/rdt/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.553573 rdt_identity-1.6.1.dev0/rdt/transformers/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.553646 rdt_identity-1.6.1.dev0/rdt/transformers/addons/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.557590 rdt_identity-1.6.1.dev0/rdt/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/rdt/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.6.1.dev0/rdt/transformers/addons/identity/identity.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-07-17 20:29:39.566759 rdt_identity-1.6.1.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4134 2023-07-12 20:34:53.000000 rdt_identity-1.6.1.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.558028 rdt_identity-1.6.1.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.6.1.dev0/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt_identity-1.6.1.dev0/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.554018 rdt_identity-1.6.1.dev0/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.559059 rdt_identity-1.6.1.dev0/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.559732 rdt_identity-1.6.1.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    45910 2023-07-17 20:29:05.000000 rdt_identity-1.6.1.dev0/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt_identity-1.6.1.dev0/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.560943 rdt_identity-1.6.1.dev0/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.561432 rdt_identity-1.6.1.dev0/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7106 2023-07-12 20:34:31.000000 rdt_identity-1.6.1.dev0/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.6.1.dev0/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-07-12 20:34:31.000000 rdt_identity-1.6.1.dev0/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.6.1.dev0/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-12 20:34:31.000000 rdt_identity-1.6.1.dev0/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-07-12 20:34:31.000000 rdt_identity-1.6.1.dev0/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.6.1.dev0/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.562057 rdt_identity-1.6.1.dev0/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.6.1.dev0/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.562419 rdt_identity-1.6.1.dev0/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.6.1.dev0/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.563004 rdt_identity-1.6.1.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-07-12 20:34:31.000000 rdt_identity-1.6.1.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   104228 2023-07-17 20:29:05.000000 rdt_identity-1.6.1.dev0/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.564881 rdt_identity-1.6.1.dev0/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.565057 rdt_identity-1.6.1.dev0/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.565381 rdt_identity-1.6.1.dev0/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:39.565937 rdt_identity-1.6.1.dev0/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29367 2023-07-12 20:34:31.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3221 2023-07-17 20:29:05.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-12 20:34:31.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-07-12 20:34:31.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.6.1.dev0/tests/unit/transformers/test_utils.py
```

### Comparing `rdt_identity-1.6.0.dev0/CONTRIBUTING.rst` & `rdt_identity-1.6.1.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/HISTORY.md` & `rdt_identity-1.6.1.dev0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,33 @@
 # History
 
+## 1.6.0 -2023-07-12
+
+This release adds the ability to generate missing values to the `AnonymizedFaker`. Users can now provide the `missing_value_generation` parameter during initialization. They can set it to `None` to not generate any missing values, or `'random'` to generate random missing values in the same proportion as the fitted data.
+
+Additionally, this release improves the `NullTransformer` by allowing nulls to be replaced on the forward transform even if `missing_value_generation` is set to None. It also fixes a bug that was causing the `UnixTimestampEncoder` to return a different dtype than the input on `reverse_transform`. This was particularly problematic when datetime columns are represented as ints.
+
+### New Features
+
+* AnonymizedFaker should be able to model and generate missing values - Issue [#660](https://github.com/sdv-dev/RDT/issues/660) by @R-Palazzo
+
+### Bugs
+
+* The datetime transformers don't give me back the same dtype sometimes - Issue [#657](https://github.com/sdv-dev/RDT/issues/657) by @frances-h
+* RDT NullTransformer doesn't replace nulls if missing_value_generation is None - Issue [#658](https://github.com/sdv-dev/RDT/issues/658) by @amontanez24
+
+### Maintenance
+
+* Remove python 3.7 builds - Issue [#663](https://github.com/sdv-dev/RDT/issues/663) by @amontanez24
+* Drop support for Python 3.7 - Issue [#666](https://github.com/sdv-dev/RDT/issues/666) by @amontanez24
+
+### Internal
+
+* Add add-on modules to sys.modules - Issue [#653](https://github.com/sdv-dev/RDT/issues/653) by @amontanez24
+
 ## 1.5.0 - 2023-06-01
 
 This release adds a new parameter called `missing_value_generation` to the initialization of certain transformers to specify how missing values should be created. The parameter can be used in the `FloatFormatter`, `BinaryEncoder`, `UnixTimestampEncoder`, `OptimizedTimestampEncoder`, `GaussianNormalizer` and `ClusterBasedNormalizer`. Additionally, it fixes a bug that was causing every column that had nulls to generate them in the same place.
 
 ### Deprecations
 
 * The `model_missing_values` parameter is being deprecated in favor of the new `missing_value_generation` parameter.
```

### Comparing `rdt_identity-1.6.0.dev0/LICENSE` & `rdt_identity-1.6.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/PKG-INFO` & `rdt_identity-1.6.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt_identity
-Version: 1.6.0.dev0
+Version: 1.6.1.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt,rdt_identity
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt_identity Version: 1.6.0.dev0 Summary:
+Metadata-Version: 2.1 Name: rdt_identity Version: 1.6.1.dev0 Summary:
 Reversible Data Transforms Home-page: https://github.com/sdv-dev/RDT Author:
 DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords:
 rdt,rdt_identity Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `rdt_identity-1.6.0.dev0/README.md` & `rdt_identity-1.6.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/RELEASE.md` & `rdt_identity-1.6.1.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/rdt/transformers/addons/identity/identity.py` & `rdt_identity-1.6.1.dev0/rdt/transformers/addons/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/setup.cfg` & `rdt_identity-1.6.1.dev0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.6.0.dev0
+current_version = 1.6.1.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt_identity-1.6.0.dev0/setup.py` & `rdt_identity-1.6.1.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,10 +135,10 @@
         exclude=['rdt.transformers.addons.*']
     ),
     python_requires='>=3.8,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/RDT',
-    version='1.6.0.dev0',
+    version='1.6.1.dev0',
     zip_safe=False,
 )
```

### Comparing `rdt_identity-1.6.0.dev0/tests/__init__.py` & `rdt_identity-1.6.1.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/code_style.py` & `rdt_identity-1.6.1.dev0/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/contributing.py` & `rdt_identity-1.6.1.dev0/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_boolean.py` & `rdt_identity-1.6.1.dev0/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_categorical.py` & `rdt_identity-1.6.1.dev0/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_datetime.py` & `rdt_identity-1.6.1.dev0/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_numerical.py` & `rdt_identity-1.6.1.dev0/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_utils.py` & `rdt_identity-1.6.1.dev0/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/integration/test_hyper_transformer.py` & `rdt_identity-1.6.1.dev0/tests/integration/test_hyper_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,24 +88,33 @@
         1.264982e+18,
         1.262304e+18,
         1.262304e+18
     ]
     return pd.DataFrame({
         'integer': [1., 2., 1., 3., 1., 4., 2., 3.],
         'float': [0.1, 0.2, 0.1, 0.2, 0.1, 0.4, 0.2, 0.3],
-        'categorical': [0.3125, 0.3125, .8125, 0.8125, 0.3125, 0.8125, 0.3125, 0.3125],
-        'bool': [0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 1.0, 0.0],
+        'categorical': [
+            0.9690758764963199, 0.8816575994729887, 1.1326495454234662, 1.7988488918189502,
+            0.9265972159030215, 1.885454600378942, 0.9280858691537548, 0.5093227924068265
+        ],
+        'bool': [
+            0.26161253184788935, 0.5735484647493089, 0.026673806296574787, 1.197229599974477,
+            0.8860641570557322, 0.33432787358513416, 1.1089412122841389, 0.6182653878449814
+        ],
         'datetime': datetimes,
-        'names': [0.3125, 0.75, 0.75, 0.3125, 0.3125, 0.9375, 0.3125, 0.3125]
+        'names': [
+            0.24180193241041126, 1.9297787196579723, 1.5617500744772101, 0.6811042561384157,
+            0.48017218468846856, 2.2867787591284823, 0.25476586891248476, 0.620052082101593
+        ]
     }, index=TEST_DATA_INDEX)
 
 
 def get_reversed_data():
     data = get_input_data()
-    data['bool'] = data['bool'].astype('object')
+
     return data
 
 
 def test_hypertransformer_default_inputs():
     """Test the HyperTransformer with default parameters.
 
     This tests that if default parameters are provided to the HyperTransformer,
@@ -157,18 +166,27 @@
         1.264982e+18,
         1.262304e+18,
         1.262304e+18
     ]
     expected_transformed = pd.DataFrame({
         'integer': [1., 2., 1., 3., 1., 4., 2., 3.],
         'float': [0.1, 0.2, 0.1, 0.2, 0.1, 0.4, 0.2, 0.3],
-        'categorical': [0.3125, 0.3125, 0.9375, 0.75, 0.3125, 0.75, 0.3125, 0.3125],
-        'bool': [0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 1.0, 0.0],
+        'categorical': [
+            0.9690758764963199, 0.8816575994729887, 1.1326495454234662, 2.7988488918189502,
+            0.9265972159030215, 2.8854546003789423, 0.9280858691537548, 0.5093227924068265
+        ],
+        'bool': [
+            0.26161253184788935, 1.573548464749309, 0.026673806296574787, 2.1972295999744773,
+            0.8860641570557322, 1.334327873585134, 2.108941212284139, 0.6182653878449814
+        ],
         'datetime': expected_datetimes,
-        'names': [0.3125, 0.75, 0.75, 0.3125, 0.3125, 0.9375, 0.3125, 0.3125]
+        'names': [
+            0.24180193241041126, 1.9297787196579723, 1.5617500744772101, 0.6811042561384157,
+            0.48017218468846856, 2.2867787591284823, 0.25476586891248476, 0.620052082101593
+        ]
     }, index=TEST_DATA_INDEX)
     pd.testing.assert_frame_equal(transformed, expected_transformed)
 
     reversed_datetimes = pd.to_datetime([
         '2010-01-09',
         '2010-02-01',
         '2010-01-01',
@@ -190,18 +208,18 @@
         for column in range(reverse_transformed.shape[1]):
             expected = expected_reversed.iloc[row, column]
             actual = reverse_transformed.iloc[row, column]
             assert pd.isna(actual) or expected == actual
 
     assert isinstance(ht.field_transformers['integer'], FloatFormatter)
     assert isinstance(ht.field_transformers['float'], FloatFormatter)
-    assert isinstance(ht.field_transformers['categorical'], FrequencyEncoder)
-    assert isinstance(ht.field_transformers['bool'], BinaryEncoder)
+    assert isinstance(ht.field_transformers['categorical'], LabelEncoder)
+    assert isinstance(ht.field_transformers['bool'], LabelEncoder)
     assert isinstance(ht.field_transformers['datetime'], UnixTimestampEncoder)
-    assert isinstance(ht.field_transformers['names'], FrequencyEncoder)
+    assert isinstance(ht.field_transformers['names'], LabelEncoder)
 
     get_default_transformers.cache_clear()
     get_default_transformer.cache_clear()
 
 
 def test_hypertransformer_field_transformers():
     """Test the HyperTransformer with ``field_transformers`` provided.
@@ -232,18 +250,18 @@
             'bool': 'boolean',
             'datetime': 'datetime',
             'names': 'categorical'
         },
         'transformers': {
             'integer': FloatFormatter(missing_value_replacement='mean'),
             'float': FloatFormatter(missing_value_replacement='mean'),
-            'categorical': FrequencyEncoder(),
-            'bool': BinaryEncoder(missing_value_replacement='mode'),
+            'categorical': LabelEncoder(add_noise=True),
+            'bool': LabelEncoder(add_noise=True),
             'datetime': DummyTransformerNotMLReady(),
-            'names': FrequencyEncoder()
+            'names': LabelEncoder(add_noise=True)
         }
     }
 
     data = get_input_data()
 
     # Run
     ht = HyperTransformer()
```

### Comparing `rdt_identity-1.6.0.dev0/tests/integration/test_transformers.py` & `rdt_identity-1.6.1.dev0/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/integration/transformers/pii/test_anonymizer.py` & `rdt_identity-1.6.1.dev0/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_base.py` & `rdt_identity-1.6.1.dev0/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_boolean.py` & `rdt_identity-1.6.1.dev0/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_categorical.py` & `rdt_identity-1.6.1.dev0/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_datetime.py` & `rdt_identity-1.6.1.dev0/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_numerical.py` & `rdt_identity-1.6.1.dev0/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_text.py` & `rdt_identity-1.6.1.dev0/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/performance/test_performance.py` & `rdt_identity-1.6.1.dev0/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/performance/tests/test_profiling.py` & `rdt_identity-1.6.1.dev0/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/test___init__.py` & `rdt_identity-1.6.1.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/test_hyper_transformer.py` & `rdt_identity-1.6.1.dev0/tests/unit/test_hyper_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,14 @@
     def test___init__(self, validation_mock, multi_column_mock):
         """Test create new instance of HyperTransformer"""
         # Run
         ht = HyperTransformer()
 
         # Asserts
         assert ht.field_sdtypes == {}
-        assert ht._default_sdtype_transformers == {}
         assert ht.field_transformers == {}
         assert ht._specified_fields == set()
         assert ht._valid_output_sdtypes == ht._DEFAULT_OUTPUT_SDTYPES
         assert ht._transformers_sequence == []
         assert ht._output_columns == []
         assert ht._input_columns == []
         assert ht._fitted_fields == set()
@@ -213,46 +212,57 @@
             - A DataFrame with multiple columns of different sdtypes.
 
         Side effects:
             - The appropriate ``sdtypes`` and ``transformers`` should be found.
         """
         # Setup
         data = self.get_data()
+        data['pii'] = ['a', 'b', 'c', 'd']
+        data['text'] = ['e', 'f', 'g', 'h']
         field_transformers = {
             'integer': FloatFormatter(),
             'float': ClusterBasedNormalizer(),
         }
-        default_sdtype_transformers = {
-            'boolean': BinaryEncoder(),
-            'categorical': FrequencyEncoder()
-        }
-        get_default_transformer_mock.return_value = UnixTimestampEncoder()
+        get_default_transformer_mock.side_effect = [
+            LabelEncoder(),
+            LabelEncoder(),
+            UnixTimestampEncoder(),
+            AnonymizedFaker(),
+            RegexGenerator(),
+        ]
         ht = HyperTransformer()
         ht.field_transformers = field_transformers
-        ht.field_sdtypes = {'datetime': 'datetime'}
-        ht._default_sdtype_transformers = default_sdtype_transformers
+        ht.field_sdtypes = {
+            'datetime': 'datetime',
+            'pii': 'pii',
+            'text': 'text'
+        }
         ht._unfit = Mock()
 
         # Run
         ht._learn_config(data)
 
         # Assert
         assert ht.field_sdtypes == {
             'integer': 'numerical',
             'float': 'numerical',
             'bool': 'boolean',
             'categorical': 'categorical',
-            'datetime': 'datetime'
+            'datetime': 'datetime',
+            'pii': 'pii',
+            'text': 'text',
         }
 
         assert isinstance(ht.field_transformers['integer'], FloatFormatter)
         assert isinstance(ht.field_transformers['float'], ClusterBasedNormalizer)
-        assert isinstance(ht.field_transformers['categorical'], FrequencyEncoder)
-        assert isinstance(ht.field_transformers['bool'], BinaryEncoder)
+        assert isinstance(ht.field_transformers['categorical'], LabelEncoder)
+        assert isinstance(ht.field_transformers['bool'], LabelEncoder)
         assert isinstance(ht.field_transformers['datetime'], UnixTimestampEncoder)
+        assert isinstance(ht.field_transformers['pii'], AnonymizedFaker)
+        assert isinstance(ht.field_transformers['text'], RegexGenerator)
         ht._unfit.assert_called_once()
 
     @patch('rdt.hyper_transformer.LOGGER')
     def test_detect_initial_config(self, logger_mock):
         """Test the ``detect_initial_config`` method.
 
         This tests that ``field_sdtypes`` and ``field_transformers`` are correctly set,
@@ -282,16 +292,16 @@
             'col4': 'datetime',
             'col5': 'numerical'
         }
 
         field_transformers = {k: repr(v) for (k, v) in ht.field_transformers.items()}
         assert field_transformers == {
             'col1': 'FloatFormatter()',
-            'col2': 'FrequencyEncoder()',
-            'col3': 'BinaryEncoder()',
+            'col2': 'LabelEncoder(add_noise=True)',
+            'col3': 'LabelEncoder(add_noise=True)',
             'col4': 'UnixTimestampEncoder()',
             'col5': 'FloatFormatter()'
         }
 
         expected_config = '\n'.join((
             '{',
             '    "sdtypes": {',
@@ -299,16 +309,16 @@
             '        "col2": "categorical",',
             '        "col3": "boolean",',
             '        "col4": "datetime",',
             '        "col5": "numerical"',
             '    },',
             '    "transformers": {',
             '        "col1": FloatFormatter(),',
-            '        "col2": FrequencyEncoder(),',
-            '        "col3": BinaryEncoder(),',
+            '        "col2": LabelEncoder(add_noise=True),',
+            '        "col3": LabelEncoder(add_noise=True),',
             '        "col4": UnixTimestampEncoder(),',
             '        "col5": FloatFormatter()',
             '    }',
             '}'
         ))
         logger_mock.info.assert_has_calls([
             call('Detecting a new config from the data ... SUCCESS'),
```

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/identity/test_identity.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/test_anonymizer.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/test_utils.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/test___init__.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/test___init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
 
-from rdt.transformers import BinaryEncoder, get_transformer_class, get_transformer_name
+from rdt.transformers import (
+    AnonymizedFaker, BinaryEncoder, FloatFormatter, LabelEncoder, RegexGenerator,
+    UnixTimestampEncoder, get_default_transformers, get_transformer_class, get_transformer_name)
 from rdt.transformers.addons.identity.identity import IdentityTransformer
 
 
 def test_get_transformer_name():
     """Test the ``get_transformer_name`` method.
 
     Validate the method returns the class path when passed the class.
@@ -90,7 +92,29 @@
     transformer_path = 'rdt.transformers.addons.identity.identity.IdentityTransformer'
 
     # Run
     returned = get_transformer_class(transformer_path)
 
     # Assert
     assert returned == IdentityTransformer
+
+
+def test_get_default_transformers():
+    """Test the ``get_default_transformers`` method.
+
+    Check that the right default transformer is returned for each type.
+    """
+    # Run
+    default_transformer_dict = get_default_transformers()
+
+    # Assert
+    expected_dict = {
+        'numerical': FloatFormatter,
+        'categorical': LabelEncoder,
+        'boolean': LabelEncoder,
+        'datetime': UnixTimestampEncoder,
+        'text': RegexGenerator,
+        'pii': AnonymizedFaker,
+    }
+
+    for sdtype, transformer in expected_dict.items():
+        assert isinstance(default_transformer_dict[sdtype], transformer)
```

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_base.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_boolean.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_categorical.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_datetime.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_null.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_numerical.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_text.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_utils.py` & `rdt_identity-1.6.1.dev0/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

