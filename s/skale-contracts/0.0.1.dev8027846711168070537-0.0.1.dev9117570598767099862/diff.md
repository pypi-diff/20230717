# Comparing `tmp/skale-contracts-0.0.1.dev8027846711168070537.tar.gz` & `tmp/skale-contracts-0.0.1.dev9117570598767099862.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skale-contracts-0.0.1.dev8027846711168070537.tar", last modified: Thu Jul 13 13:52:38 2023, max compression
+gzip compressed data, was "skale-contracts-0.0.1.dev9117570598767099862.tar", last modified: Fri Jul 14 09:28:22 2023, max compression
```

## Comparing `skale-contracts-0.0.1.dev8027846711168070537.tar` & `skale-contracts-0.0.1.dev9117570598767099862.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:52:38.562816 skale-contracts-0.0.1.dev8027846711168070537/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-13 13:52:38.562816 skale-contracts-0.0.1.dev8027846711168070537/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 13:52:20.000000 skale-contracts-0.0.1.dev8027846711168070537/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 13:52:20.000000 skale-contracts-0.0.1.dev8027846711168070537/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-13 13:52:38.566816 skale-contracts-0.0.1.dev8027846711168070537/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:52:38.562816 skale-contracts-0.0.1.dev8027846711168070537/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:52:38.562816 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-13 13:52:38.000000 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 13:52:38.000000 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:52:38.000000 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 13:52:38.000000 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:52:38.000000 skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 13:52:29.000000 skale-contracts-0.0.1.dev8027846711168070537/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:22.620516 skale-contracts-0.0.1.dev9117570598767099862/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-14 09:28:22.624516 skale-contracts-0.0.1.dev9117570598767099862/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 09:28:08.000000 skale-contracts-0.0.1.dev9117570598767099862/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 09:28:08.000000 skale-contracts-0.0.1.dev9117570598767099862/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-14 09:28:22.624516 skale-contracts-0.0.1.dev9117570598767099862/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:22.616516 skale-contracts-0.0.1.dev9117570598767099862/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:22.620516 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-14 09:28:08.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 09:28:08.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-14 09:28:08.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-14 09:28:08.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-14 09:28:08.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-14 09:28:08.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 09:28:08.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts/skale_contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:22.620516 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-14 09:28:22.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 09:28:22.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:28:22.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 09:28:22.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 09:28:22.000000 skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-14 09:28:15.000000 skale-contracts-0.0.1.dev9117570598767099862/version.txt
```

### Comparing `skale-contracts-0.0.1.dev8027846711168070537/PKG-INFO` & `skale-contracts-0.0.1.dev9117570598767099862/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 0.0.1.dev8027846711168070537
+Version: 0.0.1.dev9117570598767099862
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `skale-contracts-0.0.1.dev8027846711168070537/setup.cfg` & `skale-contracts-0.0.1.dev9117570598767099862/setup.cfg`

 * *Files identical despite different names*

### Comparing `skale-contracts-0.0.1.dev8027846711168070537/src/skale_contracts.egg-info/PKG-INFO` & `skale-contracts-0.0.1.dev9117570598767099862/src/skale_contracts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 0.0.1.dev8027846711168070537
+Version: 0.0.1.dev9117570598767099862
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

