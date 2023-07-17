# Comparing `tmp/backend.ai-accelerator-mock-23.3.8.tar.gz` & `tmp/backend.ai-accelerator-mock-23.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-accelerator-mock-23.3.8.tar", last modified: Thu Jul  6 04:38:11 2023, max compression
+gzip compressed data, was "backend.ai-accelerator-mock-23.3.9.tar", last modified: Mon Jul 17 14:36:04 2023, max compression
```

## Comparing `backend.ai-accelerator-mock-23.3.8.tar` & `backend.ai-accelerator-mock-23.3.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:11.180336 backend.ai-accelerator-mock-23.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 04:38:10.000000 backend.ai-accelerator-mock-23.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-06 04:38:11.180336 backend.ai-accelerator-mock-23.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:11.176336 backend.ai-accelerator-mock-23.3.8/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:11.176336 backend.ai-accelerator-mock-23.3.8/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:11.176336 backend.ai-accelerator-mock-23.3.8/ai/backend/accelerator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:11.176336 backend.ai-accelerator-mock-23.3.8/ai/backend/accelerator/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 04:38:10.000000 backend.ai-accelerator-mock-23.3.8/ai/backend/accelerator/mock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 04:38:10.000000 backend.ai-accelerator-mock-23.3.8/ai/backend/accelerator/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-06 04:38:10.000000 backend.ai-accelerator-mock-23.3.8/ai/backend/accelerator/mock/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-07-06 04:38:10.000000 backend.ai-accelerator-mock-23.3.8/ai/backend/accelerator/mock/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 04:38:10.000000 backend.ai-accelerator-mock-23.3.8/ai/backend/accelerator/mock/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-06 04:38:10.000000 backend.ai-accelerator-mock-23.3.8/ai/backend/accelerator/mock/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:11.180336 backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-06 04:38:11.000000 backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-06 04:38:11.000000 backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:11.000000 backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 04:38:11.000000 backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:11.000000 backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:11.000000 backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-06 04:38:11.000000 backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 04:38:11.000000 backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 04:38:10.000000 backend.ai-accelerator-mock-23.3.8/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 04:38:11.180336 backend.ai-accelerator-mock-23.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-06 04:38:10.000000 backend.ai-accelerator-mock-23.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:04.908687 backend.ai-accelerator-mock-23.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-17 14:36:04.908687 backend.ai-accelerator-mock-23.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:04.908687 backend.ai-accelerator-mock-23.3.9/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:04.908687 backend.ai-accelerator-mock-23.3.9/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:04.908687 backend.ai-accelerator-mock-23.3.9/ai/backend/accelerator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:04.908687 backend.ai-accelerator-mock-23.3.9/ai/backend/accelerator/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/ai/backend/accelerator/mock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/ai/backend/accelerator/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/ai/backend/accelerator/mock/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/ai/backend/accelerator/mock/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/ai/backend/accelerator/mock/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/ai/backend/accelerator/mock/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:04.908687 backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:36:04.908687 backend.ai-accelerator-mock-23.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-17 14:36:04.000000 backend.ai-accelerator-mock-23.3.9/setup.py
```

### Comparing `backend.ai-accelerator-mock-23.3.8/PKG-INFO` & `backend.ai-accelerator-mock-23.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-mock
-Version: 23.3.8
+Version: 23.3.9
 Summary: Backend.AI Mockup Accelerator Plugin
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-accelerator-mock-23.3.8/ai/backend/accelerator/mock/plugin.py` & `backend.ai-accelerator-mock-23.3.9/ai/backend/accelerator/mock/plugin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.8/ai/backend/accelerator/mock/types.py` & `backend.ai-accelerator-mock-23.3.9/ai/backend/accelerator/mock/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/PKG-INFO` & `backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-mock
-Version: 23.3.8
+Version: 23.3.9
 Summary: Backend.AI Mockup Accelerator Plugin
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-accelerator-mock-23.3.8/backend.ai_accelerator_mock.egg-info/SOURCES.txt` & `backend.ai-accelerator-mock-23.3.9/backend.ai_accelerator_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.8/backend_shim.py` & `backend.ai-accelerator-mock-23.3.9/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.8/setup.py` & `backend.ai-accelerator-mock-23.3.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,27 +23,27 @@
     'entry_points': {
         'backendai_accelerator_v21': [
             'mock = ai.backend.accelerator.mock.plugin:MockPlugin',
         ],
     },
     'install_requires': (
         'aiodocker~=0.21.0',
-        """backend.ai-agent==23.03.8
+        """backend.ai-agent==23.03.9
 """,
-        """backend.ai-cli==23.03.8
+        """backend.ai-cli==23.03.9
 """,
-        """backend.ai-common==23.03.8
+        """backend.ai-common==23.03.9
 """,
-        """backend.ai-kernel-binary==23.03.8
+        """backend.ai-kernel-binary==23.03.9
 """,
-        """backend.ai-kernel-helper==23.03.8
+        """backend.ai-kernel-helper==23.03.9
 """,
-        """backend.ai-kernel==23.03.8
+        """backend.ai-kernel==23.03.9
 """,
-        """backend.ai-plugin==23.03.8
+        """backend.ai-plugin==23.03.9
 """,
         'trafaret~=2.1',
     ),
     'license': 'LGPLv3',
     'long_description': """# backend.ai-accelerator-mock
 
 A mockup plugin for accelerators
@@ -75,11 +75,11 @@
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

