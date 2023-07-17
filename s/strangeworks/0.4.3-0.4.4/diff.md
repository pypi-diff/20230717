# Comparing `tmp/strangeworks-0.4.3.tar.gz` & `tmp/strangeworks-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks-0.4.3.tar", max compression
+gzip compressed data, was "strangeworks-0.4.4.tar", max compression
```

## Comparing `strangeworks-0.4.3.tar` & `strangeworks-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      222 2023-07-14 02:30:58.688727 strangeworks-0.4.3/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-07-14 02:30:58.688727 strangeworks-0.4.3/LICENSE
--rw-r--r--   0        0        0      795 2023-07-14 02:31:15.400779 strangeworks-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      756 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/__init__.py
--rw-r--r--   0        0        0       19 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/client/__init__.py
--rw-r--r--   0        0        0     1853 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/client/auth.py
--rw-r--r--   0        0        0     2950 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/client/backends.py
--rw-r--r--   0        0        0     4916 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/client/file.py
--rw-r--r--   0        0        0     5923 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/client/jobs.py
--rw-r--r--   0        0        0     4157 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/client/platform.py
--rw-r--r--   0        0        0     3005 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/client/resource.py
--rw-r--r--   0        0        0    10443 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/client/rest_client.py
--rw-r--r--   0        0        0     3276 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/client/transport.py
--rw-r--r--   0        0        0     1015 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/client/workspace.py
--rw-r--r--   0        0        0        0 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/config/__init__.py
--rw-r--r--   0        0        0     1647 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/config/base.py
--rw-r--r--   0        0        0     3855 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/config/config.py
--rw-r--r--   0        0        0      802 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/config/defaults.py
--rw-r--r--   0        0        0     1542 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/config/env.py
--rw-r--r--   0        0        0     6593 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/config/file.py
--rw-r--r--   0        0        0       17 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/errors/__init__.py
--rw-r--r--   0        0        0     2614 2023-07-14 02:30:58.688727 strangeworks-0.4.3/strangeworks/core/errors/error.py
--rw-r--r--   0        0        0      316 2023-07-14 02:30:58.692727 strangeworks-0.4.3/strangeworks/core/utils.py
--rw-r--r--   0        0        0    15221 2023-07-14 02:30:58.692727 strangeworks-0.4.3/strangeworks/sw_client.py
--rw-r--r--   0        0        0      323 2023-07-14 02:30:58.692727 strangeworks-0.4.3/strangeworks/utils.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 strangeworks-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      222 2023-07-17 20:59:35.019764 strangeworks-0.4.4/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-07-17 20:59:35.019764 strangeworks-0.4.4/LICENSE
+-rw-r--r--   0        0        0      795 2023-07-17 20:59:50.367936 strangeworks-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      756 2023-07-17 20:59:35.019764 strangeworks-0.4.4/strangeworks/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-17 20:59:35.019764 strangeworks-0.4.4/strangeworks/core/client/__init__.py
+-rw-r--r--   0        0        0     1853 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/client/auth.py
+-rw-r--r--   0        0        0     2950 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/client/backends.py
+-rw-r--r--   0        0        0     4916 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/client/file.py
+-rw-r--r--   0        0        0     5923 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/client/jobs.py
+-rw-r--r--   0        0        0     4157 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/client/platform.py
+-rw-r--r--   0        0        0     3005 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/client/resource.py
+-rw-r--r--   0        0        0    10443 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/client/rest_client.py
+-rw-r--r--   0        0        0     3276 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/client/transport.py
+-rw-r--r--   0        0        0     1015 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/client/workspace.py
+-rw-r--r--   0        0        0        0 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/config/__init__.py
+-rw-r--r--   0        0        0     1647 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/config/base.py
+-rw-r--r--   0        0        0     3855 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/config/config.py
+-rw-r--r--   0        0        0      802 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/config/defaults.py
+-rw-r--r--   0        0        0     1542 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/config/env.py
+-rw-r--r--   0        0        0     6593 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/config/file.py
+-rw-r--r--   0        0        0       17 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/errors/__init__.py
+-rw-r--r--   0        0        0     2614 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/errors/error.py
+-rw-r--r--   0        0        0      316 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/core/utils.py
+-rw-r--r--   0        0        0    15221 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/sw_client.py
+-rw-r--r--   0        0        0      323 2023-07-17 20:59:35.023764 strangeworks-0.4.4/strangeworks/utils.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 strangeworks-0.4.4/PKG-INFO
```

### Comparing `strangeworks-0.4.3/LICENSE` & `strangeworks-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/pyproject.toml` & `strangeworks-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "strangeworks"
-version = "0.4.3"
+version = "0.4.4"
 description = "Strangeworks Python SDK"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.30.0"
-pyyaml = "^5.4.1"
+pyyaml = "^6.0.0"
 tomlkit = "^0.11.1"
 gql = "^3.4.1"
 requests-toolbelt = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 black = "^22.1.0"
```

### Comparing `strangeworks-0.4.3/strangeworks/__init__.py` & `strangeworks-0.4.4/strangeworks/__init__.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/client/auth.py` & `strangeworks-0.4.4/strangeworks/core/client/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/client/backends.py` & `strangeworks-0.4.4/strangeworks/core/client/backends.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/client/file.py` & `strangeworks-0.4.4/strangeworks/core/client/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/client/jobs.py` & `strangeworks-0.4.4/strangeworks/core/client/jobs.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/client/platform.py` & `strangeworks-0.4.4/strangeworks/core/client/platform.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/client/resource.py` & `strangeworks-0.4.4/strangeworks/core/client/resource.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/client/rest_client.py` & `strangeworks-0.4.4/strangeworks/core/client/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/client/transport.py` & `strangeworks-0.4.4/strangeworks/core/client/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/client/workspace.py` & `strangeworks-0.4.4/strangeworks/core/client/workspace.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/config/base.py` & `strangeworks-0.4.4/strangeworks/core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/config/config.py` & `strangeworks-0.4.4/strangeworks/core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/config/defaults.py` & `strangeworks-0.4.4/strangeworks/core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/config/env.py` & `strangeworks-0.4.4/strangeworks/core/config/env.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/config/file.py` & `strangeworks-0.4.4/strangeworks/core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/core/errors/error.py` & `strangeworks-0.4.4/strangeworks/core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/strangeworks/sw_client.py` & `strangeworks-0.4.4/strangeworks/sw_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.4.3/PKG-INFO` & `strangeworks-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strangeworks
-Version: 0.4.3
+Version: 0.4.4
 Summary: Strangeworks Python SDK
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gql (>=3.4.1,<4.0.0)
-Requires-Dist: pyyaml (>=5.4.1,<6.0.0)
+Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: tomlkit (>=0.11.1,<0.12.0)
 Description-Content-Type: text/markdown
 
 # Strangeworks SDK
```

