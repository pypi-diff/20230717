# Comparing `tmp/webreq-1.0.0.tar.gz` & `tmp/webreq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webreq-1.0.0.tar", last modified: Mon Jul 17 03:17:46 2023, max compression
+gzip compressed data, was "webreq-1.0.1.tar", last modified: Mon Jul 17 09:47:38 2023, max compression
```

## Comparing `webreq-1.0.0.tar` & `webreq-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 03:17:46.745726 webreq-1.0.0/
--rw-rw-rw-   0        0        0       97 2023-07-17 03:17:46.745726 webreq-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-17 03:16:23.000000 webreq-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 03:17:46.745726 webreq-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      177 2023-07-17 03:17:30.000000 webreq-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:17:46.729907 webreq-1.0.0/webreq/
--rw-rw-rw-   0        0        0     4963 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/__init__.py
--rw-rw-rw-   0        0        0      435 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/__version__.py
--rw-rw-rw-   0        0        0     1495 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/_internal_utils.py
--rw-rw-rw-   0        0        0    19553 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/adapters.py
--rw-rw-rw-   0        0        0     6449 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/api.py
--rw-rw-rw-   0        0        0    10187 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/auth.py
--rw-rw-rw-   0        0        0      429 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/certs.py
--rw-rw-rw-   0        0        0     1451 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/compat.py
--rw-rw-rw-   0        0        0    18560 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/cookies.py
--rw-rw-rw-   0        0        0     3811 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/exceptions.py
--rw-rw-rw-   0        0        0     3875 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/help.py
--rw-rw-rw-   0        0        0      733 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/hooks.py
--rw-rw-rw-   0        0        0    35223 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/models.py
--rw-rw-rw-   0        0        0      957 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/packages.py
--rw-rw-rw-   0        0        0    30373 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/sessions.py
--rw-rw-rw-   0        0        0     4235 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/status_codes.py
--rw-rw-rw-   0        0        0     2912 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/structures.py
--rw-rw-rw-   0        0        0    33448 2023-07-17 02:54:26.000000 webreq-1.0.0/webreq/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:17:46.745726 webreq-1.0.0/webreq.egg-info/
--rw-rw-rw-   0        0        0       97 2023-07-17 03:17:46.000000 webreq-1.0.0/webreq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-07-17 03:17:46.000000 webreq-1.0.0/webreq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 03:17:46.000000 webreq-1.0.0/webreq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-17 03:17:46.000000 webreq-1.0.0/webreq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 09:47:38.648424 webreq-1.0.1/
+-rw-rw-rw-   0        0        0       97 2023-07-17 09:47:38.648424 webreq-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-17 03:16:23.000000 webreq-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:47:38.648424 webreq-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-07-17 09:40:16.000000 webreq-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:47:38.617426 webreq-1.0.1/webreq/
+-rw-rw-rw-   0        0        0     4963 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/__version__.py
+-rw-rw-rw-   0        0        0     1495 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/_internal_utils.py
+-rw-rw-rw-   0        0        0    19553 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/adapters.py
+-rw-rw-rw-   0        0        0     6449 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/api.py
+-rw-rw-rw-   0        0        0    10187 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/auth.py
+-rw-rw-rw-   0        0        0      429 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/certs.py
+-rw-rw-rw-   0        0        0     1451 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/cookies.py
+-rw-rw-rw-   0        0        0     3811 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/exceptions.py
+-rw-rw-rw-   0        0        0     3875 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/help.py
+-rw-rw-rw-   0        0        0      733 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/hooks.py
+-rw-rw-rw-   0        0        0    35223 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/models.py
+-rw-rw-rw-   0        0        0      957 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/packages.py
+-rw-rw-rw-   0        0        0    30373 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/structures.py
+-rw-rw-rw-   0        0        0    33448 2023-07-17 02:54:26.000000 webreq-1.0.1/webreq/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:47:38.648424 webreq-1.0.1/webreq.egg-info/
+-rw-rw-rw-   0        0        0       97 2023-07-17 09:47:38.000000 webreq-1.0.1/webreq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-07-17 09:47:38.000000 webreq-1.0.1/webreq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:47:38.000000 webreq-1.0.1/webreq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-17 09:47:38.000000 webreq-1.0.1/webreq.egg-info/top_level.txt
```

### Comparing `webreq-1.0.0/webreq/__init__.py` & `webreq-1.0.1/webreq/__init__.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/_internal_utils.py` & `webreq-1.0.1/webreq/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/adapters.py` & `webreq-1.0.1/webreq/adapters.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/api.py` & `webreq-1.0.1/webreq/api.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/auth.py` & `webreq-1.0.1/webreq/auth.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/compat.py` & `webreq-1.0.1/webreq/compat.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/cookies.py` & `webreq-1.0.1/webreq/cookies.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/exceptions.py` & `webreq-1.0.1/webreq/exceptions.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/help.py` & `webreq-1.0.1/webreq/help.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/hooks.py` & `webreq-1.0.1/webreq/hooks.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/models.py` & `webreq-1.0.1/webreq/models.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/packages.py` & `webreq-1.0.1/webreq/packages.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/sessions.py` & `webreq-1.0.1/webreq/sessions.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/status_codes.py` & `webreq-1.0.1/webreq/status_codes.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/structures.py` & `webreq-1.0.1/webreq/structures.py`

 * *Files identical despite different names*

### Comparing `webreq-1.0.0/webreq/utils.py` & `webreq-1.0.1/webreq/utils.py`

 * *Files identical despite different names*

