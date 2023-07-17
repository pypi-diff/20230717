# Comparing `tmp/suanpan-sprt-0.6.1.tar.gz` & `tmp/suanpan-sprt-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.6.1.tar", last modified: Wed Jul 12 09:43:26 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.6.2.tar", last modified: Mon Jul 17 07:00:32 2023, max compression
```

## Comparing `suanpan-sprt-0.6.1.tar` & `suanpan-sprt-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-06-02 08:38:14.000000 suanpan-sprt-0.6.1/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.6.1/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.6.1/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4249 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.6.1/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.6.1/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5622 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2082 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.6.1/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6628 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:06:17.000000 suanpan-sprt-0.6.1/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-06-02 08:38:14.000000 suanpan-sprt-0.6.1/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-12 09:25:29.000000 suanpan-sprt-0.6.1/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-12 09:43:26.000000 suanpan-sprt-0.6.1/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4249 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5713 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.2/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2087 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.2/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6628 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.2/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.6.1/setup.py` & `suanpan-sprt-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.1/sprt/__main__.py` & `suanpan-sprt-0.6.2/sprt/__main__.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.1/sprt/arguments.py` & `suanpan-sprt-0.6.2/sprt/arguments.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.1/sprt/envs.py` & `suanpan-sprt-0.6.2/sprt/envs.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.1/sprt/loader.py` & `suanpan-sprt-0.6.2/sprt/loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import logging
 import inspect
-import os
 import pathlib
 import importlib
 import importlib.util
 from .arguments import init_arg_from_arg_spec, init_return_from_value, DEFAULT_DATA_SUBTYPE_ARGS_MAP
 from .storage import Storage
 from .exceptions import ParamsArgError, InvocationFunctionError
 from .log import NodeStreamHandler, LogkitHandler
@@ -18,14 +17,17 @@
         self.location = pathlib.Path(working_dir) / filename
         self.function = function
         self.module = self.load_module()
         self.context = RuntimeContext(user_id, app_id, node_id)
         self.input_arguments = []
         self.has_context = False
         self.load_validator()
+        self._logkit = self._init_logkit(app_id, node_id)
+        self.context.log = self._logkit
+        self._logkit_handler = None
 
     def load_module(self):
         if not self.location.is_file():
             raise Exception(f'invalid component file: {self.location}')
 
         spec = importlib.util.spec_from_file_location(self.name, self.location)
         if spec is None:
@@ -86,68 +88,66 @@
                         for index, r in enumerate(ret)}
             else:
                 return {'out1': init_return_from_value(ret, arg_spec, 0)(f'out{1}', request_id=request_id).save(ret)}
         except Exception as e:
             raise InvocationFunctionError(f'call function: {e}')
 
     def update_logkit(self, logkit=None):
-        self.context.update_logkit(logkit)
-
-    def __del__(self):
-        # os.remove(self.location)
-        pass
-
-
-class RuntimeContext(object):
-    def __init__(self, user_id, app_id, node_id):
-        self.request_id = None
-        self.user_id = user_id
-        self.app_id = app_id
-        self.node_id = node_id
-        self.params = NodeParams()
-        self.log = self._init_log()
-        self.storage = Storage.get_instance()
-        self._logkit_handler = None
-
-    def reset(self, request_id, params):
-        self.request_id = request_id
-        if not isinstance(params, dict):
-            params = json.loads(params)
-        self.params._data = params
-
-    def update_logkit(self, logkit):
         if logkit is None:
-            self.log.removeHandler(self._logkit_handler)
+            self._logkit.removeHandler(self._logkit_handler)
         else:
             if self._logkit_handler and logkit.uri != self._logkit_handler.uri:
-                self.log.removeHandler(self._logkit_handler)
+                self._logkit.removeHandler(self._logkit_handler)
                 self._logkit_handler = None
 
             if self._logkit_handler is None:
                 lh = LogkitHandler(logkit.uri, logkit.namespace, logkit.path, logkit.events_append)
                 lh.setLevel('INFO')
-                self.log.addHandler(lh)
+                self._logkit.addHandler(lh)
                 self._logkit_handler = lh
-                self.log.setLevel(logkit.logs_level.upper())
+                self._logkit.setLevel(logkit.logs_level.upper())
 
-    def _init_log(self):
-        name = f'logkit_{self.app_id}_{self.node_id}'
+    @staticmethod
+    def _init_logkit(app_id, node_id):
+        name = f'logkit_{app_id}_{node_id}'
         logger = logging.getLogger(name)
+        logger.propagate = False
 
         if len(logger.handlers) > 0:
             return logger
 
         formatter = logging.Formatter('%(asctime)s :: [%(levelname)-8s] %(message)s')
         sh = NodeStreamHandler()
         sh.setLevel('DEBUG')
         sh.setFormatter(formatter)
         logger.addHandler(sh)
 
         return logger
 
+    def __del__(self):
+        # os.remove(self.location)
+        self._logkit.handlers.clear()
+
+
+class RuntimeContext(object):
+    def __init__(self, user_id, app_id, node_id):
+        self.request_id = None
+        self.user_id = user_id
+        self.app_id = app_id
+        self.node_id = node_id
+        self.params = NodeParams()
+        self.log = None
+        self.storage = Storage.get_instance()
+
+    def reset(self, request_id, params):
+        self.request_id = request_id
+        if not isinstance(params, dict):
+            params = json.loads(params)
+        self.params._data = params
+
     def __repr__(self):
         return f'<Context: request_id {self.request_id}>'
 
 
 class NodeParams(object):
     def __init__(self):
         self._data = {}
```

### Comparing `suanpan-sprt-0.6.1/sprt/log.py` & `suanpan-sprt-0.6.2/sprt/log.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     @staticmethod
     def make_pickle(record):
         app = envs.appId
         extra = {"node": envs.nodeId}
         data = (app,
                 {
                     "level": record.levelname,
-                    "title": record.message,
+                    "title": record.getMessage(),
                     "data": extra,
                     "time": datetime.now(timezone.utc).isoformat(),
                 })
         return data
 
     def emit(self, record):
         if not self.uri:
```

### Comparing `suanpan-sprt-0.6.1/sprt/master.py` & `suanpan-sprt-0.6.2/sprt/master.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.1/sprt/server.py` & `suanpan-sprt-0.6.2/sprt/server.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.1/sprt/storage.py` & `suanpan-sprt-0.6.2/sprt/storage.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.1/sprt/testing.py` & `suanpan-sprt-0.6.2/sprt/testing.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.1/sprt/utils.py` & `suanpan-sprt-0.6.2/sprt/utils.py`

 * *Files identical despite different names*

