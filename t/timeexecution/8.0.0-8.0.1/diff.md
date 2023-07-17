# Comparing `tmp/timeexecution-8.0.0.tar.gz` & `tmp/timeexecution-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeexecution-8.0.0.tar", last modified: Wed Apr 26 15:48:06 2023, max compression
+gzip compressed data, was "timeexecution-8.0.1.tar", last modified: Mon Jul 17 12:07:44 2023, max compression
```

## Comparing `timeexecution-8.0.0.tar` & `timeexecution-8.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:48:06.336107 timeexecution-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-26 15:47:50.000000 timeexecution-8.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-26 15:47:50.000000 timeexecution-8.0.0/.gitchangelog.rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:48:06.332107 timeexecution-8.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:48:06.332107 timeexecution-8.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-26 15:47:50.000000 timeexecution-8.0.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-26 15:47:50.000000 timeexecution-8.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-26 15:47:50.000000 timeexecution-8.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-26 15:47:50.000000 timeexecution-8.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-04-26 15:47:50.000000 timeexecution-8.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 15:47:50.000000 timeexecution-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-26 15:47:50.000000 timeexecution-8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-26 15:47:50.000000 timeexecution-8.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-26 15:48:06.336107 timeexecution-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-04-26 15:47:50.000000 timeexecution-8.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-26 15:47:50.000000 timeexecution-8.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-26 15:47:50.000000 timeexecution-8.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-26 15:48:06.336107 timeexecution-8.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1693 2023-04-26 15:47:50.000000 timeexecution-8.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:48:06.336107 timeexecution-8.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:47:50.000000 timeexecution-8.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-26 15:47:50.000000 timeexecution-8.0.0/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      490 2023-04-26 15:47:50.000000 timeexecution-8.0.0/tests/dummy_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 15:47:50.000000 timeexecution-8.0.0/tests/test_base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-26 15:47:50.000000 timeexecution-8.0.0/tests/test_decorator_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-04-26 15:47:50.000000 timeexecution-8.0.0/tests/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-04-26 15:47:50.000000 timeexecution-8.0.0/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-04-26 15:47:50.000000 timeexecution-8.0.0/tests/test_threaded_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:48:06.336107 timeexecution-8.0.0/time_execution/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 15:47:50.000000 timeexecution-8.0.0/time_execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:48:06.336107 timeexecution-8.0.0/time_execution/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:47:50.000000 timeexecution-8.0.0/time_execution/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-26 15:47:50.000000 timeexecution-8.0.0/time_execution/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-26 15:47:50.000000 timeexecution-8.0.0/time_execution/backends/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-26 15:47:50.000000 timeexecution-8.0.0/time_execution/backends/threaded.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2509 2023-04-26 15:47:50.000000 timeexecution-8.0.0/time_execution/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:47:50.000000 timeexecution-8.0.0/time_execution/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-26 15:47:50.000000 timeexecution-8.0.0/time_execution/timed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:48:06.336107 timeexecution-8.0.0/timeexecution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-26 15:48:06.000000 timeexecution-8.0.0/timeexecution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-26 15:48:06.000000 timeexecution-8.0.0/timeexecution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:48:06.000000 timeexecution-8.0.0/timeexecution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:48:06.000000 timeexecution-8.0.0/timeexecution.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 15:48:06.000000 timeexecution-8.0.0/timeexecution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 15:48:06.000000 timeexecution-8.0.0/timeexecution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-26 15:47:50.000000 timeexecution-8.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:07:44.050544 timeexecution-8.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-17 12:07:30.000000 timeexecution-8.0.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-17 12:07:30.000000 timeexecution-8.0.1/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:07:44.046544 timeexecution-8.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:07:44.046544 timeexecution-8.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-17 12:07:30.000000 timeexecution-8.0.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-17 12:07:30.000000 timeexecution-8.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-17 12:07:30.000000 timeexecution-8.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-17 12:07:30.000000 timeexecution-8.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-17 12:07:30.000000 timeexecution-8.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 12:07:30.000000 timeexecution-8.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-17 12:07:30.000000 timeexecution-8.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-17 12:07:30.000000 timeexecution-8.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-17 12:07:44.050544 timeexecution-8.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-07-17 12:07:30.000000 timeexecution-8.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-17 12:07:30.000000 timeexecution-8.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-17 12:07:30.000000 timeexecution-8.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 12:07:44.050544 timeexecution-8.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1693 2023-07-17 12:07:30.000000 timeexecution-8.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:07:44.046544 timeexecution-8.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:07:30.000000 timeexecution-8.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 12:07:30.000000 timeexecution-8.0.1/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      490 2023-07-17 12:07:30.000000 timeexecution-8.0.1/tests/dummy_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-17 12:07:30.000000 timeexecution-8.0.1/tests/test_base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-17 12:07:30.000000 timeexecution-8.0.1/tests/test_decorator_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-17 12:07:30.000000 timeexecution-8.0.1/tests/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-17 12:07:30.000000 timeexecution-8.0.1/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-17 12:07:30.000000 timeexecution-8.0.1/tests/test_threaded_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:07:44.050544 timeexecution-8.0.1/time_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 12:07:30.000000 timeexecution-8.0.1/time_execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:07:44.050544 timeexecution-8.0.1/time_execution/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:07:30.000000 timeexecution-8.0.1/time_execution/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-17 12:07:30.000000 timeexecution-8.0.1/time_execution/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-17 12:07:30.000000 timeexecution-8.0.1/time_execution/backends/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-17 12:07:30.000000 timeexecution-8.0.1/time_execution/backends/threaded.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2509 2023-07-17 12:07:30.000000 timeexecution-8.0.1/time_execution/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:07:30.000000 timeexecution-8.0.1/time_execution/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-17 12:07:30.000000 timeexecution-8.0.1/time_execution/timed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:07:44.050544 timeexecution-8.0.1/timeexecution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-17 12:07:44.000000 timeexecution-8.0.1/timeexecution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-17 12:07:44.000000 timeexecution-8.0.1/timeexecution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:07:44.000000 timeexecution-8.0.1/timeexecution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:07:44.000000 timeexecution-8.0.1/timeexecution.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 12:07:44.000000 timeexecution-8.0.1/timeexecution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 12:07:44.000000 timeexecution-8.0.1/timeexecution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-17 12:07:30.000000 timeexecution-8.0.1/tox.ini
```

### Comparing `timeexecution-8.0.0/.editorconfig` & `timeexecution-8.0.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/.gitchangelog.rc` & `timeexecution-8.0.1/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/.github/workflows/publish.yml` & `timeexecution-8.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/.github/workflows/tests.yml` & `timeexecution-8.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/.gitignore` & `timeexecution-8.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/CHANGELOG.md` & `timeexecution-8.0.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/LICENSE` & `timeexecution-8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/Makefile` & `timeexecution-8.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/PKG-INFO` & `timeexecution-8.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeexecution
-Version: 8.0.0
+Version: 8.0.1
 Summary: Python project
 Home-page: https://github.com/kpn/py-timeexecution
 Author: KPN DE Platform
 Author-email: de-platform@kpn.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `timeexecution-8.0.0/README.md` & `timeexecution-8.0.1/README.md`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/pyproject.toml` & `timeexecution-8.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/setup.py` & `timeexecution-8.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/tests/test_decorator_async.py` & `timeexecution-8.0.1/tests/test_decorator_async.py`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/tests/test_elasticsearch.py` & `timeexecution-8.0.1/tests/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/tests/test_hooks.py` & `timeexecution-8.0.1/tests/test_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
             collector.clean()
 
     def test_hook(self):
         def test_args(**kwargs):
             assert "response" in kwargs
             assert "exception" in kwargs
             assert "metric" in kwargs
+            assert "name" in kwargs["metric"]
             return dict()
 
         def test_metadata(*args, **kwargs):
             return dict(test_key="test value")
 
         def asserts(name, **data):
             assert data["test_key"] == "test value"
```

### Comparing `timeexecution-8.0.0/tests/test_threaded_backend.py` & `timeexecution-8.0.1/tests/test_threaded_backend.py`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/time_execution/backends/elasticsearch.py` & `timeexecution-8.0.1/time_execution/backends/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/time_execution/backends/threaded.py` & `timeexecution-8.0.1/time_execution/backends/threaded.py`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/time_execution/decorator.py` & `timeexecution-8.0.1/time_execution/decorator.py`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/time_execution/timed.py` & `timeexecution-8.0.1/time_execution/timed.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,15 +66,20 @@
 
         hooks = self._extra_hooks or []
         if not self._disable_default_hooks:
             hooks = settings.hooks + hooks
 
         # Apply the registered hooks, and collect the metadata they might
         # return to be stored with the metrics.
-        metadata = self._apply_hooks(hooks=hooks, response=self.result, exception=__exc_val, metric=metric)
+        metadata = self._apply_hooks(
+            hooks=hooks,
+            response=self.result,
+            exception=__exc_val,
+            metric={**metric, "name": self._fqn},
+        )
 
         metric.update(metadata)
         write_metric(name=self._fqn, **metric)
 
     def _apply_hooks(self, hooks, response, exception, metric) -> Dict:
         metadata = dict()
         for hook in hooks:
```

### Comparing `timeexecution-8.0.0/timeexecution.egg-info/PKG-INFO` & `timeexecution-8.0.1/timeexecution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeexecution
-Version: 8.0.0
+Version: 8.0.1
 Summary: Python project
 Home-page: https://github.com/kpn/py-timeexecution
 Author: KPN DE Platform
 Author-email: de-platform@kpn.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `timeexecution-8.0.0/timeexecution.egg-info/SOURCES.txt` & `timeexecution-8.0.1/timeexecution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeexecution-8.0.0/tox.ini` & `timeexecution-8.0.1/tox.ini`

 * *Files identical despite different names*

