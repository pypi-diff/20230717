# Comparing `tmp/claude-api-1.0.0.tar.gz` & `tmp/claude-api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claude-api-1.0.0.tar", last modified: Mon Jul 17 05:40:32 2023, max compression
+gzip compressed data, was "claude-api-1.0.1.tar", last modified: Mon Jul 17 06:06:47 2023, max compression
```

## Comparing `claude-api-1.0.0.tar` & `claude-api-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 05:40:32.379299 claude-api-1.0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-17 05:36:02.000000 claude-api-1.0.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      898 2023-07-17 05:40:32.379299 claude-api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3688 2023-07-17 05:36:02.000000 claude-api-1.0.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 05:40:32.375299 claude-api-1.0.0/claude_api.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      898 2023-07-17 05:40:32.000000 claude-api-1.0.0/claude_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      195 2023-07-17 05:40:32.000000 claude-api-1.0.0/claude_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 05:40:32.000000 claude-api-1.0.0/claude_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-17 05:40:32.000000 claude-api-1.0.0/claude_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 05:40:32.000000 claude-api-1.0.0/claude_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-17 05:40:32.383299 claude-api-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1107 2023-07-17 05:39:44.000000 claude-api-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:06:47.646432 claude-api-1.0.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-17 06:03:36.000000 claude-api-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      898 2023-07-17 06:06:47.646432 claude-api-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3448 2023-07-17 06:05:20.000000 claude-api-1.0.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:06:47.642432 claude-api-1.0.1/claude_api/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:06:47.642432 claude-api-1.0.1/claude_api/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:06:47.646432 claude-api-1.0.1/claude_api/src/claude_api.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      898 2023-07-17 06:06:47.000000 claude-api-1.0.1/claude_api/src/claude_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      270 2023-07-17 06:06:47.000000 claude-api-1.0.1/claude_api/src/claude_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:06:47.000000 claude-api-1.0.1/claude_api/src/claude_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-17 06:06:47.000000 claude-api-1.0.1/claude_api/src/claude_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:06:47.000000 claude-api-1.0.1/claude_api/src/claude_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-17 06:06:47.646432 claude-api-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1274 2023-07-17 06:06:42.000000 claude-api-1.0.1/setup.py
```

### Comparing `claude-api-1.0.0/LICENSE` & `claude-api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `claude-api-1.0.0/PKG-INFO` & `claude-api-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/KoushikNavuluri/Claude-API/
 Author: Koushik
 Author-email: navulurikoushik@outlook.com
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `claude-api-1.0.0/README.md` & `claude-api-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,28 +30,24 @@
     git clone https://github.com/KoushikNavuluri/Claude-API.git
 
 ## Usage
 
 
 Import the claude_api module in your Python script:
 
-    from claude_ai import Client
+    from claude_api import Client
 
 * Next, you need to create an instance of the Client class by providing your Claude AI cookie:
 
 * You can get cookie from the browser's developer tools network tab ( see for any claude.ai requests check out cookie ,copy whole value ) or storage tab ( You can find cookie of claude.ai ,there will be four values )
 
-* (Checkout below image for the format of cookie ,It is Better to Use from network tab to grab cookie easily )
 
-   ![Screenshot (8)](https://github.com/KoushikNavuluri/Claude-API/assets/103725723/355971e3-f46c-47fc-a3cf-008bb55bb4c6)
-
-
-        cookie = os.environ.get('cookie')
-    
-        claude_api = Client(cookie)
+      cookie = os.environ.get('cookie')
+  
+      claude_api = Client(cookie)
 
 ## List All Conversations
 
 To list all the conversation Id's you had with Claude , you can use the list_all_conversations method:
 
     conversations = claude_api.list_all_conversations()
     for conversation in conversations:
```

### Comparing `claude-api-1.0.0/claude_api.egg-info/PKG-INFO` & `claude-api-1.0.1/claude_api/src/claude_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/KoushikNavuluri/Claude-API/
 Author: Koushik
 Author-email: navulurikoushik@outlook.com
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `claude-api-1.0.0/setup.py` & `claude-api-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+base_path = Path(__file__).parent
+long_description = (base_path / "README.md").read_text()
+
 
 setup(
     name='claude-api', 
-    version='1.0.0',  
+    version='1.0.1',  
     author='Koushik',
     author_email='navulurikoushik@outlook.com',
     description='An unofficial API for Claude AI, allowing users to access and interact with Claude AII',
     long_description='This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude A',
     long_description_content_type='text/markdown',
     url='https://github.com/KoushikNavuluri/Claude-API/', 
     packages=find_packages(),
@@ -16,13 +20,16 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3',
         'Operating System :: Unix',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
     ],
+    package_dir={
+    "": "claude_api/src"
+    },
     keywords=['claude', 'ai', 'claude-ai', 'API', 'requests', 'chatbot'],
     install_requires=[
         'requests'  
     ],
     python_requires=">=3.7",
 )
```

