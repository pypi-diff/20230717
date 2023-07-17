# Comparing `tmp/multimcts-0.1.2.tar.gz` & `tmp/multimcts-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.1.2.tar", last modified: Mon Jul 17 19:23:02 2023, max compression
+gzip compressed data, was "multimcts-0.1.3.tar", last modified: Mon Jul 17 19:25:38 2023, max compression
```

## Comparing `multimcts-0.1.2.tar` & `multimcts-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 19:23:02.131466 multimcts-0.1.2/
--rw-r--r--   0 taylorvance   (501) staff       (20)      228 2023-07-17 19:23:02.131324 multimcts-0.1.2/PKG-INFO
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 19:23:02.129020 multimcts-0.1.2/multimcts/
--rw-r--r--   0 taylorvance   (501) staff       (20)   257682 2023-07-17 17:46:23.000000 multimcts-0.1.2/multimcts/gamestate.c
--rw-r--r--   0 taylorvance   (501) staff       (20)   434959 2023-07-17 17:46:23.000000 multimcts-0.1.2/multimcts/mcts.c
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 19:23:02.131111 multimcts-0.1.2/multimcts.egg-info/
--rw-r--r--   0 taylorvance   (501) staff       (20)      228 2023-07-17 19:23:02.000000 multimcts-0.1.2/multimcts.egg-info/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)      226 2023-07-17 19:23:02.000000 multimcts-0.1.2/multimcts.egg-info/SOURCES.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 19:23:02.000000 multimcts-0.1.2/multimcts.egg-info/dependency_links.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 19:12:04.000000 multimcts-0.1.2/multimcts.egg-info/not-zip-safe
--rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-17 19:23:02.000000 multimcts-0.1.2/multimcts.egg-info/top_level.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-17 18:23:36.000000 multimcts-0.1.2/pyproject.toml
--rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-17 19:23:02.131524 multimcts-0.1.2/setup.cfg
--rw-r--r--   0 taylorvance   (501) staff       (20)      539 2023-07-17 19:22:56.000000 multimcts-0.1.2/setup.py
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 19:25:38.240318 multimcts-0.1.3/
+-rw-r--r--   0 taylorvance   (501) staff       (20)      228 2023-07-17 19:25:38.240165 multimcts-0.1.3/PKG-INFO
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 19:25:38.237741 multimcts-0.1.3/multimcts/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       56 2023-07-17 17:45:55.000000 multimcts-0.1.3/multimcts/__init__.py
+-rw-r--r--   0 taylorvance   (501) staff       (20)   257682 2023-07-17 17:46:23.000000 multimcts-0.1.3/multimcts/gamestate.c
+-rw-r--r--   0 taylorvance   (501) staff       (20)   434959 2023-07-17 17:46:23.000000 multimcts-0.1.3/multimcts/mcts.c
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 19:25:38.239904 multimcts-0.1.3/multimcts.egg-info/
+-rw-r--r--   0 taylorvance   (501) staff       (20)      228 2023-07-17 19:25:38.000000 multimcts-0.1.3/multimcts.egg-info/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)      248 2023-07-17 19:25:38.000000 multimcts-0.1.3/multimcts.egg-info/SOURCES.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 19:25:38.000000 multimcts-0.1.3/multimcts.egg-info/dependency_links.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 19:12:04.000000 multimcts-0.1.3/multimcts.egg-info/not-zip-safe
+-rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-17 19:25:38.000000 multimcts-0.1.3/multimcts.egg-info/top_level.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-17 18:23:36.000000 multimcts-0.1.3/pyproject.toml
+-rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-17 19:25:38.240387 multimcts-0.1.3/setup.cfg
+-rw-r--r--   0 taylorvance   (501) staff       (20)      567 2023-07-17 19:25:25.000000 multimcts-0.1.3/setup.py
```

### Comparing `multimcts-0.1.2/multimcts/gamestate.c` & `multimcts-0.1.3/multimcts/gamestate.c`

 * *Files identical despite different names*

### Comparing `multimcts-0.1.2/multimcts/mcts.c` & `multimcts-0.1.3/multimcts/mcts.c`

 * *Files identical despite different names*

### Comparing `multimcts-0.1.2/setup.py` & `multimcts-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 extensions = [
     Extension("multimcts.mcts", ["multimcts/mcts.pyx"]),
     Extension("multimcts.gamestate", ["multimcts/gamestate.pyx"]),
 ]
 
 setup(
     name="multimcts",
-    version="0.1.2",
+    version="0.1.3",
     author="Taylor Vance",
     author_email="mirrors.cities0w@icloud.com",
     # url="https://github.com/taylorvance/multimcts",
     description="Monte Carlo Tree Search for multiple teams",
     license="MIT",
+    packages=["multimcts"],
     ext_modules=cythonize(extensions),
     zip_safe=False,
 )
```

