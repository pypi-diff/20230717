# Comparing `tmp/ICICONSOLE-0.3.0.tar.gz` & `tmp/ICICONSOLE-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.3.0.tar", last modified: Mon Jul 17 20:31:48 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.4.0.tar", last modified: Mon Jul 17 20:39:33 2023, max compression
```

## Comparing `ICICONSOLE-0.3.0.tar` & `ICICONSOLE-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:31:48.632325 ICICONSOLE-0.3.0/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:31:48.631047 ICICONSOLE-0.3.0/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1076 2023-07-03 21:32:23.000000 ICICONSOLE-0.3.0/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1276 2023-07-03 20:46:08.000000 ICICONSOLE-0.3.0/ICICONSOLE/Utilities.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLE-0.3.0/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)    12164 2023-07-17 20:26:47.000000 ICICONSOLE-0.3.0/ICICONSOLE/__main__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLE-0.3.0/ICICONSOLE/helpCypher.json
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:31:48.631974 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43864 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      381 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       41 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-07-17 20:31:48.000000 ICICONSOLE-0.3.0/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-07-17 20:04:48.000000 ICICONSOLE-0.3.0/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-07-17 20:04:54.000000 ICICONSOLE-0.3.0/MANIFEST.in
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43864 2023-07-17 20:31:48.632197 ICICONSOLE-0.3.0/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     2736 2023-07-17 20:31:24.000000 ICICONSOLE-0.3.0/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)      925 2023-07-17 20:31:37.000000 ICICONSOLE-0.3.0/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-07-17 20:31:48.632365 ICICONSOLE-0.3.0/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:39:33.460290 ICICONSOLE-0.4.0/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:39:33.459034 ICICONSOLE-0.4.0/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1076 2023-07-03 21:32:23.000000 ICICONSOLE-0.4.0/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1276 2023-07-03 20:46:08.000000 ICICONSOLE-0.4.0/ICICONSOLE/Utilities.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLE-0.4.0/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    12164 2023-07-17 20:26:47.000000 ICICONSOLE-0.4.0/ICICONSOLE/__main__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLE-0.4.0/ICICONSOLE/helpCypher.json
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-17 20:39:33.459910 ICICONSOLE-0.4.0/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    44423 2023-07-17 20:39:33.000000 ICICONSOLE-0.4.0/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      381 2023-07-17 20:39:33.000000 ICICONSOLE-0.4.0/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-07-17 20:39:33.000000 ICICONSOLE-0.4.0/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-07-17 20:39:33.000000 ICICONSOLE-0.4.0/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       41 2023-07-17 20:39:33.000000 ICICONSOLE-0.4.0/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-07-17 20:39:33.000000 ICICONSOLE-0.4.0/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-07-17 20:04:48.000000 ICICONSOLE-0.4.0/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-07-17 20:04:54.000000 ICICONSOLE-0.4.0/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    44423 2023-07-17 20:39:33.460148 ICICONSOLE-0.4.0/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     3295 2023-07-17 20:38:58.000000 ICICONSOLE-0.4.0/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      925 2023-07-17 20:39:21.000000 ICICONSOLE-0.4.0/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-07-17 20:39:33.460326 ICICONSOLE-0.4.0/setup.cfg
```

### Comparing `ICICONSOLE-0.3.0/ICICONSOLE/BasicCypherCommands.py` & `ICICONSOLE-0.4.0/ICICONSOLE/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.3.0/ICICONSOLE/Utilities.py` & `ICICONSOLE-0.4.0/ICICONSOLE/Utilities.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.3.0/ICICONSOLE/__main__.py` & `ICICONSOLE-0.4.0/ICICONSOLE/__main__.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.3.0/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.4.0/ICICONSOLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.3.0
+Version: 0.4.0
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -741,24 +741,31 @@
 
 ### First time user setup
 
 You have two options as of now: connecting to a Neo4j database hosted on a Tapis Pod at the Texas Advanced Computing Center, or downloading Neo4j Desktop and connecting to a database that you are running locally. 
 
 #### Tapis
 
-You will be asked to login with your TACC account. If you aren't sure if you have this, visit the TACC [portal](https://portal.tacc.utexas.edu/).
+When prompted to change authentication type from Tapis, enter "n". It will then present the default ICICLE base url for tapis, which you can modify by typing "y" to the prompt to change base url. 
+
+You will then be asked to login with your TACC account. If you aren't sure if you have this, visit the TACC [portal](https://portal.tacc.utexas.edu/).
 
 Once you enter your username and password to ICICONSOLE, you will see the Tapis Pods that you have been given permission to access. If you don't see any, please contact the owner of the Pod you wish to access. Type in the ID of the Pod that you want to access. 
 
 #### Local
-
 If you are running a Neo4j database locally, you will need to download Neo4j Desktop. You can download it [here](https://neo4j.com/download/).
 
 Next, you have to run a local dbms. This should be running by default on bolt port 7687, which is what ICICONSOLE will try to connect to. 
 
+In ICICONSOLE, when prompted to change authentication type from Tapis, enter "y". Then type "local". 
+
+Next, enter any username and graph name; this is just for personalization in the application and not needed for authentication. 
+
+The graph password, however, is important. This is the password that you set within Neo4j Desktop for your local database.
+
 
 ### First time usage guide
 
 Once you access either a Tapis Pod or your local database, you will be in a custom made console for interfacing with your Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
 
 ```
 MATCH(n) RETURN n LIMIT 10
```

### Comparing `ICICONSOLE-0.3.0/LICENSE` & `ICICONSOLE-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.3.0/PKG-INFO` & `ICICONSOLE-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.3.0
+Version: 0.4.0
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -741,24 +741,31 @@
 
 ### First time user setup
 
 You have two options as of now: connecting to a Neo4j database hosted on a Tapis Pod at the Texas Advanced Computing Center, or downloading Neo4j Desktop and connecting to a database that you are running locally. 
 
 #### Tapis
 
-You will be asked to login with your TACC account. If you aren't sure if you have this, visit the TACC [portal](https://portal.tacc.utexas.edu/).
+When prompted to change authentication type from Tapis, enter "n". It will then present the default ICICLE base url for tapis, which you can modify by typing "y" to the prompt to change base url. 
+
+You will then be asked to login with your TACC account. If you aren't sure if you have this, visit the TACC [portal](https://portal.tacc.utexas.edu/).
 
 Once you enter your username and password to ICICONSOLE, you will see the Tapis Pods that you have been given permission to access. If you don't see any, please contact the owner of the Pod you wish to access. Type in the ID of the Pod that you want to access. 
 
 #### Local
-
 If you are running a Neo4j database locally, you will need to download Neo4j Desktop. You can download it [here](https://neo4j.com/download/).
 
 Next, you have to run a local dbms. This should be running by default on bolt port 7687, which is what ICICONSOLE will try to connect to. 
 
+In ICICONSOLE, when prompted to change authentication type from Tapis, enter "y". Then type "local". 
+
+Next, enter any username and graph name; this is just for personalization in the application and not needed for authentication. 
+
+The graph password, however, is important. This is the password that you set within Neo4j Desktop for your local database.
+
 
 ### First time usage guide
 
 Once you access either a Tapis Pod or your local database, you will be in a custom made console for interfacing with your Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
 
 ```
 MATCH(n) RETURN n LIMIT 10
```

### Comparing `ICICONSOLE-0.3.0/README.md` & `ICICONSOLE-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -51,24 +51,31 @@
 
 ### First time user setup
 
 You have two options as of now: connecting to a Neo4j database hosted on a Tapis Pod at the Texas Advanced Computing Center, or downloading Neo4j Desktop and connecting to a database that you are running locally. 
 
 #### Tapis
 
-You will be asked to login with your TACC account. If you aren't sure if you have this, visit the TACC [portal](https://portal.tacc.utexas.edu/).
+When prompted to change authentication type from Tapis, enter "n". It will then present the default ICICLE base url for tapis, which you can modify by typing "y" to the prompt to change base url. 
+
+You will then be asked to login with your TACC account. If you aren't sure if you have this, visit the TACC [portal](https://portal.tacc.utexas.edu/).
 
 Once you enter your username and password to ICICONSOLE, you will see the Tapis Pods that you have been given permission to access. If you don't see any, please contact the owner of the Pod you wish to access. Type in the ID of the Pod that you want to access. 
 
 #### Local
-
 If you are running a Neo4j database locally, you will need to download Neo4j Desktop. You can download it [here](https://neo4j.com/download/).
 
 Next, you have to run a local dbms. This should be running by default on bolt port 7687, which is what ICICONSOLE will try to connect to. 
 
+In ICICONSOLE, when prompted to change authentication type from Tapis, enter "y". Then type "local". 
+
+Next, enter any username and graph name; this is just for personalization in the application and not needed for authentication. 
+
+The graph password, however, is important. This is the password that you set within Neo4j Desktop for your local database.
+
 
 ### First time usage guide
 
 Once you access either a Tapis Pod or your local database, you will be in a custom made console for interfacing with your Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
 
 ```
 MATCH(n) RETURN n LIMIT 10
```

### Comparing `ICICONSOLE-0.3.0/pyproject.toml` & `ICICONSOLE-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE"
-version = "0.3.0"
+version = "0.4.0"
 description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

