# Comparing `tmp/htagweb-0.3.1.tar.gz` & `tmp/htagweb-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.3.1.tar", max compression
+gzip compressed data, was "htagweb-0.3.2.tar", max compression
```

## Comparing `htagweb-0.3.1.tar` & `htagweb-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-07-16 16:23:13.148472 htagweb-0.3.1/LICENSE
--rw-r--r--   0        0        0     3148 2023-07-16 16:23:13.148472 htagweb-0.3.1/README.md
--rw-r--r--   0        0        0     9938 2023-07-16 16:23:13.520501 htagweb-0.3.1/htagweb/__init__.py
--rw-r--r--   0        0        0     2225 2023-07-16 16:23:13.148472 htagweb-0.3.1/htagweb/crypto.py
--rw-r--r--   0        0        0     3732 2023-07-16 16:23:13.148472 htagweb-0.3.1/htagweb/manager.py
--rw-r--r--   0        0        0     5152 2023-07-16 16:23:13.148472 htagweb-0.3.1/htagweb/uidprocess.py
--rw-r--r--   0        0        0     1124 2023-07-16 16:23:13.520501 htagweb-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 htagweb-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-17 13:00:40.710421 htagweb-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3148 2023-07-17 13:00:40.710421 htagweb-0.3.2/README.md
+-rw-r--r--   0        0        0     9938 2023-07-17 13:00:41.018432 htagweb-0.3.2/htagweb/__init__.py
+-rw-r--r--   0        0        0     2225 2023-07-17 13:00:40.710421 htagweb-0.3.2/htagweb/crypto.py
+-rw-r--r--   0        0        0     3732 2023-07-17 13:00:40.710421 htagweb-0.3.2/htagweb/manager.py
+-rw-r--r--   0        0        0     5541 2023-07-17 13:00:40.710421 htagweb-0.3.2/htagweb/uidprocess.py
+-rw-r--r--   0        0        0     1124 2023-07-17 13:00:41.018432 htagweb-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 htagweb-0.3.2/PKG-INFO
```

### Comparing `htagweb-0.3.1/LICENSE` & `htagweb-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.1/README.md` & `htagweb-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.1/htagweb/__init__.py` & `htagweb-0.3.2/htagweb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.3.1" # auto updated
+__version__ = "0.3.2" # auto updated
 
 """
 WebServer & WebServerWS
 ~~~~~~~~~~~~~~~~~~~~~~~~
 - new versions of oldest WebHTTP & WebWS (nearly compatibles)
 - concept of an htag app application server (manager), which communicate with child process, with queue
 - Htag Apps runned in a process, per user (real isolation!)
```

### Comparing `htagweb-0.3.1/htagweb/crypto.py` & `htagweb-0.3.2/htagweb/crypto.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.1/htagweb/manager.py` & `htagweb-0.3.2/htagweb/manager.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.1/htagweb/uidprocess.py` & `htagweb-0.3.2/htagweb/uidprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # #############################################################################
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
-import asyncio
+import asyncio,sys
 import multiprocessing
 import logging,importlib
 from htag.render import HRenderer
 from shared_memory_dict import SharedMemoryDict
 
 logger = logging.getLogger(__name__)
 
@@ -34,16 +34,24 @@
             hr=HTS.get(fqn)
             if renew or (hr is None) or str(init_params)!=str(hr.init):
                 ##HRenderer(tagClass: type, js:str, exit_callback:Optional[Callable]=None, init= ((),{}), fullerror=False, statics=[], session=None ):
 
                 #--------------------------- fqn -> module, name
                 names = fqn.split(".")
                 modulename,name=".".join(names[:-1]), names[-1]
-                module=importlib.import_module(modulename)
-                module=importlib.reload(module)
+                if modulename in sys.modules:
+                    module=sys.modules[modulename]
+                    try:
+                        module=importlib.reload( module )
+                    except ModuleNotFoundError:
+                        """ can't be (really) reloaded if the component is in the 
+                        same module as the instance htag server"""
+                        pass
+                else:
+                    module=importlib.import_module(modulename)
                 #---------------------------
                 htClass = getattr(module,name)
 
 
                 hr=HRenderer( htClass,
                         js=js,
                         session=session,
```

### Comparing `htagweb-0.3.1/pyproject.toml` & `htagweb-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.3.1" # auto-updated
+version = "0.3.2" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
```

### Comparing `htagweb-0.3.1/PKG-INFO` & `htagweb-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.3.1
+Version: 0.3.2
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.8,<4.0
```

