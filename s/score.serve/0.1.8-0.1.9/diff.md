# Comparing `tmp/score.serve-0.1.8.tar.gz` & `tmp/score.serve-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/score.serve-0.1.8.tar", last modified: Fri Nov 11 15:20:31 2016, max compression
+gzip compressed data, was "dist/score.serve-0.1.9.tar", last modified: Tue Dec 13 08:19:19 2016, max compression
```

## Comparing `score.serve-0.1.8.tar` & `score.serve-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 soulmerge  (1000) soulmerge  (1000)        0 2016-11-11 15:20:31.000000 score.serve-0.1.8/
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     2707 2016-11-11 15:20:25.000000 score.serve-0.1.8/setup.py
-drwxr-xr-x   0 soulmerge  (1000) soulmerge  (1000)        0 2016-11-11 15:20:31.000000 score.serve-0.1.8/score.serve.egg-info/
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)       42 2016-11-11 15:20:31.000000 score.serve-0.1.8/score.serve.egg-info/entry_points.txt
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)      620 2016-11-11 15:20:31.000000 score.serve-0.1.8/score.serve.egg-info/SOURCES.txt
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)        1 2016-11-03 12:05:13.000000 score.serve-0.1.8/score.serve.egg-info/not-zip-safe
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)        1 2016-11-11 15:20:31.000000 score.serve-0.1.8/score.serve.egg-info/dependency_links.txt
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)        6 2016-11-11 15:20:31.000000 score.serve-0.1.8/score.serve.egg-info/namespace_packages.txt
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     2909 2016-11-11 15:20:31.000000 score.serve-0.1.8/score.serve.egg-info/PKG-INFO
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)       35 2016-11-11 15:20:31.000000 score.serve-0.1.8/score.serve.egg-info/requires.txt
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)        6 2016-11-11 15:20:31.000000 score.serve-0.1.8/score.serve.egg-info/top_level.txt
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)       59 2016-11-11 15:20:31.000000 score.serve-0.1.8/setup.cfg
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     1744 2016-10-28 06:40:35.000000 score.serve-0.1.8/README.rst
-drwxr-xr-x   0 soulmerge  (1000) soulmerge  (1000)        0 2016-11-11 15:20:31.000000 score.serve-0.1.8/score/
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)      200 2016-10-28 06:40:35.000000 score.serve-0.1.8/score/__init__.py
-drwxr-xr-x   0 soulmerge  (1000) soulmerge  (1000)        0 2016-11-11 15:20:31.000000 score.serve-0.1.8/score/serve/
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     2170 2016-10-28 06:40:35.000000 score.serve-0.1.8/score/serve/cli.py
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     4557 2016-10-28 06:40:35.000000 score.serve-0.1.8/score/serve/_forked.py
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     1674 2016-11-11 15:20:25.000000 score.serve-0.1.8/score/serve/__init__.py
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     6977 2016-10-28 06:40:35.000000 score.serve-0.1.8/score/serve/_changedetect.py
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)    11659 2016-11-10 14:28:00.000000 score.serve-0.1.8/score/serve/_init.py
-drwxr-xr-x   0 soulmerge  (1000) soulmerge  (1000)        0 2016-11-11 15:20:31.000000 score.serve-0.1.8/score/serve/worker/
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     3521 2016-10-28 06:40:35.000000 score.serve-0.1.8/score/serve/worker/socketserver.py
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)      256 2016-11-03 13:45:39.000000 score.serve-0.1.8/score/serve/worker/__init__.py
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     4478 2016-10-28 06:40:35.000000 score.serve-0.1.8/score/serve/worker/worker.py
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     5038 2016-11-10 14:15:06.000000 score.serve-0.1.8/score/serve/worker/asyncio.py
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     1314 2016-10-28 06:40:35.000000 score.serve-0.1.8/score/serve/worker/simple.py
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     7002 2016-10-28 06:40:35.000000 score.serve-0.1.8/score/serve/service.py
--rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     2909 2016-11-11 15:20:31.000000 score.serve-0.1.8/PKG-INFO
+drwxr-xr-x   0 soulmerge  (1000) soulmerge  (1000)        0 2016-12-13 08:19:19.000000 score.serve-0.1.9/
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     2707 2016-12-13 08:18:58.000000 score.serve-0.1.9/setup.py
+drwxr-xr-x   0 soulmerge  (1000) soulmerge  (1000)        0 2016-12-13 08:19:19.000000 score.serve-0.1.9/score.serve.egg-info/
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)       42 2016-12-13 08:19:19.000000 score.serve-0.1.9/score.serve.egg-info/entry_points.txt
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)      650 2016-12-13 08:19:19.000000 score.serve-0.1.9/score.serve.egg-info/SOURCES.txt
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)        1 2016-10-19 08:03:53.000000 score.serve-0.1.9/score.serve.egg-info/not-zip-safe
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)        1 2016-12-13 08:19:19.000000 score.serve-0.1.9/score.serve.egg-info/dependency_links.txt
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)        6 2016-12-13 08:19:19.000000 score.serve-0.1.9/score.serve.egg-info/namespace_packages.txt
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     2909 2016-12-13 08:19:19.000000 score.serve-0.1.9/score.serve.egg-info/PKG-INFO
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)       35 2016-12-13 08:19:19.000000 score.serve-0.1.9/score.serve.egg-info/requires.txt
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)        6 2016-12-13 08:19:19.000000 score.serve-0.1.9/score.serve.egg-info/top_level.txt
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)      702 2016-09-12 14:44:08.000000 score.serve-0.1.9/.gitignore
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)       59 2016-12-13 08:19:19.000000 score.serve-0.1.9/setup.cfg
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     1744 2016-10-19 08:03:47.000000 score.serve-0.1.9/README.rst
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)    42870 2016-09-12 14:44:08.000000 score.serve-0.1.9/COPYING.LESSER.txt
+drwxr-xr-x   0 soulmerge  (1000) soulmerge  (1000)        0 2016-12-13 08:19:19.000000 score.serve-0.1.9/score/
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)      200 2016-09-12 14:44:08.000000 score.serve-0.1.9/score/__init__.py
+drwxr-xr-x   0 soulmerge  (1000) soulmerge  (1000)        0 2016-12-13 08:19:19.000000 score.serve-0.1.9/score/serve/
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     2170 2016-10-19 08:03:47.000000 score.serve-0.1.9/score/serve/cli.py
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     4557 2016-10-18 14:48:10.000000 score.serve-0.1.9/score/serve/_forked.py
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     1674 2016-12-13 08:18:58.000000 score.serve-0.1.9/score/serve/__init__.py
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     6977 2016-10-19 08:03:47.000000 score.serve-0.1.9/score/serve/_changedetect.py
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)    11677 2016-12-13 08:17:49.000000 score.serve-0.1.9/score/serve/_init.py
+drwxr-xr-x   0 soulmerge  (1000) soulmerge  (1000)        0 2016-12-13 08:19:19.000000 score.serve-0.1.9/score/serve/worker/
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     3521 2016-10-25 08:01:29.000000 score.serve-0.1.9/score/serve/worker/socketserver.py
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)      256 2016-12-13 08:16:57.000000 score.serve-0.1.9/score/serve/worker/__init__.py
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     4478 2016-10-25 08:01:29.000000 score.serve-0.1.9/score/serve/worker/worker.py
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     5038 2016-12-13 08:16:57.000000 score.serve-0.1.9/score/serve/worker/asyncio.py
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     1314 2016-10-25 08:01:29.000000 score.serve-0.1.9/score/serve/worker/simple.py
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     7002 2016-10-25 08:01:29.000000 score.serve-0.1.9/score/serve/service.py
+-rw-r--r--   0 soulmerge  (1000) soulmerge  (1000)     2909 2016-12-13 08:19:19.000000 score.serve-0.1.9/PKG-INFO
```

### Comparing `score.serve-0.1.8/setup.py` & `score.serve-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'README.rst')) as f:
     README = f.read()
 
 setup(
     name='score.serve',
-    version='0.1.8',
+    version='0.1.9',
     description='Application server of The SCORE Framework',
     long_description=README,
     author='strg.at',
     author_email='score@strg.at',
     url='http://score-framework.org',
     keywords='score framework server',
     packages=['score', 'score.serve', 'score.serve.worker'],
```

### Comparing `score.serve-0.1.8/score.serve.egg-info/SOURCES.txt` & `score.serve-0.1.9/score.serve.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.gitignore
+COPYING.LESSER.txt
 README.rst
 setup.py
 score/__init__.py
 score.serve.egg-info/PKG-INFO
 score.serve.egg-info/SOURCES.txt
 score.serve.egg-info/dependency_links.txt
 score.serve.egg-info/entry_points.txt
```

### Comparing `score.serve-0.1.8/score.serve.egg-info/PKG-INFO` & `score.serve-0.1.9/score.serve.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: score.serve
-Version: 0.1.8
+Version: 0.1.9
 Summary: Application server of The SCORE Framework
 Home-page: http://score-framework.org
 Author: strg.at
 Author-email: score@strg.at
 License: LGPL
 Description: `The SCORE Framework`_ is a collection of harmonized python and javascript
         libraries for the development of large scale web projects. Powered by strg.at_.
```

### Comparing `score.serve-0.1.8/README.rst` & `score.serve-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `score.serve-0.1.8/score/serve/cli.py` & `score.serve-0.1.9/score/serve/cli.py`

 * *Files identical despite different names*

### Comparing `score.serve-0.1.8/score/serve/_forked.py` & `score.serve-0.1.9/score/serve/_forked.py`

 * *Files identical despite different names*

### Comparing `score.serve-0.1.8/score/serve/__init__.py` & `score.serve-0.1.9/score/serve/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,11 +26,11 @@
 
 
 from ._init import init, ConfiguredServeModule
 from .worker import (
     Worker, SocketServerWorker, SimpleWorker, AsyncioWorker, transitions)
 from .service import Service
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 __all__ = ('init', 'ConfiguredServeModule', 'Worker', 'SocketServerWorker',
            'SimpleWorker', 'AsyncioWorker', 'transitions', 'Service')
```

### Comparing `score.serve-0.1.8/score/serve/_changedetect.py` & `score.serve-0.1.9/score/serve/_changedetect.py`

 * *Files identical despite different names*

### Comparing `score.serve-0.1.8/score/serve/_init.py` & `score.serve-0.1.9/score/serve/_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         return all(state in (Service.State.STOPPED, Service.State.EXCEPTION)
                    for state in states)
 
     def quit_if_stopped(self, states):
         if not self.all_services_stopped(states):
             return
         self.controller.off('state-change', self.quit_if_stopped)
-        self.stop_loop()
+        self.loop.create_task(self.stop())
 
     def restart(self):
         if self.reload is None:
             self.reload = True
         self.loop.create_task(self.stop())
 
     @asyncio.coroutine
```

### Comparing `score.serve-0.1.8/score/serve/worker/socketserver.py` & `score.serve-0.1.9/score/serve/worker/socketserver.py`

 * *Files identical despite different names*

### Comparing `score.serve-0.1.8/score/serve/worker/worker.py` & `score.serve-0.1.9/score/serve/worker/worker.py`

 * *Files identical despite different names*

### Comparing `score.serve-0.1.8/score/serve/worker/asyncio.py` & `score.serve-0.1.9/score/serve/worker/asyncio.py`

 * *Files identical despite different names*

### Comparing `score.serve-0.1.8/score/serve/worker/simple.py` & `score.serve-0.1.9/score/serve/worker/simple.py`

 * *Files identical despite different names*

### Comparing `score.serve-0.1.8/score/serve/service.py` & `score.serve-0.1.9/score/serve/service.py`

 * *Files identical despite different names*

### Comparing `score.serve-0.1.8/PKG-INFO` & `score.serve-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: score.serve
-Version: 0.1.8
+Version: 0.1.9
 Summary: Application server of The SCORE Framework
 Home-page: http://score-framework.org
 Author: strg.at
 Author-email: score@strg.at
 License: LGPL
 Description: `The SCORE Framework`_ is a collection of harmonized python and javascript
         libraries for the development of large scale web projects. Powered by strg.at_.
```

