# Comparing `tmp/session-repository-0.2.5.tar.gz` & `tmp/session-repository-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.2.5.tar", last modified: Thu Jul 13 16:52:56 2023, max compression
+gzip compressed data, was "session-repository-0.2.6.tar", last modified: Mon Jul 17 19:09:22 2023, max compression
```

## Comparing `session-repository-0.2.5.tar` & `session-repository-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 16:52:56.484063 session-repository-0.2.5/
--rw-rw-rw-   0        0        0      599 2023-07-13 16:52:56.480840 session-repository-0.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 16:52:56.456909 session-repository-0.2.5/session_repository/
--rw-rw-rw-   0        0        0     9287 2023-07-07 14:12:40.000000 session-repository-0.2.5/session_repository/core.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.5/session_repository/enum.py
--rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.2.5/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:52:56.476840 session-repository-0.2.5/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-13 16:52:56.000000 session-repository-0.2.5/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-13 16:52:56.000000 session-repository-0.2.5/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 16:52:56.000000 session-repository-0.2.5/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-13 16:52:56.000000 session-repository-0.2.5/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-13 16:52:56.000000 session-repository-0.2.5/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 16:52:56.485065 session-repository-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-13 16:52:37.000000 session-repository-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:09:22.395529 session-repository-0.2.6/
+-rw-rw-rw-   0        0        0      599 2023-07-17 19:09:22.384945 session-repository-0.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 19:09:22.328711 session-repository-0.2.6/session_repository/
+-rw-rw-rw-   0        0        0     7747 2023-07-17 19:08:15.000000 session-repository-0.2.6/session_repository/core.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.6/session_repository/enum.py
+-rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.2.6/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:09:22.378128 session-repository-0.2.6/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-17 19:09:22.000000 session-repository-0.2.6/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-17 19:09:22.000000 session-repository-0.2.6/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 19:09:22.000000 session-repository-0.2.6/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 19:09:22.000000 session-repository-0.2.6/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 19:09:22.000000 session-repository-0.2.6/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 19:09:22.396528 session-repository-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-17 19:01:10.000000 session-repository-0.2.6/setup.py
```

### Comparing `session-repository-0.2.5/PKG-INFO` & `session-repository-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.5
+Version: 0.2.6
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.5.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.5/session_repository/enum.py` & `session-repository-0.2.6/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.5/session_repository/utils.py` & `session-repository-0.2.6/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.5/session_repository.egg-info/PKG-INFO` & `session-repository-0.2.6/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.5
+Version: 0.2.6
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.5.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.5/setup.py` & `session-repository-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.5"
+version = "0.2.6"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

