# Comparing `tmp/claude-api-1.0.3.tar.gz` & `tmp/claude-api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claude-api-1.0.3.tar", last modified: Mon Jul 17 06:40:58 2023, max compression
+gzip compressed data, was "claude-api-1.0.4.tar", last modified: Mon Jul 17 06:59:16 2023, max compression
```

## Comparing `claude-api-1.0.3.tar` & `claude-api-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:40:58.982162 claude-api-1.0.3/
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-17 06:39:39.000000 claude-api-1.0.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     4480 2023-07-17 06:40:58.982162 claude-api-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3689 2023-07-17 06:39:39.000000 claude-api-1.0.3/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:40:58.978162 claude-api-1.0.3/claude-api/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 06:40:58.982162 claude-api-1.0.3/claude-api/claude_api.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     4480 2023-07-17 06:40:58.000000 claude-api-1.0.3/claude-api/claude_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      250 2023-07-17 06:40:58.000000 claude-api-1.0.3/claude-api/claude_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:40:58.000000 claude-api-1.0.3/claude-api/claude_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-17 06:40:58.000000 claude-api-1.0.3/claude-api/claude_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 06:40:58.000000 claude-api-1.0.3/claude-api/claude_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-17 06:40:58.982162 claude-api-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1178 2023-07-17 06:40:28.000000 claude-api-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:59:16.908285 claude-api-1.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-07-17 06:55:41.000000 claude-api-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4642 2023-07-17 06:59:16.904933 claude-api-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3824 2023-07-17 06:55:41.000000 claude-api-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 06:59:16.883782 claude-api-1.0.4/claude-api/
+drwxrwxrwx   0        0        0        0 2023-07-17 06:59:16.900960 claude-api-1.0.4/claude-api/claude_api.egg-info/
+-rw-rw-rw-   0        0        0     4642 2023-07-17 06:59:16.000000 claude-api-1.0.4/claude-api/claude_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-17 06:59:16.000000 claude-api-1.0.4/claude-api/claude_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:59:16.000000 claude-api-1.0.4/claude-api/claude_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 06:59:16.000000 claude-api-1.0.4/claude-api/claude_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 06:59:16.000000 claude-api-1.0.4/claude-api/claude_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7694 2023-07-17 06:55:41.000000 claude-api-1.0.4/claude-api/claude_api.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 06:59:16.908285 claude-api-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-07-17 06:59:05.000000 claude-api-1.0.4/setup.py
```

### Comparing `claude-api-1.0.3/LICENSE` & `claude-api-1.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Koushik Navuluri
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Koushik Navuluri
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `claude-api-1.0.3/PKG-INFO` & `claude-api-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,155 +1,156 @@
-Metadata-Version: 2.1
-Name: claude-api
-Version: 1.0.3
-Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
-Home-page: https://github.com/KoushikNavuluri/Claude-API/
-Author: Koushik
-Author-email: navulurikoushik@outlook.com
-Keywords: claude,ai,claude-ai,API,requests,chatbot
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Claude AI-API ( Unofficial )
-This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude AI .
-
-## Use Cases 
-
-    1. Python Console ChatBot
-
-    2. Discord Chatbot   
-    
-    3. Many more can be done....
-    
-
-## Prerequisites
-
-To use this API, you need to have the following:
-
-Python installed on your system
-requests library installed 
-```bash
-  pip install requests
-
-```
-
-## Installation
-
-To use the Claude AI Unofficial API, you can either clone the GitHub repository or directly download the Python file.
-
-Clone the repository:
-
-    git clone https://github.com/KoushikNavuluri/Claude-API.git
-
-## Usage
-
-
-Import the claude_api module in your Python script:
-
-    from claude_api import Client
-
-* Next, you need to create an instance of the Client class by providing your Claude AI cookie:
-
-* You can get cookie from the browser's developer tools network tab ( see for any claude.ai requests check out cookie ,copy whole value ) or storage tab ( You can find cookie of claude.ai ,there will be four values )
-
-* (Checkout below image for the format of cookie ,It is Better to Use from network tab to grab cookie easily )
-
-   ![Screenshot (8)](https://github.com/KoushikNavuluri/Claude-API/assets/103725723/355971e3-f46c-47fc-a3cf-008bb55bb4c6)
-
-
-        cookie = os.environ.get('cookie')
-    
-        claude_api = Client(cookie)
-
-## List All Conversations
-
-To list all the conversation Id's you had with Claude , you can use the list_all_conversations method:
-
-    conversations = claude_api.list_all_conversations()
-    for conversation in conversations:
-        conversation_id = conversation['uuid']
-        print(conversation_id)
-
-## Send Message
-
-To send a message to Claude, you can use the send_message method. You need to provide the prompt and the conversation ID:
-
-
-
-    prompt = "Hello, Claude!"
-    conversation_id = "<conversation_id>"
-    response = claude_api.send_message(prompt, conversation_id)
-    print(response)
-
-## Delete Conversation
-
-To delete a conversation, you can use the delete_conversation method:
-
-
-    conversation_id = "<conversation_id>"
-    deleted = claude_api.delete_conversation(conversation_id)
-    if deleted:
-        print("Conversation deleted successfully")
-    else:
-        print("Failed to delete conversation")
-
-## Chat Conversation History
-
-To get the chat conversation history, you can use the chat_conversation_history method:    
-
-    conversation_id = "<conversation_id>"
-    history = claude_api.chat_conversation_history(conversation_id)
-    print(history)
-
-## Create New Chat
-
-To create a new chat conversation (id), you can use the create_new_chat method:
-
-
-    new_chat = claude_api.create_new_chat()
-    conversation_id = new_chat['uuid']
-    print(conversation_id)
-
-## Reset All Conversations
-
-To reset all conversations, you can use the reset_all method:
-
-
-    reset = claude_api.reset_all()
-    if reset:
-        print("All conversations reset successfully")
-    else:
-        print("Failed to reset conversations")   
-
-## Rename Chat
-
-To rename a chat conversation, you can use the rename_chat method:
-
-    conversation_id = "<conversation_id>"
-    title = "New Chat Title"
-    renamed = claude_api.rename_chat(title, conversation_id)
-    if renamed:
-        print("Chat conversation renamed successfully")
-    else:
-        print("Failed to rename chat conversation")
-
-## Disclaimer
-
-This project provides an unofficial API for Claude AI and is not affiliated with or endorsed by Claude AI or Anthropic. Use it at your own risk.
-
-Please refer to the official Claude AI documentation[https://claude.ai/docs] for more information on how to use Claude AI.
-        
-    
-
-
-
-
-    
+Metadata-Version: 2.1
+Name: claude-api
+Version: 1.0.4
+Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
+Home-page: https://github.com/KoushikNavuluri/Claude-API/
+Author: Koushik
+Author-email: koushikk@outlook.com
+License: MIT
+Keywords: claude,ai,claude-ai,API,requests,chatbot
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Claude AI-API ( Unofficial )
+This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude AI .
+
+## Use Cases 
+
+    1. Python Console ChatBot
+
+    2. Discord Chatbot   
+    
+    3. Many more can be done....
+    
+
+## Prerequisites
+
+To use this API, you need to have the following:
+
+Python installed on your system
+requests library installed 
+```bash
+  pip install requests
+
+```
+
+## Installation
+
+To use the Claude AI Unofficial API, you can either clone the GitHub repository or directly download the Python file.
+
+Clone the repository:
+
+    git clone https://github.com/KoushikNavuluri/Claude-API.git
+
+## Usage
+
+
+Import the claude_api module in your Python script:
+
+    from claude_api import Client
+
+* Next, you need to create an instance of the Client class by providing your Claude AI cookie:
+
+* You can get cookie from the browser's developer tools network tab ( see for any claude.ai requests check out cookie ,copy whole value ) or storage tab ( You can find cookie of claude.ai ,there will be four values )
+
+* (Checkout below image for the format of cookie ,It is Better to Use from network tab to grab cookie easily )
+
+   ![Screenshot (8)](https://github.com/KoushikNavuluri/Claude-API/assets/103725723/355971e3-f46c-47fc-a3cf-008bb55bb4c6)
+
+
+        cookie = os.environ.get('cookie')
+    
+        claude_api = Client(cookie)
+
+## List All Conversations
+
+To list all the conversation Id's you had with Claude , you can use the list_all_conversations method:
+
+    conversations = claude_api.list_all_conversations()
+    for conversation in conversations:
+        conversation_id = conversation['uuid']
+        print(conversation_id)
+
+## Send Message
+
+To send a message to Claude, you can use the send_message method. You need to provide the prompt and the conversation ID:
+
+
+
+    prompt = "Hello, Claude!"
+    conversation_id = "<conversation_id>"
+    response = claude_api.send_message(prompt, conversation_id)
+    print(response)
+
+## Delete Conversation
+
+To delete a conversation, you can use the delete_conversation method:
+
+
+    conversation_id = "<conversation_id>"
+    deleted = claude_api.delete_conversation(conversation_id)
+    if deleted:
+        print("Conversation deleted successfully")
+    else:
+        print("Failed to delete conversation")
+
+## Chat Conversation History
+
+To get the chat conversation history, you can use the chat_conversation_history method:    
+
+    conversation_id = "<conversation_id>"
+    history = claude_api.chat_conversation_history(conversation_id)
+    print(history)
+
+## Create New Chat
+
+To create a new chat conversation (id), you can use the create_new_chat method:
+
+
+    new_chat = claude_api.create_new_chat()
+    conversation_id = new_chat['uuid']
+    print(conversation_id)
+
+## Reset All Conversations
+
+To reset all conversations, you can use the reset_all method:
+
+
+    reset = claude_api.reset_all()
+    if reset:
+        print("All conversations reset successfully")
+    else:
+        print("Failed to reset conversations")   
+
+## Rename Chat
+
+To rename a chat conversation, you can use the rename_chat method:
+
+    conversation_id = "<conversation_id>"
+    title = "New Chat Title"
+    renamed = claude_api.rename_chat(title, conversation_id)
+    if renamed:
+        print("Chat conversation renamed successfully")
+    else:
+        print("Failed to rename chat conversation")
+
+## Disclaimer
+
+This project provides an unofficial API for Claude AI and is not affiliated with or endorsed by Claude AI or Anthropic. Use it at your own risk.
+
+Please refer to the official Claude AI documentation[https://claude.ai/docs] for more information on how to use Claude AI.
+        
+    
+
+
+
+
+
```

### Comparing `claude-api-1.0.3/README.md` & `claude-api-1.0.4/claude-api/claude_api.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,135 +1,156 @@
-# Claude AI-API ( Unofficial )
-This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude AI .
-
-## Use Cases 
-
-    1. Python Console ChatBot
-
-    2. Discord Chatbot   
-    
-    3. Many more can be done....
-    
-
-## Prerequisites
-
-To use this API, you need to have the following:
-
-Python installed on your system
-requests library installed 
-```bash
-  pip install requests
-
-```
-
-## Installation
-
-To use the Claude AI Unofficial API, you can either clone the GitHub repository or directly download the Python file.
-
-Clone the repository:
-
-    git clone https://github.com/KoushikNavuluri/Claude-API.git
-
-## Usage
-
-
-Import the claude_api module in your Python script:
-
-    from claude_api import Client
-
-* Next, you need to create an instance of the Client class by providing your Claude AI cookie:
-
-* You can get cookie from the browser's developer tools network tab ( see for any claude.ai requests check out cookie ,copy whole value ) or storage tab ( You can find cookie of claude.ai ,there will be four values )
-
-* (Checkout below image for the format of cookie ,It is Better to Use from network tab to grab cookie easily )
-
-   ![Screenshot (8)](https://github.com/KoushikNavuluri/Claude-API/assets/103725723/355971e3-f46c-47fc-a3cf-008bb55bb4c6)
-
-
-        cookie = os.environ.get('cookie')
-    
-        claude_api = Client(cookie)
-
-## List All Conversations
-
-To list all the conversation Id's you had with Claude , you can use the list_all_conversations method:
-
-    conversations = claude_api.list_all_conversations()
-    for conversation in conversations:
-        conversation_id = conversation['uuid']
-        print(conversation_id)
-
-## Send Message
-
-To send a message to Claude, you can use the send_message method. You need to provide the prompt and the conversation ID:
-
-
-
-    prompt = "Hello, Claude!"
-    conversation_id = "<conversation_id>"
-    response = claude_api.send_message(prompt, conversation_id)
-    print(response)
-
-## Delete Conversation
-
-To delete a conversation, you can use the delete_conversation method:
-
-
-    conversation_id = "<conversation_id>"
-    deleted = claude_api.delete_conversation(conversation_id)
-    if deleted:
-        print("Conversation deleted successfully")
-    else:
-        print("Failed to delete conversation")
-
-## Chat Conversation History
-
-To get the chat conversation history, you can use the chat_conversation_history method:    
-
-    conversation_id = "<conversation_id>"
-    history = claude_api.chat_conversation_history(conversation_id)
-    print(history)
-
-## Create New Chat
-
-To create a new chat conversation (id), you can use the create_new_chat method:
-
-
-    new_chat = claude_api.create_new_chat()
-    conversation_id = new_chat['uuid']
-    print(conversation_id)
-
-## Reset All Conversations
-
-To reset all conversations, you can use the reset_all method:
-
-
-    reset = claude_api.reset_all()
-    if reset:
-        print("All conversations reset successfully")
-    else:
-        print("Failed to reset conversations")   
-
-## Rename Chat
-
-To rename a chat conversation, you can use the rename_chat method:
-
-    conversation_id = "<conversation_id>"
-    title = "New Chat Title"
-    renamed = claude_api.rename_chat(title, conversation_id)
-    if renamed:
-        print("Chat conversation renamed successfully")
-    else:
-        print("Failed to rename chat conversation")
-
-## Disclaimer
-
-This project provides an unofficial API for Claude AI and is not affiliated with or endorsed by Claude AI or Anthropic. Use it at your own risk.
-
-Please refer to the official Claude AI documentation[https://claude.ai/docs] for more information on how to use Claude AI.
-        
-    
-
-
-
-
-    
+Metadata-Version: 2.1
+Name: claude-api
+Version: 1.0.4
+Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
+Home-page: https://github.com/KoushikNavuluri/Claude-API/
+Author: Koushik
+Author-email: koushikk@outlook.com
+License: MIT
+Keywords: claude,ai,claude-ai,API,requests,chatbot
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Claude AI-API ( Unofficial )
+This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude AI .
+
+## Use Cases 
+
+    1. Python Console ChatBot
+
+    2. Discord Chatbot   
+    
+    3. Many more can be done....
+    
+
+## Prerequisites
+
+To use this API, you need to have the following:
+
+Python installed on your system
+requests library installed 
+```bash
+  pip install requests
+
+```
+
+## Installation
+
+To use the Claude AI Unofficial API, you can either clone the GitHub repository or directly download the Python file.
+
+Clone the repository:
+
+    git clone https://github.com/KoushikNavuluri/Claude-API.git
+
+## Usage
+
+
+Import the claude_api module in your Python script:
+
+    from claude_api import Client
+
+* Next, you need to create an instance of the Client class by providing your Claude AI cookie:
+
+* You can get cookie from the browser's developer tools network tab ( see for any claude.ai requests check out cookie ,copy whole value ) or storage tab ( You can find cookie of claude.ai ,there will be four values )
+
+* (Checkout below image for the format of cookie ,It is Better to Use from network tab to grab cookie easily )
+
+   ![Screenshot (8)](https://github.com/KoushikNavuluri/Claude-API/assets/103725723/355971e3-f46c-47fc-a3cf-008bb55bb4c6)
+
+
+        cookie = os.environ.get('cookie')
+    
+        claude_api = Client(cookie)
+
+## List All Conversations
+
+To list all the conversation Id's you had with Claude , you can use the list_all_conversations method:
+
+    conversations = claude_api.list_all_conversations()
+    for conversation in conversations:
+        conversation_id = conversation['uuid']
+        print(conversation_id)
+
+## Send Message
+
+To send a message to Claude, you can use the send_message method. You need to provide the prompt and the conversation ID:
+
+
+
+    prompt = "Hello, Claude!"
+    conversation_id = "<conversation_id>"
+    response = claude_api.send_message(prompt, conversation_id)
+    print(response)
+
+## Delete Conversation
+
+To delete a conversation, you can use the delete_conversation method:
+
+
+    conversation_id = "<conversation_id>"
+    deleted = claude_api.delete_conversation(conversation_id)
+    if deleted:
+        print("Conversation deleted successfully")
+    else:
+        print("Failed to delete conversation")
+
+## Chat Conversation History
+
+To get the chat conversation history, you can use the chat_conversation_history method:    
+
+    conversation_id = "<conversation_id>"
+    history = claude_api.chat_conversation_history(conversation_id)
+    print(history)
+
+## Create New Chat
+
+To create a new chat conversation (id), you can use the create_new_chat method:
+
+
+    new_chat = claude_api.create_new_chat()
+    conversation_id = new_chat['uuid']
+    print(conversation_id)
+
+## Reset All Conversations
+
+To reset all conversations, you can use the reset_all method:
+
+
+    reset = claude_api.reset_all()
+    if reset:
+        print("All conversations reset successfully")
+    else:
+        print("Failed to reset conversations")   
+
+## Rename Chat
+
+To rename a chat conversation, you can use the rename_chat method:
+
+    conversation_id = "<conversation_id>"
+    title = "New Chat Title"
+    renamed = claude_api.rename_chat(title, conversation_id)
+    if renamed:
+        print("Chat conversation renamed successfully")
+    else:
+        print("Failed to rename chat conversation")
+
+## Disclaimer
+
+This project provides an unofficial API for Claude AI and is not affiliated with or endorsed by Claude AI or Anthropic. Use it at your own risk.
+
+Please refer to the official Claude AI documentation[https://claude.ai/docs] for more information on how to use Claude AI.
+        
+    
+
+
+
+
+
```

### Comparing `claude-api-1.0.3/setup.py` & `claude-api-1.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-from setuptools import setup, find_packages
-from pathlib import Path
-base_path = Path(__file__).parent
-long_description = (base_path / "README.md").read_text()
-
-
-setup(
-    name='claude-api', 
-    version='1.0.3',  
-    author='Koushik',
-    author_email='navulurikoushik@outlook.com',
-    description='An unofficial API for Claude AI, allowing users to access and interact with Claude AII',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/KoushikNavuluri/Claude-API/', 
-    packages=find_packages(),
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3',
-        'Operating System :: Unix',
-        'Operating System :: MacOS :: MacOS X',
-        'Operating System :: Microsoft :: Windows',
-    ],
-    package_dir={
-    "": "claude-api"
-    },
-    keywords=['claude', 'ai', 'claude-ai', 'API', 'requests', 'chatbot'],
-    install_requires=[
-        'requests'  
-    ],
-    python_requires=">=3.7",
-)
+from setuptools import setup, find_packages
+from pathlib import Path
+base_path = Path(__file__).parent
+long_description = (base_path / "README.md").read_text()
+
+
+setup(
+    name='claude-api', 
+    version='1.0.4',  
+    author='Koushik',
+    license="MIT",
+    author_email='koushikk@outlook.com',
+    description='An unofficial API for Claude AI, allowing users to access and interact with Claude AII',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/KoushikNavuluri/Claude-API/', 
+    packages=find_packages(),
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3',
+        'Operating System :: Unix',
+        'Operating System :: MacOS :: MacOS X',
+        'Operating System :: Microsoft :: Windows',
+    ],
+    package_dir={
+    "": "claude-api"
+    },
+    py_modules=["claude_api"],
+    keywords=['claude', 'ai', 'claude-ai', 'API', 'requests', 'chatbot'],
+    install_requires=[
+        'requests'  
+    ],
+    python_requires=">=3.7",
+)
```

