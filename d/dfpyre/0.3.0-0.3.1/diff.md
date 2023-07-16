# Comparing `tmp/dfpyre-0.3.0.tar.gz` & `tmp/dfpyre-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfpyre-0.3.0.tar", last modified: Sat Jul 15 02:40:24 2023, max compression
+gzip compressed data, was "dfpyre-0.3.1.tar", last modified: Sun Jul 16 23:37:30 2023, max compression
```

## Comparing `dfpyre-0.3.0.tar` & `dfpyre-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 02:40:24.212761 dfpyre-0.3.0/
--rw-rw-rw-   0        0        0     1081 2023-07-15 02:28:19.000000 dfpyre-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      275 2023-07-15 02:40:24.212761 dfpyre-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    10197 2023-07-14 03:50:47.000000 dfpyre-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 02:40:24.189477 dfpyre-0.3.0/dfpyre/
--rw-rw-rw-   0        0        0       25 2023-07-14 02:26:37.000000 dfpyre-0.3.0/dfpyre/__init__.py
--rw-rw-rw-   0        0        0     5555 2023-07-14 03:05:11.000000 dfpyre-0.3.0/dfpyre/items.py
--rw-rw-rw-   0        0        0    11831 2023-07-15 02:16:20.000000 dfpyre-0.3.0/dfpyre/pyre.py
-drwxrwxrwx   0        0        0        0 2023-07-15 02:40:24.210760 dfpyre-0.3.0/dfpyre.egg-info/
--rw-rw-rw-   0        0        0      275 2023-07-15 02:40:24.000000 dfpyre-0.3.0/dfpyre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-07-15 02:40:24.000000 dfpyre-0.3.0/dfpyre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 02:40:24.000000 dfpyre-0.3.0/dfpyre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-15 02:40:24.000000 dfpyre-0.3.0/dfpyre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 02:40:24.213762 dfpyre-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      361 2023-07-15 02:37:03.000000 dfpyre-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:37:30.622538 dfpyre-0.3.1/
+-rw-rw-rw-   0        0        0     1081 2023-07-15 02:28:19.000000 dfpyre-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      275 2023-07-16 23:37:30.621268 dfpyre-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10197 2023-07-14 03:50:47.000000 dfpyre-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 23:37:30.580906 dfpyre-0.3.1/dfpyre/
+-rw-rw-rw-   0        0        0       25 2023-07-14 02:26:37.000000 dfpyre-0.3.1/dfpyre/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:37:30.620269 dfpyre-0.3.1/dfpyre/data/
+-rw-rw-rw-   0        0        0    50261 2023-07-14 02:33:57.000000 dfpyre-0.3.1/dfpyre/data/data.json
+-rw-rw-rw-   0        0        0     5555 2023-07-14 03:05:11.000000 dfpyre-0.3.1/dfpyre/items.py
+-rw-rw-rw-   0        0        0    11831 2023-07-15 02:16:20.000000 dfpyre-0.3.1/dfpyre/pyre.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:37:30.606680 dfpyre-0.3.1/dfpyre.egg-info/
+-rw-rw-rw-   0        0        0      275 2023-07-16 23:37:30.000000 dfpyre-0.3.1/dfpyre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-16 23:37:30.000000 dfpyre-0.3.1/dfpyre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 23:37:30.000000 dfpyre-0.3.1/dfpyre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 23:37:30.000000 dfpyre-0.3.1/dfpyre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 23:37:30.622538 dfpyre-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      410 2023-07-16 23:37:24.000000 dfpyre-0.3.1/setup.py
```

### Comparing `dfpyre-0.3.0/LICENSE` & `dfpyre-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dfpyre-0.3.0/README.md` & `dfpyre-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dfpyre-0.3.0/dfpyre/items.py` & `dfpyre-0.3.1/dfpyre/items.py`

 * *Files identical despite different names*

### Comparing `dfpyre-0.3.0/dfpyre/pyre.py` & `dfpyre-0.3.1/dfpyre/pyre.py`

 * *Files identical despite different names*

