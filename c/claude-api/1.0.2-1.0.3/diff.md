# Comparing `tmp/claude-api-1.0.2.tar.gz` & `tmp/claude-api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claude-api-1.0.2.tar", last modified: Mon Jul 17 06:33:37 2023, max compression
+gzip compressed data, was "claude-api-1.0.3.tar", last modified: Mon Jul 17 06:40:58 2023, max compression
```

## Comparing `claude-api-1.0.2.tar` & `claude-api-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:33:37.671005 claude-api-1.0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-17 06:26:07.000000 claude-api-1.0.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     4480 2023-07-17 06:33:37.667005 claude-api-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3689 2023-07-17 06:26:07.000000 claude-api-1.0.2/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:33:37.667005 claude-api-1.0.2/claude-api/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:33:37.667005 claude-api-1.0.2/claude-api/claude_api.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     4480 2023-07-17 06:33:37.000000 claude-api-1.0.2/claude-api/claude_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      250 2023-07-17 06:33:37.000000 claude-api-1.0.2/claude-api/claude_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:33:37.000000 claude-api-1.0.2/claude-api/claude_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-17 06:33:37.000000 claude-api-1.0.2/claude-api/claude_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:33:37.000000 claude-api-1.0.2/claude-api/claude_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-17 06:33:37.671005 claude-api-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1178 2023-07-17 06:33:30.000000 claude-api-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:40:58.982162 claude-api-1.0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-17 06:39:39.000000 claude-api-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     4480 2023-07-17 06:40:58.982162 claude-api-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3689 2023-07-17 06:39:39.000000 claude-api-1.0.3/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:40:58.978162 claude-api-1.0.3/claude-api/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:40:58.982162 claude-api-1.0.3/claude-api/claude_api.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     4480 2023-07-17 06:40:58.000000 claude-api-1.0.3/claude-api/claude_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      250 2023-07-17 06:40:58.000000 claude-api-1.0.3/claude-api/claude_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:40:58.000000 claude-api-1.0.3/claude-api/claude_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-17 06:40:58.000000 claude-api-1.0.3/claude-api/claude_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:40:58.000000 claude-api-1.0.3/claude-api/claude_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-17 06:40:58.982162 claude-api-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1178 2023-07-17 06:40:28.000000 claude-api-1.0.3/setup.py
```

### Comparing `claude-api-1.0.2/LICENSE` & `claude-api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `claude-api-1.0.2/PKG-INFO` & `claude-api-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/KoushikNavuluri/Claude-API/
 Author: Koushik
 Author-email: navulurikoushik@outlook.com
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `claude-api-1.0.2/README.md` & `claude-api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `claude-api-1.0.2/claude-api/claude_api.egg-info/PKG-INFO` & `claude-api-1.0.3/claude-api/claude_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/KoushikNavuluri/Claude-API/
 Author: Koushik
 Author-email: navulurikoushik@outlook.com
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `claude-api-1.0.2/setup.py` & `claude-api-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 
 setup(
     name='claude-api', 
-    version='1.0.2',  
+    version='1.0.3',  
     author='Koushik',
     author_email='navulurikoushik@outlook.com',
     description='An unofficial API for Claude AI, allowing users to access and interact with Claude AII',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/KoushikNavuluri/Claude-API/', 
     packages=find_packages(),
```

