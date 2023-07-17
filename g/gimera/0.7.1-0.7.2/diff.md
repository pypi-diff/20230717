# Comparing `tmp/gimera-0.7.1.tar.gz` & `tmp/gimera-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimera-0.7.1.tar", last modified: Thu Jun 29 06:21:41 2023, max compression
+gzip compressed data, was "gimera-0.7.2.tar", last modified: Mon Jul 17 10:17:10 2023, max compression
```

## Comparing `gimera-0.7.1.tar` & `gimera-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:21:41.512135 gimera-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 06:20:56.000000 gimera-0.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-29 06:21:41.512135 gimera-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-29 06:20:56.000000 gimera-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:21:41.512135 gimera-0.7.1/gimera/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37461 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/gimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/gitcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:21:41.512135 gimera-0.7.1/gimera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 06:21:41.512135 gimera-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-29 06:20:56.000000 gimera-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:17:10.113565 gimera-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-17 10:16:19.000000 gimera-0.7.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-17 10:17:10.113565 gimera-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-17 10:16:19.000000 gimera-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:17:10.113565 gimera-0.7.2/gimera/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37461 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/gimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/gitcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-17 10:16:19.000000 gimera-0.7.2/gimera/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:17:10.113565 gimera-0.7.2/gimera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 10:17:10.000000 gimera-0.7.2/gimera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 10:17:10.113565 gimera-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-17 10:16:19.000000 gimera-0.7.2/setup.py
```

### Comparing `gimera-0.7.1/LICENSE.txt` & `gimera-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gimera-0.7.1/PKG-INFO` & `gimera-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.1
+Version: 0.7.2
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.1/README.md` & `gimera-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `gimera-0.7.1/gimera/config.py` & `gimera-0.7.2/gimera/config.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.1/gimera/gimera.py` & `gimera-0.7.2/gimera/gimera.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.1/gimera/gitcommands.py` & `gimera-0.7.2/gimera/gitcommands.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.1/gimera/repo.py` & `gimera-0.7.2/gimera/repo.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.1/gimera/tools.py` & `gimera-0.7.2/gimera/tools.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.1/gimera.egg-info/PKG-INFO` & `gimera-0.7.2/gimera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.1
+Version: 0.7.2
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.1/setup.py` & `gimera-0.7.2/setup.py`

 * *Files identical despite different names*

