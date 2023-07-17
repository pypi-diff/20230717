# Comparing `tmp/lmclient_core-0.3.1.tar.gz` & `tmp/lmclient_core-0.3.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmclient_core-0.3.1.tar", max compression
+gzip compressed data, was "lmclient_core-0.3.1.post1.tar", max compression
```

## Comparing `lmclient_core-0.3.1.tar` & `lmclient_core-0.3.1.post1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-31 03:04:19.348371 lmclient_core-0.3.1/LICENSE
--rw-r--r--   0        0        0     3448 2023-07-13 11:01:26.959807 lmclient_core-0.3.1/README.md
--rw-r--r--   0        0        0      267 2023-07-17 10:03:19.077199 lmclient_core-0.3.1/lmclient/__init__.py
--rw-r--r--   0        0        0     6899 2023-07-17 09:58:46.733361 lmclient_core-0.3.1/lmclient/client.py
--rw-r--r--   0        0        0      180 2023-07-17 10:03:19.083039 lmclient_core-0.3.1/lmclient/models/__init__.py
--rw-r--r--   0        0        0     1508 2023-07-17 09:58:46.733420 lmclient_core-0.3.1/lmclient/models/azure.py
--rw-r--r--   0        0        0     3130 2023-07-17 10:17:07.464084 lmclient_core-0.3.1/lmclient/models/minimax.py
--rw-r--r--   0        0        0     1320 2023-07-17 09:58:46.743029 lmclient_core-0.3.1/lmclient/models/openai.py
--rw-r--r--   0        0        0      528 2023-07-17 09:58:46.733323 lmclient_core-0.3.1/lmclient/types.py
--rw-r--r--   0        0        0      708 2023-07-17 10:45:16.502183 lmclient_core-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 lmclient_core-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 03:04:19.348371 lmclient_core-0.3.1.post1/LICENSE
+-rw-r--r--   0        0        0     3448 2023-07-13 11:01:26.959807 lmclient_core-0.3.1.post1/README.md
+-rw-r--r--   0        0        0      267 2023-07-17 10:03:19.077199 lmclient_core-0.3.1.post1/lmclient/__init__.py
+-rw-r--r--   0        0        0     6616 2023-07-17 11:04:36.330778 lmclient_core-0.3.1.post1/lmclient/client.py
+-rw-r--r--   0        0        0      180 2023-07-17 10:03:19.083039 lmclient_core-0.3.1.post1/lmclient/models/__init__.py
+-rw-r--r--   0        0        0     1928 2023-07-17 11:41:21.947835 lmclient_core-0.3.1.post1/lmclient/models/azure.py
+-rw-r--r--   0        0        0     3638 2023-07-17 11:40:37.180751 lmclient_core-0.3.1.post1/lmclient/models/minimax.py
+-rw-r--r--   0        0        0     1740 2023-07-17 11:41:09.589953 lmclient_core-0.3.1.post1/lmclient/models/openai.py
+-rw-r--r--   0        0        0      554 2023-07-17 11:01:15.271410 lmclient_core-0.3.1.post1/lmclient/types.py
+-rw-r--r--   0        0        0      714 2023-07-17 11:41:46.142182 lmclient_core-0.3.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 lmclient_core-0.3.1.post1/PKG-INFO
```

### Comparing `lmclient_core-0.3.1/LICENSE` & `lmclient_core-0.3.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmclient_core-0.3.1/README.md` & `lmclient_core-0.3.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `lmclient_core-0.3.1/lmclient/client.py` & `lmclient_core-0.3.1.post1/lmclient/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,41 +34,36 @@
         max_requests_per_minute: int = 20,
         async_capacity: int = 3,
         timeout: int | None = 20,
         error_mode: ErrorMode | str = ErrorMode.RAISE,
         cache_dir: str | None = None,
         progress_bar: ProgressBarMode | str = ProgressBarMode.AUTO,
     ):
-        self.completion_model = model
+        self.model = model
         self.async_capacity = async_capacity
         self.max_requests_per_minute = max_requests_per_minute
         self.error_mode = ErrorMode(error_mode)
         self.progress_bar_mode = ProgressBarMode(progress_bar)
         self._task_created_time_list: list[int] = []
         self.cache = diskcache.Cache(cache_dir) if cache_dir is not None else None
 
-        if timeout is None:
-            default_kwargs = {}
-        else:
-            default_kwargs = {'request_timeout': timeout}
-        self.default_kwargs = default_kwargs
+        if timeout is not None:
+            self.model.timeout = timeout
 
     def run(self, prompts: Sequence[str | Messages], **kwargs) -> list[str]:
-        kwargs = {**self.default_kwargs, **kwargs}
         progress_bar = self._get_progress_bar(num_tasks=len(prompts))
         completions: list[str] = []
         for prompt in prompts:
             completion = self._run_single_task(prompt=prompt, progress_bar=progress_bar, **kwargs)
             completions.append(completion)
         progress_bar.close()
         return completions
 
     @asyncer.runnify
     async def async_run(self, prompts: Sequence[str | Messages], **kwargs) -> list[str]:
-        kwargs = {**self.default_kwargs, **kwargs}
         limiter = anyio.CapacityLimiter(self.async_capacity)
         task_created_lock = anyio.Lock()
         progress_bar = self._get_progress_bar(num_tasks=len(prompts))
 
         soon_values: list[asyncer.SoonValue[str]] = []
         async with asyncer.create_task_group() as task_group:
             soon_func = task_group.soonify(self._async_run_single_task)
@@ -104,15 +99,15 @@
             async with task_created_lock:
                 sleep_time = self._calculate_sleep_time()
                 if sleep_time > 0:
                     await anyio.sleep(sleep_time)
                 self._task_created_time_list.append(int(time.time()))
 
             try:
-                completion = await self.completion_model.async_chat(prompt=prompt, **kwargs)
+                completion = await self.model.async_chat(prompt=prompt, **kwargs)
                 if self.cache is not None:
                     self.cache[task_key] = completion
             except BaseException as e:
                 if self.error_mode is ErrorMode.RAISE:
                     raise
                 elif self.error_mode is ErrorMode.IGNORE:
                     completion: str = f'Error: {e}'
@@ -131,15 +126,15 @@
 
         sleep_time = self._calculate_sleep_time()
         if sleep_time > 0:
             time.sleep(sleep_time)
         self._task_created_time_list.append(int(time.time()))
 
         try:
-            completion = self.completion_model.chat(prompt=prompt, **kwargs)
+            completion = self.model.chat(prompt=prompt, **kwargs)
             if self.cache is not None:
                 self.cache[task_key] = completion
         except BaseException as e:
             if self.error_mode is ErrorMode.RAISE:
                 raise
             elif self.error_mode is ErrorMode.IGNORE:
                 completion: str = f'Error: {e}'
@@ -163,23 +158,21 @@
         else:
             return max(self.NUM_SECONDS_PER_MINUTE - int(current_time - self._task_created_time_list[0]) + 1, 0)
 
     def _gen_task_key(self, prompt: str | Messages, **kwargs) -> str:
         if not isinstance(prompt, str):
             prompt = '---'.join([f'{message["role"]}={message["content"]}' for message in prompt])
         items = sorted([f'{key}={value}' for key, value in kwargs.items()])
-        items = [prompt, self.completion_model.identifier] + items
+        items = [prompt, self.model.identifier] + items
         task_string = '---'.join(items)
         return self.md5_hash(task_string)
 
     @staticmethod
     def md5_hash(string: str):
         return hashlib.md5(string.encode()).hexdigest()
 
     def _get_progress_bar(self, num_tasks: int) -> tqdm.tqdm:
         use_progress_bar = (self.progress_bar_mode is ProgressBarMode.ALWAYS) or (
             self.progress_bar_mode is ProgressBarMode.AUTO and num_tasks > self.PROGRESS_BAR_THRESHOLD
         )
-        progress_bar = tqdm.tqdm(
-            desc=f'{self.completion_model.__class__.__name__}', total=num_tasks, disable=not use_progress_bar
-        )
+        progress_bar = tqdm.tqdm(desc=f'{self.model.__class__.__name__}', total=num_tasks, disable=not use_progress_bar)
         return progress_bar
```

### Comparing `lmclient_core-0.3.1/lmclient/models/minimax.py` & `lmclient_core-0.3.1.post1/lmclient/models/minimax.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,40 +16,71 @@
         group_id: str | None = None,
         api_key: str | None = None,
     ):
         self.model_name = model_name
 
         self.group_id = group_id or os.environ['MINIMAX_GROUP_ID']
         self.api_key = api_key or os.environ['MINIMAX_API_KEY']
+        self.timeout = None
 
     def chat(self, prompt: Messages | str, **kwargs) -> str:
         if isinstance(prompt, str):
             prompt = [Message(role='user', content=prompt)]
 
         headers = {
             'Authorization': f'Bearer {self.api_key}',
             'Content-Type': 'application/json',
         }
         json_data = self._messages_to_request_json_data(prompt)
+        if 'temperature' in kwargs:
+            kwargs['temperature'] = max(0.01, kwargs['temperature'])
         json_data.update(kwargs)
         response = requests.post(
             f'https://api.minimax.chat/v1/text/chatcompletion?GroupId={self.group_id}',
             json=json_data,
             headers=headers,
+            timeout=self.timeout,
         ).json()
-        completion: str = response['choices'][0]['text']  # type: ignore
+        try:
+            completion: str = response['choices'][0]['text']  # type: ignore
+        except (KeyError, IndexError):
+            raise ValueError(f'Invalid response: {response}')
+        return completion
+
+    async def async_chat(self, prompt: Messages | str, **kwargs) -> str:
+        if isinstance(prompt, str):
+            prompt = [Message(role='user', content=prompt)]
+
+        async with httpx.AsyncClient() as client:
+            headers = {
+                'Authorization': f'Bearer {self.api_key}',
+                'Content-Type': 'application/json',
+            }
+            json_data = self._messages_to_request_json_data(prompt)
+            if 'temperature' in kwargs:
+                kwargs['temperature'] = max(0.01, kwargs['temperature'])
+            json_data.update(kwargs)
+            response = await client.post(
+                f'https://api.minimax.chat/v1/text/chatcompletion?GroupId={self.group_id}',
+                json=json_data,
+                headers=headers,
+                timeout=self.timeout,
+            )
+            response = response.json()
+
+        try:
+            completion: str = response['choices'][0]['text']  # type: ignore
+        except (KeyError, IndexError):
+            raise ValueError(f'Invalid response: {response}')
         return completion
 
     def _messages_to_request_json_data(self, messages: Messages):
         data: dict[str, Any] = {
             'model': self.model_name,
-            "role_meta": {
-                "user_name": "用户",
-                "bot_name": "MM智能助理"
-            },
+            'role_meta': {'user_name': '用户', 'bot_name': 'MM智能助理'},
         }
 
         if messages[0]['role'] == 'system':
             data['prompt'] = messages[0]['content']
             messages = messages[1:]
         else:
             data['prompt'] = '你是MM智能助理'
@@ -67,31 +98,10 @@
                     'sender_type': role,
                     'text': message['content'],
                 }
             )
         data['messages'] = minimax_messages
         return data
 
-    async def async_chat(self, prompt: Messages | str, **kwargs) -> str:
-        if isinstance(prompt, str):
-            prompt = [Message(role='user', content=prompt)]
-
-        async with httpx.AsyncClient() as client:
-            headers = {
-                'Authorization': f'Bearer {self.api_key}',
-                'Content-Type': 'application/json',
-            }
-            json_data = self._messages_to_request_json_data(prompt)
-            json_data.update(kwargs)
-            response = await client.post(
-                f'https://api.minimax.chat/v1/text/chatcompletion?GroupId={self.group_id}',
-                json=json_data,
-                headers=headers,
-            )
-            response = response.json()
-
-        completion: str = response['choices'][0]['text']  # type: ignore
-        return completion
-
     @property
     def identifier(self) -> str:
         return f'{self.__class__.__name__}({self.model_name})'
```

### Comparing `lmclient_core-0.3.1/lmclient/types.py` & `lmclient_core-0.3.1.post1/lmclient/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 Messages = Sequence[Message]
 
 
 @runtime_checkable
 class ChatModel(Protocol):
+    timeout: float | None
     identifier: str
 
     def chat(self, prompt: Messages | str, **kwargs) -> str:
         ...
 
     async def async_chat(self, prompt: Messages | str, **kwargs) -> str:
         ...
```

### Comparing `lmclient_core-0.3.1/pyproject.toml` & `lmclient_core-0.3.1.post1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lmclient-core"
-version = "0.3.1"
+version = "0.3.1.post1"
 description = "LM Async Client, openai client, azure openai client ..."
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "lmclient"}]
 repository = "https://github.com/wangyuxinwhy/lmclient"
 keywords = ["lmclient", "openai", "azure", "async"]
```

### Comparing `lmclient_core-0.3.1/PKG-INFO` & `lmclient_core-0.3.1.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmclient-core
-Version: 0.3.1
+Version: 0.3.1.post1
 Summary: LM Async Client, openai client, azure openai client ...
 Home-page: https://github.com/wangyuxinwhy/lmclient
 License: Apache-2.0
 Keywords: lmclient,openai,azure,async
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.8,<4.0
```

