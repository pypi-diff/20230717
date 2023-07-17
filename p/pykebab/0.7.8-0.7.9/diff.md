# Comparing `tmp/pykebab-0.7.8.tar.gz` & `tmp/pykebab-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.7.8.tar", max compression
+gzip compressed data, was "pykebab-0.7.9.tar", max compression
```

## Comparing `pykebab-0.7.8.tar` & `pykebab-0.7.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/aws.py
--rw-r--r--   0        0        0       40 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/cli/cli.py
--rw-r--r--   0        0        0      798 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/constants.py
--rw-r--r--   0        0        0       42 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/exceptions.py
--rw-r--r--   0        0        0     2587 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/k8s.py
--rw-r--r--   0        0        0      773 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/loader.py
--rw-r--r--   0        0        0     2368 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/magic.py
--rw-r--r--   0        0        0     2108 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/openers.py
--rw-r--r--   0        0        0    22564 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/utils.py
--rw-r--r--   0        0        0     1025 2023-06-26 04:27:04.825862 pykebab-0.7.8/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      821 2022-11-06 03:32:21.214628 pykebab-0.7.9/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2022-11-06 03:32:21.214802 pykebab-0.7.9/kebab/aws.py
+-rw-r--r--   0        0        0       40 2022-11-06 03:32:21.214897 pykebab-0.7.9/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-01-05 03:45:44.147407 pykebab-0.7.9/kebab/cli/cli.py
+-rw-r--r--   0        0        0      798 2023-02-03 08:02:22.409418 pykebab-0.7.9/kebab/constants.py
+-rw-r--r--   0        0        0       42 2022-11-06 03:32:21.215088 pykebab-0.7.9/kebab/exceptions.py
+-rw-r--r--   0        0        0     2587 2023-01-05 03:45:44.147717 pykebab-0.7.9/kebab/k8s.py
+-rw-r--r--   0        0        0      773 2023-07-14 11:25:15.559702 pykebab-0.7.9/kebab/loader.py
+-rw-r--r--   0        0        0     2368 2023-06-26 02:47:04.851901 pykebab-0.7.9/kebab/magic.py
+-rw-r--r--   0        0        0     2108 2023-07-14 09:08:11.442108 pykebab-0.7.9/kebab/openers.py
+-rw-r--r--   0        0        0    22614 2023-07-14 11:00:17.432224 pykebab-0.7.9/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-01-05 03:45:44.148106 pykebab-0.7.9/kebab/utils.py
+-rw-r--r--   0        0        0     1025 2023-07-14 11:28:34.838114 pykebab-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.7.9/PKG-INFO
```

### Comparing `pykebab-0.7.8/kebab/__init__.py` & `pykebab-0.7.9/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.8/kebab/aws.py` & `pykebab-0.7.9/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.8/kebab/cli/cli.py` & `pykebab-0.7.9/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.8/kebab/constants.py` & `pykebab-0.7.9/kebab/constants.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.8/kebab/k8s.py` & `pykebab-0.7.9/kebab/k8s.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.8/kebab/loader.py` & `pykebab-0.7.9/kebab/loader.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.8/kebab/magic.py` & `pykebab-0.7.9/kebab/magic.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.8/kebab/openers.py` & `pykebab-0.7.9/kebab/openers.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.8/kebab/sources.py` & `pykebab-0.7.9/kebab/sources.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     def __init__(self, **kwargs):
         # Variables for sources reload (first load is also a reload).
         super(KebabSource, self).__init__(**kwargs)
         self._last_reload_timestamp = 0  # type: float
         self._reload_lock = threading.RLock()
         self._reload_timer = None
         self._reload_disabled = threading.Event()
-        self._last_cached_timestamp = 0  # type: float
         self._cached_context = {}
         self._str_loader = YamlLoader()
 
     def __repr__(self):
         return self.__class__.__name__
 
     def __getitem__(self, key):
@@ -95,17 +94,25 @@
         return item in self.get()
 
     def __iter__(self):
         return iter(self.get())
 
     @abc.abstractmethod
     def _load_context(self):
+        """
+        Load the context from the source.
+        This method should be implemented by subclasses.
+        """
         return {}
 
     def _load_context_recursively(self):
+        """
+        Load the context from the source and recursively update the context from
+        the extensions.
+        """
         _logger.debug(f"loading {self}")
 
         _context = self._load_context()
 
         for keyword, extension in KebabSource._context_extensions.items():
             if keyword in _context:
                 extension_context = _context.pop(keyword)
@@ -172,20 +179,16 @@
                 )
                 self._reload_timer.daemon = True
                 self._reload_timer.start()
 
         return self
 
     def _get_context(self):
-        if (
-            not self._cached_context
-            or self._last_cached_timestamp < self.last_reload_timestamp
-        ):
+        if not self._cached_context:
             self.reload()
-            self._last_cached_timestamp = time.time()
 
         return self._cached_context
 
     @property
     def last_reload_timestamp(self):
         return self._last_reload_timestamp
 
@@ -200,27 +203,23 @@
 
         # not thread safe
         class KebabProxy:
             def __init__(self):
                 self.__value = f()
                 self.__last_eval_timestamp = time.time()
 
-            def reload_if_necessary(self):
+            def _reload_getattr(self, name):
                 if self.__last_eval_timestamp < source.last_reload_timestamp:
                     self.__value = f()
                     self.__last_eval_timestamp = time.time()
+                return getattr(self.__value, name)
 
             def __getattr__(self, name):
-                self.reload_if_necessary()
-                ret = getattr(self.__value, name)
-
-                def reloader():
-                    self.reload_if_necessary()
-                    return getattr(self.__value, name)
-                return source.proxy(reloader, type(ret))
+                ret = self._reload_getattr(name)
+                return source.proxy(lambda: self._reload_getattr(name), type(ret))
         return KebabProxy()
 
     @deprecated_alias(default_value="default")
     def get(
         self,
         config_name=".",
         default=None,
@@ -590,14 +589,17 @@
 
     def _load_context(self):
         return self._parent_source.get(
             self._source_name, required=True, expected_type=dict
         )
 
     def _get_context(self):
+        """
+        SubSource never caches, relies on parent source/cache
+        """
         return self._load_context()
 
     @property
     def last_reload_timestamp(self):
         return self._parent_source.last_reload_timestamp
 
 
@@ -661,14 +663,14 @@
 
     if len(sources) == 1:
         # for single url, do not read with union source so that self configured auto
         # reload will work
         source = sources[0]
     else:
         source = UnionSource(sources=sources)
-    source.reload(reload_interval_in_secs=reload_interval_in_secs)
+    source.reload(reload_interval_in_secs=reload_interval_in_secs, skip_first=True)
     return source
 
 
 KebabSource.register_extension(ImportExtension)
 KebabSource.register_extension(EnvVarSource)
 KebabSource.register_extension(ReloadExtension)
```

### Comparing `pykebab-0.7.8/kebab/utils.py` & `pykebab-0.7.9/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.8/pyproject.toml` & `pykebab-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykebab"
-version = "0.7.8"
+version = "0.7.9"
 description = ""
 authors = ["Yangming Huang <leonmax@gmail.com>"]
 packages = [
     { include = "kebab" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `pykebab-0.7.8/PKG-INFO` & `pykebab-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.7.8
+Version: 0.7.9
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

