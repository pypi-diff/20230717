# Comparing `tmp/ICICONSOLE-0.2.0.tar.gz` & `tmp/ICICONSOLE-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.2.0.tar", last modified: Mon Jul 17 20:27:44 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.3.0.tar", last modified: Mon Jul 17 20:31:48 2023, max compression
```

## Comparing `ICICONSOLE-0.2.0.tar` & `ICICONSOLE-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:27:44.869900 ICICONSOLE-0.2.0/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:27:44.868516 ICICONSOLE-0.2.0/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1076 2023-07-03 21:32:23.000000 ICICONSOLE-0.2.0/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1276 2023-07-03 20:46:08.000000 ICICONSOLE-0.2.0/ICICONSOLE/Utilities.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLE-0.2.0/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)    12164 2023-07-17 20:26:47.000000 ICICONSOLE-0.2.0/ICICONSOLE/__main__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLE-0.2.0/ICICONSOLE/helpCypher.json
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:27:44.869473 ICICONSOLE-0.2.0/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43999 2023-07-17 20:27:44.000000 ICICONSOLE-0.2.0/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      381 2023-07-17 20:27:44.000000 ICICONSOLE-0.2.0/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-07-17 20:27:44.000000 ICICONSOLE-0.2.0/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-07-17 20:27:44.000000 ICICONSOLE-0.2.0/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       41 2023-07-17 20:27:44.000000 ICICONSOLE-0.2.0/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-07-17 20:27:44.000000 ICICONSOLE-0.2.0/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-07-17 20:04:48.000000 ICICONSOLE-0.2.0/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-07-17 20:04:54.000000 ICICONSOLE-0.2.0/MANIFEST.in
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43999 2023-07-17 20:27:44.869740 ICICONSOLE-0.2.0/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     2871 2023-07-17 20:22:30.000000 ICICONSOLE-0.2.0/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)      925 2023-07-17 20:27:38.000000 ICICONSOLE-0.2.0/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-07-17 20:27:44.869938 ICICONSOLE-0.2.0/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:31:48.632325 ICICONSOLE-0.3.0/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:31:48.631047 ICICONSOLE-0.3.0/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1076 2023-07-03 21:32:23.000000 ICICONSOLE-0.3.0/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1276 2023-07-03 20:46:08.000000 ICICONSOLE-0.3.0/ICICONSOLE/Utilities.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLE-0.3.0/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    12164 2023-07-17 20:26:47.000000 ICICONSOLE-0.3.0/ICICONSOLE/__main__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLE-0.3.0/ICICONSOLE/helpCypher.json
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:31:48.631974 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43864 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      381 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       41 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-07-17 20:04:48.000000 ICICONSOLE-0.3.0/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-07-17 20:04:54.000000 ICICONSOLE-0.3.0/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43864 2023-07-17 20:31:48.632197 ICICONSOLE-0.3.0/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     2736 2023-07-17 20:31:24.000000 ICICONSOLE-0.3.0/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      925 2023-07-17 20:31:37.000000 ICICONSOLE-0.3.0/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-07-17 20:31:48.632365 ICICONSOLE-0.3.0/setup.cfg
```

### Comparing `ICICONSOLE-0.2.0/ICICONSOLE/BasicCypherCommands.py` & `ICICONSOLE-0.3.0/ICICONSOLE/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.2.0/ICICONSOLE/Utilities.py` & `ICICONSOLE-0.3.0/ICICONSOLE/Utilities.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.2.0/ICICONSOLE/__main__.py` & `ICICONSOLE-0.3.0/ICICONSOLE/__main__.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.2.0/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.3.0/ICICONSOLE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.2.0
+Version: 0.3.0
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,17 +684,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# ICICONSOLE PROD DETAILS
+# ICICONSOLE
 
-**Note: ICICONSOLEGPT is NOT in PROD, and it is currently in development. For details, see the ICICONSOLEGPT README.md.**
 
 ## Overview
 
 ICICONSOLE is designed to provide an efficient and powerful interface to Neo4j Knowledge Graph databases hosted on HPC resources, leveraging Tapis. 
 
 This application is specialized for knowledge graph querying, and has some basic CYPHER commands built in.
```

### Comparing `ICICONSOLE-0.2.0/LICENSE` & `ICICONSOLE-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.2.0/PKG-INFO` & `ICICONSOLE-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.2.0
+Version: 0.3.0
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,17 +684,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# ICICONSOLE PROD DETAILS
+# ICICONSOLE
 
-**Note: ICICONSOLEGPT is NOT in PROD, and it is currently in development. For details, see the ICICONSOLEGPT README.md.**
 
 ## Overview
 
 ICICONSOLE is designed to provide an efficient and powerful interface to Neo4j Knowledge Graph databases hosted on HPC resources, leveraging Tapis. 
 
 This application is specialized for knowledge graph querying, and has some basic CYPHER commands built in.
```

### Comparing `ICICONSOLE-0.2.0/README.md` & `ICICONSOLE-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# ICICONSOLE PROD DETAILS
+# ICICONSOLE
 
-**Note: ICICONSOLEGPT is NOT in PROD, and it is currently in development. For details, see the ICICONSOLEGPT README.md.**
 
 ## Overview
 
 ICICONSOLE is designed to provide an efficient and powerful interface to Neo4j Knowledge Graph databases hosted on HPC resources, leveraging Tapis. 
 
 This application is specialized for knowledge graph querying, and has some basic CYPHER commands built in.
```

### Comparing `ICICONSOLE-0.2.0/pyproject.toml` & `ICICONSOLE-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE"
-version = "0.2.0"
+version = "0.3.0"
 description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

