# Comparing `tmp/roblox-pyc-1.6.6.5.4.tar.gz` & `tmp/roblox-pyc-1.6.6.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-1.6.6.5.4.tar", last modified: Sun Jul  9 21:03:36 2023, max compression
+gzip compressed data, was "roblox-pyc-1.6.6.5a0.tar", last modified: Sun Jul  9 20:03:59 2023, max compression
```

## Comparing `roblox-pyc-1.6.6.5.4.tar` & `roblox-pyc-1.6.6.5a0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:03:36.243073 roblox-pyc-1.6.6.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34525 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-09 21:03:36.243073 roblox-pyc-1.6.6.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:03:36.239073 roblox-pyc-1.6.6.5.4/roblox_pyc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-09 21:03:36.000000 roblox-pyc-1.6.6.5.4/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-09 21:03:36.000000 roblox-pyc-1.6.6.5.4/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:03:36.000000 roblox-pyc-1.6.6.5.4/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-09 21:03:36.000000 roblox-pyc-1.6.6.5.4/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-09 21:03:36.000000 roblox-pyc-1.6.6.5.4/roblox_pyc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 21:03:36.000000 roblox-pyc-1.6.6.5.4/roblox_pyc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-09 21:03:36.243073 roblox-pyc-1.6.6.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:03:36.243073 roblox-pyc-1.6.6.5.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/binopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/boolopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/cmpopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/cnodevisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/colortext.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/cpAST.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/ctranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/header.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/loopcounter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/luainit.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/nameconstdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27684 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/nodevisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/pytranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/robloxpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/symbolsstack.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/tokenendmode.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-09 21:03:24.000000 roblox-pyc-1.6.6.5.4/src/unaryopdesc.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 20:03:59.818242 roblox-pyc-1.6.6.5a0/
+-rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/LICENSE
+-rw-r--r--   0 aaravs     (501) staff       (20)     3010 2023-07-09 20:03:59.818469 roblox-pyc-1.6.6.5a0/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)     2784 2023-07-09 17:36:20.000000 roblox-pyc-1.6.6.5a0/README.md
+-rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.6.6.5a0/pyproject.toml
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 20:03:59.798189 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/
+-rw-r--r--   0 aaravs     (501) staff       (20)     3010 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)      606 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      102 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)       43 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/requires.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/top_level.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      243 2023-07-09 20:03:59.819423 roblox-pyc-1.6.6.5a0/setup.cfg
+-rw-r--r--   0 aaravs     (501) staff       (20)      440 2023-07-09 15:41:08.000000 roblox-pyc-1.6.6.5a0/setup.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 20:03:59.817083 roblox-pyc-1.6.6.5a0/src/
+-rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/__init__.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/binopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/boolopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/cmpopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1848 2023-07-09 20:00:46.000000 roblox-pyc-1.6.6.5a0/src/cnodevisitor.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.6.6.5a0/src/colortext.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/config.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/context.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      447 2023-07-09 15:13:23.000000 roblox-pyc-1.6.6.5a0/src/cpAST.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      404 2023-07-09 20:02:43.000000 roblox-pyc-1.6.6.5a0/src/ctranslator.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      482 2023-07-09 17:33:56.000000 roblox-pyc-1.6.6.5a0/src/header.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.6.6.5a0/src/loopcounter.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    21165 2023-07-09 17:23:29.000000 roblox-pyc-1.6.6.5a0/src/luainit.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/nameconstdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.6.6.5a0/src/nodevisitor.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     2153 2023-07-09 17:33:27.000000 roblox-pyc-1.6.6.5a0/src/pytranslator.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     7632 2023-07-09 18:40:50.000000 roblox-pyc-1.6.6.5a0/src/robloxpy.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/symbolsstack.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/tokenendmode.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.6.6.5a0/src/unaryopdesc.py
```

### Comparing `roblox-pyc-1.6.6.5.4/LICENSE` & `roblox-pyc-1.6.6.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/PKG-INFO` & `roblox-pyc-1.6.6.5a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 1.6.6.5.4
+Version: 1.6.6.5a0
 Summary: A Python, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox-pyc
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # roblox.pyc
```

### Comparing `roblox-pyc-1.6.6.5.4/README.md` & `roblox-pyc-1.6.6.5a0/README.md`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/roblox_pyc.egg-info/PKG-INFO` & `roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 1.6.6.5.4
+Version: 1.6.6.5a0
 Summary: A Python, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox-pyc
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # roblox.pyc
```

### Comparing `roblox-pyc-1.6.6.5.4/roblox_pyc.egg-info/SOURCES.txt` & `roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/src/binopdesc.py` & `roblox-pyc-1.6.6.5a0/src/binopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/src/colortext.py` & `roblox-pyc-1.6.6.5a0/src/colortext.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/src/config.py` & `roblox-pyc-1.6.6.5a0/src/config.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/src/context.py` & `roblox-pyc-1.6.6.5a0/src/context.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/src/luainit.py` & `roblox-pyc-1.6.6.5a0/src/luainit.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/src/nodevisitor.py` & `roblox-pyc-1.6.6.5a0/src/nodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/src/pytranslator.py` & `roblox-pyc-1.6.6.5a0/src/pytranslator.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/src/robloxpy.py` & `roblox-pyc-1.6.6.5a0/src/robloxpy.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/src/symbolsstack.py` & `roblox-pyc-1.6.6.5a0/src/symbolsstack.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5.4/src/unaryopdesc.py` & `roblox-pyc-1.6.6.5a0/src/unaryopdesc.py`

 * *Files identical despite different names*

