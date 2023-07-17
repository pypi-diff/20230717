# Comparing `tmp/claude-api-1.0.4.tar.gz` & `tmp/claude-api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claude-api-1.0.4.tar", last modified: Mon Jul 17 06:59:16 2023, max compression
+gzip compressed data, was "claude-api-1.0.5.tar", last modified: Mon Jul 17 07:06:06 2023, max compression
```

## Comparing `claude-api-1.0.4.tar` & `claude-api-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 06:59:16.908285 claude-api-1.0.4/
--rw-rw-rw-   0        0        0     1094 2023-07-17 06:55:41.000000 claude-api-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     4642 2023-07-17 06:59:16.904933 claude-api-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3824 2023-07-17 06:55:41.000000 claude-api-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 06:59:16.883782 claude-api-1.0.4/claude-api/
-drwxrwxrwx   0        0        0        0 2023-07-17 06:59:16.900960 claude-api-1.0.4/claude-api/claude_api.egg-info/
--rw-rw-rw-   0        0        0     4642 2023-07-17 06:59:16.000000 claude-api-1.0.4/claude-api/claude_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-17 06:59:16.000000 claude-api-1.0.4/claude-api/claude_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 06:59:16.000000 claude-api-1.0.4/claude-api/claude_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 06:59:16.000000 claude-api-1.0.4/claude-api/claude_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 06:59:16.000000 claude-api-1.0.4/claude-api/claude_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7694 2023-07-17 06:55:41.000000 claude-api-1.0.4/claude-api/claude_api.py
--rw-rw-rw-   0        0        0       42 2023-07-17 06:59:16.908285 claude-api-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1258 2023-07-17 06:59:05.000000 claude-api-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:06:06.217369 claude-api-1.0.5/
+-rw-rw-rw-   0        0        0     1094 2023-07-17 06:55:41.000000 claude-api-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4642 2023-07-17 07:06:06.217369 claude-api-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3824 2023-07-17 06:55:41.000000 claude-api-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 07:06:06.195729 claude-api-1.0.5/claude-api/
+drwxrwxrwx   0        0        0        0 2023-07-17 07:06:06.211415 claude-api-1.0.5/claude-api/claude_api.egg-info/
+-rw-rw-rw-   0        0        0     4642 2023-07-17 07:06:06.000000 claude-api-1.0.5/claude-api/claude_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-17 07:06:06.000000 claude-api-1.0.5/claude-api/claude_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 07:06:06.000000 claude-api-1.0.5/claude-api/claude_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 07:06:06.000000 claude-api-1.0.5/claude-api/claude_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 07:06:06.000000 claude-api-1.0.5/claude-api/claude_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7623 2023-07-17 07:04:57.000000 claude-api-1.0.5/claude-api/claude_api.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 07:06:06.217369 claude-api-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-07-17 07:05:56.000000 claude-api-1.0.5/setup.py
```

### Comparing `claude-api-1.0.4/LICENSE` & `claude-api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `claude-api-1.0.4/PKG-INFO` & `claude-api-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/KoushikNavuluri/Claude-API/
 Author: Koushik
 Author-email: koushikk@outlook.com
 License: MIT
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `claude-api-1.0.4/README.md` & `claude-api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `claude-api-1.0.4/claude-api/claude_api.egg-info/PKG-INFO` & `claude-api-1.0.5/claude-api/claude_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/KoushikNavuluri/Claude-API/
 Author: Koushik
 Author-email: koushikk@outlook.com
 License: MIT
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `claude-api-1.0.4/claude-api/claude_api.py` & `claude-api-1.0.5/claude-api/claude_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     self.organization_id = self.get_organization_id()
 
   def get_organization_id(self):
     url = "https://claude.ai/api/organizations"
   
     headers = {
       'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
-      'Accept': '*/*',
       'Accept-Language': 'en-US,en;q=0.5',
-      'Accept-Encoding': 'gzip, deflate, br',
       'Referer': 'https://claude.ai/chats',
       'Content-Type': 'application/json',
       'Sec-Fetch-Dest': 'empty',
       'Sec-Fetch-Mode': 'cors',
       'Sec-Fetch-Site': 'same-origin',
       'Connection': 'keep-alive',
       'Cookie': f'{self.cookie}'
```

### Comparing `claude-api-1.0.4/setup.py` & `claude-api-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 
 setup(
     name='claude-api', 
-    version='1.0.4',  
+    version='1.0.5',  
     author='Koushik',
     license="MIT",
     author_email='koushikk@outlook.com',
     description='An unofficial API for Claude AI, allowing users to access and interact with Claude AII',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/KoushikNavuluri/Claude-API/',
```

