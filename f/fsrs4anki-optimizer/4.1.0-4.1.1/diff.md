# Comparing `tmp/fsrs4anki_optimizer-4.1.0.tar.gz` & `tmp/fsrs4anki_optimizer-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.1.0.tar", last modified: Mon Jul 17 03:40:25 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.1.1.tar", last modified: Mon Jul 17 07:40:43 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.1.0.tar` & `fsrs4anki_optimizer-4.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:40:25.845582 fsrs4anki_optimizer-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 03:40:25.845582 fsrs4anki_optimizer-4.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:40:25.845582 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 03:40:13.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-17 03:40:13.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50266 2023-07-17 03:40:13.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:40:25.845582 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 03:40:25.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 03:40:25.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:40:25.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 03:40:25.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 03:40:25.000000 fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-17 03:40:13.000000 fsrs4anki_optimizer-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:40:25.845582 fsrs4anki_optimizer-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 03:40:13.000000 fsrs4anki_optimizer-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:43.151601 fsrs4anki_optimizer-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 07:40:43.151601 fsrs4anki_optimizer-4.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:43.151601 fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 07:40:24.000000 fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-17 07:40:24.000000 fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50266 2023-07-17 07:40:24.000000 fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:40:43.151601 fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 07:40:43.000000 fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 07:40:43.000000 fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:40:43.000000 fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 07:40:43.000000 fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 07:40:43.000000 fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-17 07:40:24.000000 fsrs4anki_optimizer-4.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:40:43.151601 fsrs4anki_optimizer-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 07:40:24.000000 fsrs4anki_optimizer-4.1.1/setup.py
```

### Comparing `fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-4.1.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.1.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files identical despite different names*

