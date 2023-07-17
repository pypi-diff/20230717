# Comparing `tmp/backend.ai-kernel-helper-23.3.8.tar.gz` & `tmp/backend.ai-kernel-helper-23.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-helper-23.3.8.tar", last modified: Thu Jul  6 04:38:08 2023, max compression
+gzip compressed data, was "backend.ai-kernel-helper-23.3.9.tar", last modified: Mon Jul 17 14:35:59 2023, max compression
```

## Comparing `backend.ai-kernel-helper-23.3.8.tar` & `backend.ai-kernel-helper-23.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:08.664304 backend.ai-kernel-helper-23.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 04:38:07.000000 backend.ai-kernel-helper-23.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-06 04:38:08.664304 backend.ai-kernel-helper-23.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:08.664304 backend.ai-kernel-helper-23.3.8/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:08.664304 backend.ai-kernel-helper-23.3.8/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:08.664304 backend.ai-kernel-helper-23.3.8/ai/backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 04:38:07.000000 backend.ai-kernel-helper-23.3.8/ai/backend/helpers/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-06 04:38:07.000000 backend.ai-kernel-helper-23.3.8/ai/backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-06 04:38:07.000000 backend.ai-kernel-helper-23.3.8/ai/backend/helpers/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:08.664304 backend.ai-kernel-helper-23.3.8/backend.ai_kernel_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-06 04:38:08.000000 backend.ai-kernel-helper-23.3.8/backend.ai_kernel_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-06 04:38:08.000000 backend.ai-kernel-helper-23.3.8/backend.ai_kernel_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:08.000000 backend.ai-kernel-helper-23.3.8/backend.ai_kernel_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:08.000000 backend.ai-kernel-helper-23.3.8/backend.ai_kernel_helper.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:08.000000 backend.ai-kernel-helper-23.3.8/backend.ai_kernel_helper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 04:38:08.000000 backend.ai-kernel-helper-23.3.8/backend.ai_kernel_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 04:38:08.000000 backend.ai-kernel-helper-23.3.8/backend.ai_kernel_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 04:38:07.000000 backend.ai-kernel-helper-23.3.8/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 04:38:08.664304 backend.ai-kernel-helper-23.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-06 04:38:07.000000 backend.ai-kernel-helper-23.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:59.512602 backend.ai-kernel-helper-23.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 14:35:58.000000 backend.ai-kernel-helper-23.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-17 14:35:59.512602 backend.ai-kernel-helper-23.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:59.508602 backend.ai-kernel-helper-23.3.9/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:59.508602 backend.ai-kernel-helper-23.3.9/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:59.508602 backend.ai-kernel-helper-23.3.9/ai/backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:35:58.000000 backend.ai-kernel-helper-23.3.9/ai/backend/helpers/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 14:35:58.000000 backend.ai-kernel-helper-23.3.9/ai/backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-17 14:35:58.000000 backend.ai-kernel-helper-23.3.9/ai/backend/helpers/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:59.508602 backend.ai-kernel-helper-23.3.9/backend.ai_kernel_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-17 14:35:59.000000 backend.ai-kernel-helper-23.3.9/backend.ai_kernel_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-17 14:35:59.000000 backend.ai-kernel-helper-23.3.9/backend.ai_kernel_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:35:59.000000 backend.ai-kernel-helper-23.3.9/backend.ai_kernel_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:35:59.000000 backend.ai-kernel-helper-23.3.9/backend.ai_kernel_helper.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:35:59.000000 backend.ai-kernel-helper-23.3.9/backend.ai_kernel_helper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 14:35:59.000000 backend.ai-kernel-helper-23.3.9/backend.ai_kernel_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-17 14:35:59.000000 backend.ai-kernel-helper-23.3.9/backend.ai_kernel_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-17 14:35:58.000000 backend.ai-kernel-helper-23.3.9/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:35:59.512602 backend.ai-kernel-helper-23.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-17 14:35:58.000000 backend.ai-kernel-helper-23.3.9/setup.py
```

### Comparing `backend.ai-kernel-helper-23.3.8/PKG-INFO` & `backend.ai-kernel-helper-23.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel-helper
-Version: 23.3.8
+Version: 23.3.9
 Summary: Backend.AI Kernel Runner Prebuilt Binaries Package
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-helper-23.3.8/ai/backend/helpers/package.py` & `backend.ai-kernel-helper-23.3.9/ai/backend/helpers/package.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-helper-23.3.8/backend.ai_kernel_helper.egg-info/PKG-INFO` & `backend.ai-kernel-helper-23.3.9/backend.ai_kernel_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel-helper
-Version: 23.3.8
+Version: 23.3.9
 Summary: Backend.AI Kernel Runner Prebuilt Binaries Package
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-helper-23.3.8/backend_shim.py` & `backend.ai-kernel-helper-23.3.9/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-helper-23.3.8/setup.py` & `backend.ai-kernel-helper-23.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,11 +40,11 @@
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

