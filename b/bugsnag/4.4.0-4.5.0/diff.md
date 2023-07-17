# Comparing `tmp/bugsnag-4.4.0.tar.gz` & `tmp/bugsnag-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugsnag-4.4.0.tar", last modified: Tue Feb 21 09:13:28 2023, max compression
+gzip compressed data, was "bugsnag-4.5.0.tar", last modified: Mon Jul 17 09:25:56 2023, max compression
```

## Comparing `bugsnag-4.4.0.tar` & `bugsnag-4.5.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-02-21 09:13:28.814075 bugsnag-4.4.0/
--rw-r--r--   0 joe.haines   (504) staff       (20)     1050 2022-10-04 14:38:17.000000 bugsnag-4.4.0/LICENSE.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)     1312 2023-02-21 09:13:28.814169 bugsnag-4.4.0/PKG-INFO
--rw-r--r--   0 joe.haines   (504) staff       (20)     1975 2023-01-18 16:09:16.000000 bugsnag-4.4.0/README.md
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-02-21 09:13:28.796843 bugsnag-4.4.0/bugsnag/
--rw-r--r--   0 joe.haines   (504) staff       (20)     1150 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     4743 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/asgi.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     3389 2023-01-19 12:01:29.000000 bugsnag-4.4.0/bugsnag/breadcrumbs.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-02-21 09:13:28.809537 bugsnag-4.4.0/bugsnag/celery/
--rw-r--r--   0 joe.haines   (504) staff       (20)      977 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/celery/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    10733 2023-02-03 11:23:01.000000 bugsnag-4.4.0/bugsnag/client.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    19212 2022-11-02 11:51:55.000000 bugsnag-4.4.0/bugsnag/configuration.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     5036 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/delivery.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-02-21 09:13:28.811282 bugsnag-4.4.0/bugsnag/django/
--rw-r--r--   0 joe.haines   (504) staff       (20)     3654 2023-01-19 12:40:00.000000 bugsnag-4.4.0/bugsnag/django/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     2011 2022-11-02 11:51:55.000000 bugsnag-4.4.0/bugsnag/django/middleware.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      114 2022-10-26 12:09:12.000000 bugsnag-4.4.0/bugsnag/django/utils.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      695 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/error.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    14553 2023-02-21 09:13:04.000000 bugsnag-4.4.0/bugsnag/event.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-02-21 09:13:28.811816 bugsnag-4.4.0/bugsnag/flask/
--rw-r--r--   0 joe.haines   (504) staff       (20)     2250 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/flask/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     6182 2023-02-02 13:07:41.000000 bugsnag-4.4.0/bugsnag/handlers.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     4656 2023-01-19 12:01:29.000000 bugsnag-4.4.0/bugsnag/legacy.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     5336 2023-01-19 12:01:29.000000 bugsnag-4.4.0/bugsnag/middleware.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      464 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/notification.py
--rw-r--r--   0 joe.haines   (504) staff       (20)        0 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/py.typed
--rw-r--r--   0 joe.haines   (504) staff       (20)     4934 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/sessiontracker.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-02-21 09:13:28.812354 bugsnag-4.4.0/bugsnag/tornado/
--rw-r--r--   0 joe.haines   (504) staff       (20)     3983 2023-01-19 12:01:29.000000 bugsnag-4.4.0/bugsnag/tornado/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    14067 2023-02-21 09:13:04.000000 bugsnag-4.4.0/bugsnag/utils.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     1096 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/uwsgi.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-02-21 09:13:28.813625 bugsnag-4.4.0/bugsnag/wsgi/
--rw-r--r--   0 joe.haines   (504) staff       (20)      147 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/wsgi/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     3745 2022-10-04 14:38:17.000000 bugsnag-4.4.0/bugsnag/wsgi/middleware.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-02-21 09:13:28.808735 bugsnag-4.4.0/bugsnag.egg-info/
--rw-r--r--   0 joe.haines   (504) staff       (20)     1312 2023-02-21 09:13:28.000000 bugsnag-4.4.0/bugsnag.egg-info/PKG-INFO
--rw-r--r--   0 joe.haines   (504) staff       (20)      724 2023-02-21 09:13:28.000000 bugsnag-4.4.0/bugsnag.egg-info/SOURCES.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)        1 2023-02-21 09:13:28.000000 bugsnag-4.4.0/bugsnag.egg-info/dependency_links.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)       29 2023-02-21 09:13:28.000000 bugsnag-4.4.0/bugsnag.egg-info/requires.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)        8 2023-02-21 09:13:28.000000 bugsnag-4.4.0/bugsnag.egg-info/top_level.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)       76 2023-02-21 09:13:28.815101 bugsnag-4.4.0/setup.cfg
--rwxr-xr-x   0 joe.haines   (504) staff       (20)     1653 2023-02-21 09:13:04.000000 bugsnag-4.4.0/setup.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-07-17 09:25:56.929592 bugsnag-4.5.0/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1050 2022-10-04 14:38:17.000000 bugsnag-4.5.0/LICENSE.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1312 2023-07-17 09:25:56.929690 bugsnag-4.5.0/PKG-INFO
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1975 2023-01-18 16:09:16.000000 bugsnag-4.5.0/README.md
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-07-17 09:25:56.927109 bugsnag-4.5.0/bugsnag/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1150 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     4743 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/asgi.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3389 2023-01-19 12:01:29.000000 bugsnag-4.5.0/bugsnag/breadcrumbs.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-07-17 09:25:56.927906 bugsnag-4.5.0/bugsnag/celery/
+-rw-r--r--   0 joe.haines   (504) staff       (20)      977 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/celery/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    10733 2023-02-03 11:23:01.000000 bugsnag-4.5.0/bugsnag/client.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    19598 2023-07-17 09:25:50.000000 bugsnag-4.5.0/bugsnag/configuration.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5036 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/delivery.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-07-17 09:25:56.928678 bugsnag-4.5.0/bugsnag/django/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3654 2023-01-19 12:40:00.000000 bugsnag-4.5.0/bugsnag/django/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2011 2022-11-02 11:51:55.000000 bugsnag-4.5.0/bugsnag/django/middleware.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      114 2022-10-26 12:09:12.000000 bugsnag-4.5.0/bugsnag/django/utils.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      695 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/error.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    14749 2023-07-17 09:25:50.000000 bugsnag-4.5.0/bugsnag/event.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-07-17 09:25:56.928955 bugsnag-4.5.0/bugsnag/flask/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2250 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/flask/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     6512 2023-07-17 09:25:50.000000 bugsnag-4.5.0/bugsnag/handlers.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     4656 2023-01-19 12:01:29.000000 bugsnag-4.5.0/bugsnag/legacy.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5336 2023-01-19 12:01:29.000000 bugsnag-4.5.0/bugsnag/middleware.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      464 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/notification.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)        0 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/py.typed
+-rw-r--r--   0 joe.haines   (504) staff       (20)     4934 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/sessiontracker.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-07-17 09:25:56.929129 bugsnag-4.5.0/bugsnag/tornado/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5824 2023-07-17 09:25:50.000000 bugsnag-4.5.0/bugsnag/tornado/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    15059 2023-07-17 09:25:50.000000 bugsnag-4.5.0/bugsnag/utils.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1096 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/uwsgi.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-07-17 09:25:56.929428 bugsnag-4.5.0/bugsnag/wsgi/
+-rw-r--r--   0 joe.haines   (504) staff       (20)      147 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/wsgi/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3745 2022-10-04 14:38:17.000000 bugsnag-4.5.0/bugsnag/wsgi/middleware.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2023-07-17 09:25:56.927791 bugsnag-4.5.0/bugsnag.egg-info/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1312 2023-07-17 09:25:56.000000 bugsnag-4.5.0/bugsnag.egg-info/PKG-INFO
+-rw-r--r--   0 joe.haines   (504) staff       (20)      724 2023-07-17 09:25:56.000000 bugsnag-4.5.0/bugsnag.egg-info/SOURCES.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)        1 2023-07-17 09:25:56.000000 bugsnag-4.5.0/bugsnag.egg-info/dependency_links.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)       29 2023-07-17 09:25:56.000000 bugsnag-4.5.0/bugsnag.egg-info/requires.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)        8 2023-07-17 09:25:56.000000 bugsnag-4.5.0/bugsnag.egg-info/top_level.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)       76 2023-07-17 09:25:56.929925 bugsnag-4.5.0/setup.cfg
+-rwxr-xr-x   0 joe.haines   (504) staff       (20)     1653 2023-07-17 09:25:50.000000 bugsnag-4.5.0/setup.py
```

### Comparing `bugsnag-4.4.0/LICENSE.txt` & `bugsnag-4.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/PKG-INFO` & `bugsnag-4.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugsnag
-Version: 4.4.0
+Version: 4.5.0
 Summary: Automatic error monitoring for django, flask, etc.
 Home-page: https://bugsnag.com/
 Author: Simon Maynard
 Author-email: simon@bugsnag.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `bugsnag-4.4.0/README.md` & `bugsnag-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/__init__.py` & `bugsnag-4.5.0/bugsnag/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/asgi.py` & `bugsnag-4.5.0/bugsnag/asgi.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/breadcrumbs.py` & `bugsnag-4.5.0/bugsnag/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/celery/__init__.py` & `bugsnag-4.5.0/bugsnag/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/client.py` & `bugsnag-4.5.0/bugsnag/client.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/configuration.py` & `bugsnag-4.5.0/bugsnag/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,30 +16,45 @@
 )
 from bugsnag.sessiontracker import SessionMiddleware
 from bugsnag.middleware import (
     DefaultMiddleware,
     MiddlewareStack,
     skip_bugsnag_middleware
 )
-from bugsnag.utils import (fully_qualified_class_name, validate_str_setter,
-                           validate_bool_setter, validate_iterable_setter,
-                           validate_required_str_setter, validate_int_setter)
+from bugsnag.utils import (
+    fully_qualified_class_name,
+    partly_qualified_class_name,
+    validate_str_setter,
+    validate_bool_setter,
+    validate_iterable_setter,
+    validate_required_str_setter,
+    validate_int_setter,
+    validate_path_setter
+)
 from bugsnag.delivery import (create_default_delivery, DEFAULT_ENDPOINT,
                               DEFAULT_SESSIONS_ENDPOINT)
 from bugsnag.uwsgi import warn_if_running_uwsgi_without_threads
 from bugsnag.error import Error
 
 try:
     from contextvars import ContextVar
     _request_info = ContextVar('bugsnag-request', default=None)  # type: ignore
 except ImportError:
     from bugsnag.utils import ThreadContextVar
     _request_info = ThreadContextVar('bugsnag-request', default=None)  # type: ignore  # noqa: E501
 
 
+try:
+    from os import PathLike
+except ImportError:
+    # PathLike was added in Python 3.6 so fallback to PurePath on Python 3.5 as
+    # all builtin Path objects inherit from PurePath
+    from pathlib import PurePath as PathLike  # type: ignore
+
+
 __all__ = ('Configuration', 'RequestConfiguration')
 _sentinel = object()
 
 
 class Configuration:
     """
     Global app-level Bugsnag configuration settings.
@@ -358,17 +373,17 @@
         Traceback file paths which contain this prefix are considered a part of
         the project. This prefix is also stripped to increase file name
         readability in traceback lines.
         """
         return self._project_root
 
     @project_root.setter  # type: ignore
-    @validate_str_setter
-    def project_root(self, value: str):
-        self._project_root = value
+    @validate_path_setter
+    def project_root(self, value: Union[str, PathLike]):
+        self._project_root = str(value)
 
     @property
     def proxy_host(self):
         """
         The host name of the proxy to use to deliver requests, if any
         """
         return self._proxy_host
@@ -517,15 +532,16 @@
             return False
 
         # if this is a list of Error instances, check if any of the error
         # classes are ignored
         if isinstance(exception, list):
             return any(e.error_class in self.ignore_classes for e in exception)
 
-        return fully_qualified_class_name(exception) in self.ignore_classes
+        return (fully_qualified_class_name(exception) in self.ignore_classes or
+                partly_qualified_class_name(exception) in self.ignore_classes)
 
     def _create_default_logger(self) -> logging.Logger:
         logger = logging.getLogger('bugsnag')
         logger.setLevel(logging.WARNING)
 
         format = '%(asctime)s - [%(name)s] %(levelname)s - %(message)s'
         formatter = logging.Formatter(format)
```

### Comparing `bugsnag-4.4.0/bugsnag/delivery.py` & `bugsnag-4.5.0/bugsnag/delivery.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/django/__init__.py` & `bugsnag-4.5.0/bugsnag/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/django/middleware.py` & `bugsnag-4.5.0/bugsnag/django/middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/error.py` & `bugsnag-4.5.0/bugsnag/error.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/event.py` & `bugsnag-4.5.0/bugsnag/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,29 +109,35 @@
         self.grouping_hash = options.pop("grouping_hash", None)
         self.api_key = options.pop("api_key", get_config("api_key"))
 
         self.session = None  # type: Optional[Dict]
 
         self.metadata = {}  # type: Dict[str, Dict[str, Any]]
         if 'meta_data' in options:
-            warnings.warn('The Event "metadata" argument has been replaced ' +
+            warnings.warn('The Event "meta_data" argument has been replaced ' +
                           'with "metadata"', DeprecationWarning)
             for name, tab in options.pop("meta_data").items():
                 self.add_tab(name, tab)
 
         for name, tab in options.pop('metadata', {}).items():
             self.add_tab(name, tab)
 
         for name, tab in options.items():
             self.add_tab(name, tab)
 
+        if hasattr(exception, "__notes__"):
+            self.add_tab(
+                "exception notes",
+                dict(enumerate(exception.__notes__)) # type: ignore # noqa
+            )
+
     @property
     def meta_data(self) -> Dict[str, Dict[str, Any]]:
-        warnings.warn('The Event "metadata" property has been replaced ' +
-                      'with "meta_data".', DeprecationWarning)
+        warnings.warn('The Event "meta_data" property has been replaced ' +
+                      'with "metadata".', DeprecationWarning)
         return self.metadata
 
     @property
     def breadcrumbs(self) -> List[Breadcrumb]:
         return self._breadcrumbs.copy()
 
     @property
```

### Comparing `bugsnag-4.4.0/bugsnag/flask/__init__.py` & `bugsnag-4.5.0/bugsnag/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/handlers.py` & `bugsnag-4.5.0/bugsnag/handlers.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         Creates a new handler which sends records to Bugsnag
         """
         super(BugsnagHandler, self).__init__()
         self.client = client
         self.custom_metadata_fields = extra_fields
         self.callbacks = [self.extract_default_metadata,
                           self.extract_custom_metadata,
-                          self.extract_severity]
+                          self.extract_severity,
+                          self.extract_grouping_hash]
 
     def emit(self, record: LogRecord):
         """
         Outputs the record to Bugsnag
         """
         if hasattr(bugsnag, '__path__'):
             paths = getattr(bugsnag, '__path__')
@@ -109,14 +110,21 @@
         if levelno >= logging.ERROR:
             options['severity'] = 'error'
         elif levelno >= logging.WARNING:
             options['severity'] = 'warning'
         else:
             options['severity'] = 'info'
 
+    def extract_grouping_hash(self, record: LogRecord, options: Dict):
+        """
+        Add the grouping_hash from a log record to the options
+        """
+        if 'groupingHash' in record.__dict__:
+            options['grouping_hash'] = record.__dict__['groupingHash']
+
     def extract_custom_metadata(self, record: LogRecord, options: Dict):
         """
         Append the contents of selected fields of a record to the metadata
         of a report
         """
         if self.custom_metadata_fields is None:
             return
```

### Comparing `bugsnag-4.4.0/bugsnag/legacy.py` & `bugsnag-4.5.0/bugsnag/legacy.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/middleware.py` & `bugsnag-4.5.0/bugsnag/middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/sessiontracker.py` & `bugsnag-4.5.0/bugsnag/sessiontracker.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/utils.py` & `bugsnag-4.5.0/bugsnag/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 from typing import AnyStr, Tuple, Optional
 import warnings
 import copy
 import logging
 from datetime import datetime, timedelta
 from urllib.parse import urlparse, urlunsplit, parse_qs
 
+
+try:
+    from os import PathLike
+except ImportError:
+    # PathLike was added in Python 3.6 so fallback to PurePath on Python 3.5 as
+    # all builtin Path objects inherit from PurePath
+    from pathlib import PurePath as PathLike  # type: ignore
+
+
 MAX_PAYLOAD_LENGTH = 128 * 1024
 MAX_STRING_LENGTH = 1024
 
 
 __all__ = []  # type: ignore
 
 
@@ -77,14 +86,17 @@
             for key, value in obj.items():
                 if self._should_filter(key):
                     clean_dict[key] = self.filtered_value
                 else:
                     clean_dict[key] = self.filter_string_values(
                         value, ignored, seen)
 
+            # Only ignore whilst encoding children
+            ignored.remove(id(obj))
+
             return clean_dict
 
         return obj
 
     def default(self, obj):
         """
         Coerce values to strings if possible, otherwise replace with
@@ -115,24 +127,33 @@
 
         if type(ignored) is list:
             ignored = set(ignored)
 
         if id(obj) in ignored:
             return self.recursive_value
         elif isinstance(obj, dict):
-            ignored.add(id(obj))
             seen.append(obj)
-            return self._sanitize_dict(obj, trim_strings, ignored, seen)
-        elif isinstance(obj, (set, tuple, list)):
+
             ignored.add(id(obj))
+            sanitized = self._sanitize_dict(obj, trim_strings, ignored, seen)
+            # Only ignore whilst encoding children
+            ignored.remove(id(obj))
+
+            return sanitized
+        elif isinstance(obj, (set, tuple, list)):
             seen.append(obj)
+
+            ignored.add(id(obj))
             items = []
             for value in obj:
                 items.append(
                         self._sanitize(value, trim_strings, ignored, seen))
+            # Only ignore whilst encoding children
+            ignored.remove(id(obj))
+
             return items
         elif trim_strings and isinstance(obj, str):
             return obj[:MAX_STRING_LENGTH]
         else:
             return obj
 
     def _sanitize_dict_key_value(self, clean_dict, key, clean_value):
@@ -239,23 +260,36 @@
     type, subtype, suffix, _ = parse_content_type(value.lower())
     return type == 'application' and (subtype == 'json' or suffix == 'json')
 
 
 _ignore_modules = ('__main__', 'builtins')
 
 
-def fully_qualified_class_name(obj):
+def partly_qualified_class_name(obj):
     module = inspect.getmodule(obj)
 
     if module is None or module.__name__ in _ignore_modules:
         return obj.__class__.__name__
 
     return module.__name__ + '.' + obj.__class__.__name__
 
 
+def fully_qualified_class_name(obj):
+    module = inspect.getmodule(obj)
+    if hasattr(obj.__class__, "__qualname__"):
+        qualified_name = obj.__class__.__qualname__
+    else:
+        qualified_name = obj.__class__.__name__
+
+    if module is None or module.__name__ in _ignore_modules:
+        return qualified_name
+
+    return module.__name__ + '.' + qualified_name
+
+
 def package_version(package_name):
     try:
         import pkg_resources
     except ImportError:
         return None
     else:
         try:
@@ -289,14 +323,15 @@
 
 validate_str_setter = partial(_validate_setter, (str,))
 validate_required_str_setter = partial(_validate_setter, (str,),
                                        should_error=True)
 validate_bool_setter = partial(_validate_setter, (bool,))
 validate_iterable_setter = partial(_validate_setter, (list, tuple))
 validate_int_setter = partial(_validate_setter, (int,))
+validate_path_setter = partial(_validate_setter, (str, PathLike))
 
 
 class ThreadContextVar:
     """
     A wrapper around thread-local variables to mimic the API of contextvars
     """
     LOCALS = None
```

### Comparing `bugsnag-4.4.0/bugsnag/uwsgi.py` & `bugsnag-4.5.0/bugsnag/uwsgi.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag/wsgi/middleware.py` & `bugsnag-4.5.0/bugsnag/wsgi/middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/bugsnag.egg-info/PKG-INFO` & `bugsnag-4.5.0/bugsnag.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugsnag
-Version: 4.4.0
+Version: 4.5.0
 Summary: Automatic error monitoring for django, flask, etc.
 Home-page: https://bugsnag.com/
 Author: Simon Maynard
 Author-email: simon@bugsnag.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `bugsnag-4.4.0/bugsnag.egg-info/SOURCES.txt` & `bugsnag-4.5.0/bugsnag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bugsnag-4.4.0/setup.py` & `bugsnag-4.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 and solve your bugs as fast as possible.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='bugsnag',
-    version='4.4.0',
+    version='4.5.0',
     description='Automatic error monitoring for django, flask, etc.',
     long_description=__doc__,
     author='Simon Maynard',
     author_email='simon@bugsnag.com',
     url='https://bugsnag.com/',
     license='MIT',
     python_requires='>=3.5, <4',
```

