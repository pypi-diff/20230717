# Comparing `tmp/mstuff-0.7.8.tar.gz` & `tmp/mstuff-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mstuff-0.7.8.tar", last modified: Mon Jul 17 17:26:21 2023, max compression
+gzip compressed data, was "mstuff-0.7.9.tar", last modified: Mon Jul 17 17:37:52 2023, max compression
```

## Comparing `mstuff-0.7.8.tar` & `mstuff-0.7.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-07-17 17:26:21.717814 mstuff-0.7.8/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-07-17 17:26:21.717633 mstuff-0.7.8/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:02.000000 mstuff-0.7.8/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-07-17 17:26:21.716722 mstuff-0.7.8/mstuff/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      163 2023-03-08 18:10:18.000000 mstuff-0.7.8/mstuff/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     3836 2023-07-03 15:22:37.000000 mstuff-0.7.8/mstuff/http.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     3822 2023-07-17 17:25:27.000000 mstuff-0.7.8/mstuff/mstuff.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-07-17 17:26:21.717440 mstuff-0.7.8/mstuff.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-07-17 17:26:21.000000 mstuff-0.7.8/mstuff.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      225 2023-07-17 17:26:21.000000 mstuff-0.7.8/mstuff.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-07-17 17:26:21.000000 mstuff-0.7.8/mstuff.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       17 2023-07-17 17:26:21.000000 mstuff-0.7.8/mstuff.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        7 2023-07-17 17:26:21.000000 mstuff-0.7.8/mstuff.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      186 2023-07-17 17:26:17.000000 mstuff-0.7.8/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-07-17 17:26:21.717871 mstuff-0.7.8/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-07-17 17:37:52.304831 mstuff-0.7.9/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-07-17 17:37:52.304677 mstuff-0.7.9/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:02.000000 mstuff-0.7.9/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-07-17 17:37:52.303783 mstuff-0.7.9/mstuff/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      163 2023-03-08 18:10:18.000000 mstuff-0.7.9/mstuff/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     3836 2023-07-03 15:22:37.000000 mstuff-0.7.9/mstuff/http.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     4668 2023-07-17 17:37:36.000000 mstuff-0.7.9/mstuff/mstuff.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-07-17 17:37:52.304470 mstuff-0.7.9/mstuff.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-07-17 17:37:52.000000 mstuff-0.7.9/mstuff.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      225 2023-07-17 17:37:52.000000 mstuff-0.7.9/mstuff.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-07-17 17:37:52.000000 mstuff-0.7.9/mstuff.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       17 2023-07-17 17:37:52.000000 mstuff-0.7.9/mstuff.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        7 2023-07-17 17:37:52.000000 mstuff-0.7.9/mstuff.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      186 2023-07-17 17:37:47.000000 mstuff-0.7.9/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-07-17 17:37:52.304872 mstuff-0.7.9/setup.cfg
```

### Comparing `mstuff-0.7.8/mstuff/http.py` & `mstuff-0.7.9/mstuff/http.py`

 * *Files identical despite different names*

