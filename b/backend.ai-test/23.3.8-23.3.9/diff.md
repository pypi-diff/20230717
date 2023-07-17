# Comparing `tmp/backend.ai-test-23.3.8.tar.gz` & `tmp/backend.ai-test-23.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-test-23.3.8.tar", last modified: Thu Jul  6 04:38:09 2023, max compression
+gzip compressed data, was "backend.ai-test-23.3.9.tar", last modified: Mon Jul 17 14:36:05 2023, max compression
```

## Comparing `backend.ai-test-23.3.8.tar` & `backend.ai-test-23.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.264312 backend.ai-test-23.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 04:38:08.000000 backend.ai-test-23.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-06 04:38:09.264312 backend.ai-test-23.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.264312 backend.ai-test-23.3.8/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.264312 backend.ai-test-23.3.8/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.264312 backend.ai-test-23.3.8/ai/backend/test/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 04:38:08.000000 backend.ai-test-23.3.8/ai/backend/test/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 04:38:08.000000 backend.ai-test-23.3.8/ai/backend/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.264312 backend.ai-test-23.3.8/ai/backend/test/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:08.000000 backend.ai-test-23.3.8/ai/backend/test/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-06 04:38:08.000000 backend.ai-test-23.3.8/ai/backend/test/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 04:38:08.000000 backend.ai-test-23.3.8/ai/backend/test/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-06 04:38:08.000000 backend.ai-test-23.3.8/ai/backend/test/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 04:38:08.000000 backend.ai-test-23.3.8/ai/backend/test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.264312 backend.ai-test-23.3.8/backend.ai_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-06 04:38:09.000000 backend.ai-test-23.3.8/backend.ai_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-06 04:38:09.000000 backend.ai-test-23.3.8/backend.ai_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:09.000000 backend.ai-test-23.3.8/backend.ai_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 04:38:09.000000 backend.ai-test-23.3.8/backend.ai_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:09.000000 backend.ai-test-23.3.8/backend.ai_test.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:09.000000 backend.ai-test-23.3.8/backend.ai_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-06 04:38:09.000000 backend.ai-test-23.3.8/backend.ai_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 04:38:09.000000 backend.ai-test-23.3.8/backend.ai_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 04:38:08.000000 backend.ai-test-23.3.8/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 04:38:09.264312 backend.ai-test-23.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-06 04:38:08.000000 backend.ai-test-23.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:05.292694 backend.ai-test-23.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 14:36:04.000000 backend.ai-test-23.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-17 14:36:05.292694 backend.ai-test-23.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:05.288694 backend.ai-test-23.3.9/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:05.288694 backend.ai-test-23.3.9/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:05.288694 backend.ai-test-23.3.9/ai/backend/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:36:04.000000 backend.ai-test-23.3.9/ai/backend/test/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 14:36:04.000000 backend.ai-test-23.3.9/ai/backend/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:05.288694 backend.ai-test-23.3.9/ai/backend/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:04.000000 backend.ai-test-23.3.9/ai/backend/test/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-17 14:36:04.000000 backend.ai-test-23.3.9/ai/backend/test/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 14:36:04.000000 backend.ai-test-23.3.9/ai/backend/test/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-17 14:36:04.000000 backend.ai-test-23.3.9/ai/backend/test/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 14:36:04.000000 backend.ai-test-23.3.9/ai/backend/test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:05.292694 backend.ai-test-23.3.9/backend.ai_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-17 14:36:05.000000 backend.ai-test-23.3.9/backend.ai_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-17 14:36:05.000000 backend.ai-test-23.3.9/backend.ai_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:05.000000 backend.ai-test-23.3.9/backend.ai_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-17 14:36:05.000000 backend.ai-test-23.3.9/backend.ai_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:05.000000 backend.ai-test-23.3.9/backend.ai_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:05.000000 backend.ai-test-23.3.9/backend.ai_test.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 14:36:05.000000 backend.ai-test-23.3.9/backend.ai_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-17 14:36:05.000000 backend.ai-test-23.3.9/backend.ai_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-17 14:36:04.000000 backend.ai-test-23.3.9/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:36:05.292694 backend.ai-test-23.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-17 14:36:04.000000 backend.ai-test-23.3.9/setup.py
```

### Comparing `backend.ai-test-23.3.8/PKG-INFO` & `backend.ai-test-23.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 23.3.8
+Version: 23.3.9
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-test-23.3.8/ai/backend/test/cli/__main__.py` & `backend.ai-test-23.3.9/ai/backend/test/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.8/ai/backend/test/cli/utils.py` & `backend.ai-test-23.3.9/ai/backend/test/cli/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.8/backend.ai_test.egg-info/PKG-INFO` & `backend.ai-test-23.3.9/backend.ai_test.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 23.3.8
+Version: 23.3.9
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-test-23.3.8/backend.ai_test.egg-info/SOURCES.txt` & `backend.ai-test-23.3.9/backend.ai_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.8/backend_shim.py` & `backend.ai-test-23.3.9/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.8/setup.py` & `backend.ai-test-23.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,11 +66,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.8
+    'version': """23.03.9
 """,
     'zip_safe': False,
 })
```

