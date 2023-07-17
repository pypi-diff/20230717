# Comparing `tmp/multimcts-0.1.tar.gz` & `tmp/multimcts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.1.tar", last modified: Mon Jul 17 17:52:07 2023, max compression
+gzip compressed data, was "multimcts-0.1.1.tar", last modified: Mon Jul 17 18:25:23 2023, max compression
```

## Comparing `multimcts-0.1.tar` & `multimcts-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 17:52:07.545232 multimcts-0.1/
--rw-r--r--   0 taylorvance   (501) staff       (20)      184 2023-07-17 17:52:07.545111 multimcts-0.1/PKG-INFO
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 17:52:07.543567 multimcts-0.1/multimcts/
--rw-r--r--   0 taylorvance   (501) staff       (20)   257682 2023-07-17 17:46:23.000000 multimcts-0.1/multimcts/gamestate.c
--rw-r--r--   0 taylorvance   (501) staff       (20)   434959 2023-07-17 17:46:23.000000 multimcts-0.1/multimcts/mcts.c
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 17:52:07.544942 multimcts-0.1/multimcts.egg-info/
--rw-r--r--   0 taylorvance   (501) staff       (20)      184 2023-07-17 17:52:07.000000 multimcts-0.1/multimcts.egg-info/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)      211 2023-07-17 17:52:07.000000 multimcts-0.1/multimcts.egg-info/SOURCES.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 17:52:07.000000 multimcts-0.1/multimcts.egg-info/dependency_links.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 17:52:07.000000 multimcts-0.1/multimcts.egg-info/not-zip-safe
--rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-17 17:52:07.000000 multimcts-0.1/multimcts.egg-info/top_level.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-17 17:52:07.545272 multimcts-0.1/setup.cfg
--rw-r--r--   0 taylorvance   (501) staff       (20)      435 2023-07-17 17:45:42.000000 multimcts-0.1/setup.py
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 18:25:23.746109 multimcts-0.1.1/
+-rw-r--r--   0 taylorvance   (501) staff       (20)      186 2023-07-17 18:25:23.745967 multimcts-0.1.1/PKG-INFO
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 18:25:23.743815 multimcts-0.1.1/multimcts/
+-rw-r--r--   0 taylorvance   (501) staff       (20)   257682 2023-07-17 17:46:23.000000 multimcts-0.1.1/multimcts/gamestate.c
+-rw-r--r--   0 taylorvance   (501) staff       (20)   434959 2023-07-17 17:46:23.000000 multimcts-0.1.1/multimcts/mcts.c
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 18:25:23.745778 multimcts-0.1.1/multimcts.egg-info/
+-rw-r--r--   0 taylorvance   (501) staff       (20)      186 2023-07-17 18:25:23.000000 multimcts-0.1.1/multimcts.egg-info/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)      226 2023-07-17 18:25:23.000000 multimcts-0.1.1/multimcts.egg-info/SOURCES.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 18:25:23.000000 multimcts-0.1.1/multimcts.egg-info/dependency_links.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 17:52:07.000000 multimcts-0.1.1/multimcts.egg-info/not-zip-safe
+-rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-17 18:25:23.000000 multimcts-0.1.1/multimcts.egg-info/top_level.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-17 18:23:36.000000 multimcts-0.1.1/pyproject.toml
+-rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-17 18:25:23.746155 multimcts-0.1.1/setup.cfg
+-rw-r--r--   0 taylorvance   (501) staff       (20)      437 2023-07-17 18:25:03.000000 multimcts-0.1.1/setup.py
```

### Comparing `multimcts-0.1/multimcts/gamestate.c` & `multimcts-0.1.1/multimcts/gamestate.c`

 * *Files identical despite different names*

### Comparing `multimcts-0.1/multimcts/mcts.c` & `multimcts-0.1.1/multimcts/mcts.c`

 * *Files identical despite different names*

