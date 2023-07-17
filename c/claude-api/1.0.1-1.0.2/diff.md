# Comparing `tmp/claude-api-1.0.1.tar.gz` & `tmp/claude-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claude-api-1.0.1.tar", last modified: Mon Jul 17 06:06:47 2023, max compression
+gzip compressed data, was "claude-api-1.0.2.tar", last modified: Mon Jul 17 06:33:37 2023, max compression
```

## Comparing `claude-api-1.0.1.tar` & `claude-api-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:06:47.646432 claude-api-1.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-17 06:03:36.000000 claude-api-1.0.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      898 2023-07-17 06:06:47.646432 claude-api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3448 2023-07-17 06:05:20.000000 claude-api-1.0.1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:06:47.642432 claude-api-1.0.1/claude_api/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:06:47.642432 claude-api-1.0.1/claude_api/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:06:47.646432 claude-api-1.0.1/claude_api/src/claude_api.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      898 2023-07-17 06:06:47.000000 claude-api-1.0.1/claude_api/src/claude_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      270 2023-07-17 06:06:47.000000 claude-api-1.0.1/claude_api/src/claude_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:06:47.000000 claude-api-1.0.1/claude_api/src/claude_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-17 06:06:47.000000 claude-api-1.0.1/claude_api/src/claude_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:06:47.000000 claude-api-1.0.1/claude_api/src/claude_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-17 06:06:47.646432 claude-api-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1274 2023-07-17 06:06:42.000000 claude-api-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:33:37.671005 claude-api-1.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-17 06:26:07.000000 claude-api-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     4480 2023-07-17 06:33:37.667005 claude-api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3689 2023-07-17 06:26:07.000000 claude-api-1.0.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:33:37.667005 claude-api-1.0.2/claude-api/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:33:37.667005 claude-api-1.0.2/claude-api/claude_api.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     4480 2023-07-17 06:33:37.000000 claude-api-1.0.2/claude-api/claude_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      250 2023-07-17 06:33:37.000000 claude-api-1.0.2/claude-api/claude_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:33:37.000000 claude-api-1.0.2/claude-api/claude_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-17 06:33:37.000000 claude-api-1.0.2/claude-api/claude_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:33:37.000000 claude-api-1.0.2/claude-api/claude_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-17 06:33:37.671005 claude-api-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1178 2023-07-17 06:33:30.000000 claude-api-1.0.2/setup.py
```

### Comparing `claude-api-1.0.1/LICENSE` & `claude-api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `claude-api-1.0.1/README.md` & `claude-api-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -36,18 +36,22 @@
 
     from claude_api import Client
 
 * Next, you need to create an instance of the Client class by providing your Claude AI cookie:
 
 * You can get cookie from the browser's developer tools network tab ( see for any claude.ai requests check out cookie ,copy whole value ) or storage tab ( You can find cookie of claude.ai ,there will be four values )
 
+* (Checkout below image for the format of cookie ,It is Better to Use from network tab to grab cookie easily )
 
-      cookie = os.environ.get('cookie')
-  
-      claude_api = Client(cookie)
+   ![Screenshot (8)](https://github.com/KoushikNavuluri/Claude-API/assets/103725723/355971e3-f46c-47fc-a3cf-008bb55bb4c6)
+
+
+        cookie = os.environ.get('cookie')
+    
+        claude_api = Client(cookie)
 
 ## List All Conversations
 
 To list all the conversation Id's you had with Claude , you can use the list_all_conversations method:
 
     conversations = claude_api.list_all_conversations()
     for conversation in conversations:
```

### Comparing `claude-api-1.0.1/setup.py` & `claude-api-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 from pathlib import Path
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 
 setup(
     name='claude-api', 
-    version='1.0.1',  
+    version='1.0.2',  
     author='Koushik',
     author_email='navulurikoushik@outlook.com',
     description='An unofficial API for Claude AI, allowing users to access and interact with Claude AII',
-    long_description='This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude A',
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/KoushikNavuluri/Claude-API/', 
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3',
         'Operating System :: Unix',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
     ],
     package_dir={
-    "": "claude_api/src"
+    "": "claude-api"
     },
     keywords=['claude', 'ai', 'claude-ai', 'API', 'requests', 'chatbot'],
     install_requires=[
         'requests'  
     ],
     python_requires=">=3.7",
 )
```

