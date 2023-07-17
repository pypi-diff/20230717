# Comparing `tmp/clauderevised-0.0.1.tar.gz` & `tmp/clauderevised-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clauderevised-0.0.1.tar", last modified: Mon Jul 17 08:07:37 2023, max compression
+gzip compressed data, was "clauderevised-0.0.2.tar", last modified: Mon Jul 17 08:10:46 2023, max compression
```

## Comparing `clauderevised-0.0.1.tar` & `clauderevised-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-17 08:07:37.251857 clauderevised-0.0.1/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      112 2023-07-17 08:07:37.251620 clauderevised-0.0.1/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3215 2023-07-17 07:55:04.000000 clauderevised-0.0.1/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-17 08:07:37.251222 clauderevised-0.0.1/clauderevised.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      112 2023-07-17 08:07:37.000000 clauderevised-0.0.1/clauderevised.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)      202 2023-07-17 08:07:37.000000 clauderevised-0.0.1/clauderevised.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-17 08:07:37.000000 clauderevised-0.0.1/clauderevised.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        9 2023-07-17 08:07:37.000000 clauderevised-0.0.1/clauderevised.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       10 2023-07-17 08:07:37.000000 clauderevised-0.0.1/clauderevised.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-17 08:07:37.251983 clauderevised-0.0.1/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      240 2023-07-17 08:07:27.000000 clauderevised-0.0.1/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-17 08:10:46.277402 clauderevised-0.0.2/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      112 2023-07-17 08:10:46.277133 clauderevised-0.0.2/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3215 2023-07-17 07:55:04.000000 clauderevised-0.0.2/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-17 08:10:46.274553 clauderevised-0.0.2/clauderevised/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-17 07:50:26.000000 clauderevised-0.0.2/clauderevised/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3661 2023-07-17 07:50:29.000000 clauderevised-0.0.2/clauderevised/claude.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-17 08:10:46.276632 clauderevised-0.0.2/clauderevised.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      112 2023-07-17 08:10:46.000000 clauderevised-0.0.2/clauderevised.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      252 2023-07-17 08:10:46.000000 clauderevised-0.0.2/clauderevised.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-17 08:10:46.000000 clauderevised-0.0.2/clauderevised.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        9 2023-07-17 08:10:46.000000 clauderevised-0.0.2/clauderevised.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       14 2023-07-17 08:10:46.000000 clauderevised-0.0.2/clauderevised.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-17 08:10:46.277511 clauderevised-0.0.2/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      239 2023-07-17 08:10:14.000000 clauderevised-0.0.2/setup.py
```

### Comparing `clauderevised-0.0.1/README.md` & `clauderevised-0.0.2/README.md`

 * *Files identical despite different names*

