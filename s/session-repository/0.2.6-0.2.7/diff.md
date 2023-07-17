# Comparing `tmp/session-repository-0.2.6.tar.gz` & `tmp/session-repository-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.2.6.tar", last modified: Mon Jul 17 19:09:22 2023, max compression
+gzip compressed data, was "session-repository-0.2.7.tar", last modified: Mon Jul 17 19:22:12 2023, max compression
```

## Comparing `session-repository-0.2.6.tar` & `session-repository-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 19:09:22.395529 session-repository-0.2.6/
--rw-rw-rw-   0        0        0      599 2023-07-17 19:09:22.384945 session-repository-0.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 19:09:22.328711 session-repository-0.2.6/session_repository/
--rw-rw-rw-   0        0        0     7747 2023-07-17 19:08:15.000000 session-repository-0.2.6/session_repository/core.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.6/session_repository/enum.py
--rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.2.6/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:09:22.378128 session-repository-0.2.6/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-17 19:09:22.000000 session-repository-0.2.6/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-17 19:09:22.000000 session-repository-0.2.6/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 19:09:22.000000 session-repository-0.2.6/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 19:09:22.000000 session-repository-0.2.6/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 19:09:22.000000 session-repository-0.2.6/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 19:09:22.396528 session-repository-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-17 19:01:10.000000 session-repository-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:22:12.758985 session-repository-0.2.7/
+-rw-rw-rw-   0        0        0      599 2023-07-17 19:22:12.753290 session-repository-0.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 19:22:12.690904 session-repository-0.2.7/session_repository/
+-rw-rw-rw-   0        0        0     7787 2023-07-17 19:19:07.000000 session-repository-0.2.7/session_repository/core.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.7/session_repository/enum.py
+-rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.2.7/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:22:12.746919 session-repository-0.2.7/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-17 19:22:12.000000 session-repository-0.2.7/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-17 19:22:12.000000 session-repository-0.2.7/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 19:22:12.000000 session-repository-0.2.7/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 19:22:12.000000 session-repository-0.2.7/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 19:22:12.000000 session-repository-0.2.7/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 19:22:12.766781 session-repository-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-17 19:20:25.000000 session-repository-0.2.7/setup.py
```

### Comparing `session-repository-0.2.6/PKG-INFO` & `session-repository-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.6
+Version: 0.2.7
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.6.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.7.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.6/session_repository/core.py` & `session-repository-0.2.7/session_repository/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Tuple,
     Union,
+    TypeVar
 )
 
 # SQLALCHEMY
 from sqlalchemy.orm import Session, InstrumentedAttribute, Query
 
 # UTILS
 from session_repository.utils import (
@@ -281,18 +282,19 @@
             current_session.flush()
         if commit:
             current_session.commit()
 
         return True
 
 
+T = TypeVar("T", bound=SessionRepository)
 class SessionService:
     def __init__(
         self,
-        repository: SessionRepository,
+        repository: T,
         logger: Logger,
     ) -> None:
         self._repository = repository
         self._logger = logger
 
     def session_manager(self):
         return self._repository.session_manager()
```

### Comparing `session-repository-0.2.6/session_repository/enum.py` & `session-repository-0.2.7/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.6/session_repository/utils.py` & `session-repository-0.2.7/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.6/session_repository.egg-info/PKG-INFO` & `session-repository-0.2.7/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.6
+Version: 0.2.7
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.6.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.7.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.6/setup.py` & `session-repository-0.2.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.6"
+version = "0.2.7"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

