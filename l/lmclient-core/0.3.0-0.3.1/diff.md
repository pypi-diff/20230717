# Comparing `tmp/lmclient_core-0.3.0.tar.gz` & `tmp/lmclient_core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmclient_core-0.3.0.tar", max compression
+gzip compressed data, was "lmclient_core-0.3.1.tar", max compression
```

## Comparing `lmclient_core-0.3.0.tar` & `lmclient_core-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-31 03:04:19.348371 lmclient_core-0.3.0/LICENSE
--rw-r--r--   0        0        0     3448 2023-07-13 11:01:26.959807 lmclient_core-0.3.0/README.md
--rw-r--r--   0        0        0      212 2023-07-13 10:42:16.420929 lmclient_core-0.3.0/lmclient/__init__.py
--rw-r--r--   0        0        0     6907 2023-07-13 10:55:54.493170 lmclient_core-0.3.0/lmclient/client.py
--rw-r--r--   0        0        0      117 2023-07-13 09:49:59.136022 lmclient_core-0.3.0/lmclient/models/__init__.py
--rw-r--r--   0        0        0     1516 2023-07-13 10:56:26.382623 lmclient_core-0.3.0/lmclient/models/azure.py
--rw-r--r--   0        0        0     1328 2023-07-13 11:00:57.629913 lmclient_core-0.3.0/lmclient/models/openai.py
--rw-r--r--   0        0        0      536 2023-07-13 10:42:15.726677 lmclient_core-0.3.0/lmclient/types.py
--rw-r--r--   0        0        0      690 2023-07-13 10:56:45.780077 lmclient_core-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 lmclient_core-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 03:04:19.348371 lmclient_core-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3448 2023-07-13 11:01:26.959807 lmclient_core-0.3.1/README.md
+-rw-r--r--   0        0        0      267 2023-07-17 10:03:19.077199 lmclient_core-0.3.1/lmclient/__init__.py
+-rw-r--r--   0        0        0     6899 2023-07-17 09:58:46.733361 lmclient_core-0.3.1/lmclient/client.py
+-rw-r--r--   0        0        0      180 2023-07-17 10:03:19.083039 lmclient_core-0.3.1/lmclient/models/__init__.py
+-rw-r--r--   0        0        0     1508 2023-07-17 09:58:46.733420 lmclient_core-0.3.1/lmclient/models/azure.py
+-rw-r--r--   0        0        0     3130 2023-07-17 10:17:07.464084 lmclient_core-0.3.1/lmclient/models/minimax.py
+-rw-r--r--   0        0        0     1320 2023-07-17 09:58:46.743029 lmclient_core-0.3.1/lmclient/models/openai.py
+-rw-r--r--   0        0        0      528 2023-07-17 09:58:46.733323 lmclient_core-0.3.1/lmclient/types.py
+-rw-r--r--   0        0        0      708 2023-07-17 10:45:16.502183 lmclient_core-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 lmclient_core-0.3.1/PKG-INFO
```

### Comparing `lmclient_core-0.3.0/LICENSE` & `lmclient_core-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmclient_core-0.3.0/README.md` & `lmclient_core-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lmclient_core-0.3.0/lmclient/client.py` & `lmclient_core-0.3.1/lmclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             async with task_created_lock:
                 sleep_time = self._calculate_sleep_time()
                 if sleep_time > 0:
                     await anyio.sleep(sleep_time)
                 self._task_created_time_list.append(int(time.time()))
 
             try:
-                completion = await self.completion_model.async_complete(prompt=prompt, **kwargs)
+                completion = await self.completion_model.async_chat(prompt=prompt, **kwargs)
                 if self.cache is not None:
                     self.cache[task_key] = completion
             except BaseException as e:
                 if self.error_mode is ErrorMode.RAISE:
                     raise
                 elif self.error_mode is ErrorMode.IGNORE:
                     completion: str = f'Error: {e}'
@@ -131,15 +131,15 @@
 
         sleep_time = self._calculate_sleep_time()
         if sleep_time > 0:
             time.sleep(sleep_time)
         self._task_created_time_list.append(int(time.time()))
 
         try:
-            completion = self.completion_model.complete(prompt=prompt, **kwargs)
+            completion = self.completion_model.chat(prompt=prompt, **kwargs)
             if self.cache is not None:
                 self.cache[task_key] = completion
         except BaseException as e:
             if self.error_mode is ErrorMode.RAISE:
                 raise
             elif self.error_mode is ErrorMode.IGNORE:
                 completion: str = f'Error: {e}'
```

### Comparing `lmclient_core-0.3.0/lmclient/models/azure.py` & `lmclient_core-0.3.1/lmclient/models/azure.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,23 @@
         self.model = model or os.environ['AZURE_CHAT_API_ENGINE']
 
         openai.api_type = 'azure'
         openai.api_key = api_key or os.environ['AZURE_API_KEY']
         openai.api_base = api_base or os.environ['AZURE_API_BASE']
         openai.api_version = api_version or os.getenv('AZURE_API_VERSION') or '2023-05-15'
 
-    def complete(self, prompt: Messages | str, **kwargs) -> str:
+    def chat(self, prompt: Messages | str, **kwargs) -> str:
         if isinstance(prompt, str):
             prompt = [Message(role='user', content=prompt)]
 
         response = openai.ChatCompletion.create(engine=self.model, messages=prompt, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
 
-    async def async_complete(self, prompt: Messages | str, **kwargs) -> str:
+    async def async_chat(self, prompt: Messages | str, **kwargs) -> str:
         if isinstance(prompt, str):
             prompt = [Message(role='user', content=prompt)]
 
         response = await openai.ChatCompletion.acreate(engine=self.model, messages=prompt, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
```

### Comparing `lmclient_core-0.3.0/lmclient/models/openai.py` & `lmclient_core-0.3.1/lmclient/models/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,23 @@
         self.model = model_name
 
         openai.api_type = 'open_ai'
         openai.api_base = 'https://api.openai.com/v1'
         openai.api_key = api_key or os.environ['OPENAI_API_KEY']
         openai.api_version = None
 
-    def complete(self, prompt: Messages | str, **kwargs) -> str:
+    def chat(self, prompt: Messages | str, **kwargs) -> str:
         if isinstance(prompt, str):
             prompt = [Message(role='user', content=prompt)]
 
         response = openai.ChatCompletion.create(model=self.model, messages=prompt, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
 
-    async def async_complete(self, prompt: Messages | str, **kwargs) -> str:
+    async def async_chat(self, prompt: Messages | str, **kwargs) -> str:
         if isinstance(prompt, str):
             prompt = [Message(role='user', content=prompt)]
 
         response = await openai.ChatCompletion.acreate(model=self.model, messages=prompt, **kwargs)
         completion: str = response.choices[0]['message']['content']  # type: ignore
         return completion
```

### Comparing `lmclient_core-0.3.0/lmclient/types.py` & `lmclient_core-0.3.1/lmclient/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 Messages = Sequence[Message]
 
 
 @runtime_checkable
 class ChatModel(Protocol):
     identifier: str
 
-    def complete(self, prompt: Messages | str, **kwargs) -> str:
+    def chat(self, prompt: Messages | str, **kwargs) -> str:
         ...
 
-    async def async_complete(self, prompt: Messages | str, **kwargs) -> str:
+    async def async_chat(self, prompt: Messages | str, **kwargs) -> str:
         ...
```

### Comparing `lmclient_core-0.3.0/pyproject.toml` & `lmclient_core-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "lmclient-core"
-version = "0.3.0"
+version = "0.3.1"
 description = "LM Async Client, openai client, azure openai client ..."
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "lmclient"}]
 repository = "https://github.com/wangyuxinwhy/lmclient"
 keywords = ["lmclient", "openai", "azure", "async"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 openai = "^0.27.7"
 asyncer = "0.0.2"
 typing-extensions = "^4.6.2"
 diskcache = "^5.6.1"
+httpx = "^0.24.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 blue = "^0.9.1"
 isort = "^5.12.0"
 pyright = "^1.1.310"
```

### Comparing `lmclient_core-0.3.0/PKG-INFO` & `lmclient_core-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmclient-core
-Version: 0.3.0
+Version: 0.3.1
 Summary: LM Async Client, openai client, azure openai client ...
 Home-page: https://github.com/wangyuxinwhy/lmclient
 License: Apache-2.0
 Keywords: lmclient,openai,azure,async
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.8,<4.0
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncer (==0.0.2)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
 Project-URL: Repository, https://github.com/wangyuxinwhy/lmclient
 Description-Content-Type: text/markdown
 
 # lmclient
```

