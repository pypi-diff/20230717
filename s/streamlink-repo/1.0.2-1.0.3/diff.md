# Comparing `tmp/streamlink-repo-1.0.2.tar.gz` & `tmp/streamlink-repo-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\streamlink-repo-1.0.2.tar", last modified: Mon Jul 17 13:01:59 2023, max compression
+gzip compressed data, was "dist\streamlink-repo-1.0.3.tar", last modified: Mon Jul 17 15:17:36 2023, max compression
```

## Comparing `streamlink-repo-1.0.2.tar` & `streamlink-repo-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 13:01:59.341019 streamlink-repo-1.0.2/
--rw-rw-rw-   0        0        0    17096 2023-07-17 12:16:21.000000 streamlink-repo-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      186 2023-07-17 13:01:59.340031 streamlink-repo-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-17 13:01:59.342036 streamlink-repo-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      554 2023-07-17 12:41:25.000000 streamlink-repo-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:01:59.319741 streamlink-repo-1.0.2/streamlink_repo/
--rw-rw-rw-   0        0        0    13925 2023-07-17 12:57:44.000000 streamlink-repo-1.0.2/streamlink_repo/__init__.py
--rw-rw-rw-   0        0        0     4635 2023-07-17 12:35:55.000000 streamlink-repo-1.0.2/streamlink_repo/common.py
--rw-rw-rw-   0        0        0      632 2023-07-17 08:49:48.000000 streamlink-repo-1.0.2/streamlink_repo/paths.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:01:59.337897 streamlink-repo-1.0.2/streamlink_repo.egg-info/
--rw-rw-rw-   0        0        0      186 2023-07-17 13:01:59.000000 streamlink-repo-1.0.2/streamlink_repo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-07-17 13:01:59.000000 streamlink-repo-1.0.2/streamlink_repo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 13:01:59.000000 streamlink-repo-1.0.2/streamlink_repo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-17 13:01:59.000000 streamlink-repo-1.0.2/streamlink_repo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-07-17 13:01:59.000000 streamlink-repo-1.0.2/streamlink_repo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-17 13:01:59.000000 streamlink-repo-1.0.2/streamlink_repo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 15:17:36.039396 streamlink-repo-1.0.3/
+-rw-rw-rw-   0        0        0    17096 2023-07-17 12:16:21.000000 streamlink-repo-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1416 2023-07-17 15:17:36.038368 streamlink-repo-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1187 2023-07-17 15:14:48.000000 streamlink-repo-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 15:17:36.039396 streamlink-repo-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      664 2023-07-17 15:17:19.000000 streamlink-repo-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:17:36.007243 streamlink-repo-1.0.3/streamlink_repo/
+-rw-rw-rw-   0        0        0    13925 2023-07-17 12:57:44.000000 streamlink-repo-1.0.3/streamlink_repo/__init__.py
+-rw-rw-rw-   0        0        0     4635 2023-07-17 12:35:55.000000 streamlink-repo-1.0.3/streamlink_repo/common.py
+-rw-rw-rw-   0        0        0      632 2023-07-17 08:49:48.000000 streamlink-repo-1.0.3/streamlink_repo/paths.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:17:36.036272 streamlink-repo-1.0.3/streamlink_repo.egg-info/
+-rw-rw-rw-   0        0        0     1416 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/top_level.txt
```

### Comparing `streamlink-repo-1.0.2/LICENSE` & `streamlink-repo-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.2/streamlink_repo/__init__.py` & `streamlink-repo-1.0.3/streamlink_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.2/streamlink_repo/common.py` & `streamlink-repo-1.0.3/streamlink_repo/common.py`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.2/streamlink_repo/paths.py` & `streamlink-repo-1.0.3/streamlink_repo/paths.py`

 * *Files identical despite different names*

