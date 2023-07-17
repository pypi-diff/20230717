# Comparing `tmp/threads-api-1.1.8.tar.gz` & `tmp/threads-api-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.1.8.tar", last modified: Fri Jul 14 16:34:23 2023, max compression
+gzip compressed data, was "threads-api-1.1.9.tar", last modified: Sat Jul 15 21:58:40 2023, max compression
```

## Comparing `threads-api-1.1.8.tar` & `threads-api-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:34:23.902443 threads-api-1.1.8/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.8/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    15158 2023-07-14 16:34:23.902443 threads-api-1.1.8/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    14543 2023-07-14 16:25:20.000000 threads-api-1.1.8/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      472 2023-07-14 16:29:40.000000 threads-api-1.1.8/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-14 16:34:23.902443 threads-api-1.1.8/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      853 2023-07-14 16:29:34.000000 threads-api-1.1.8/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:34:23.894443 threads-api-1.1.8/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.8/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:34:23.898443 threads-api-1.1.8/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.8/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    43640 2023-07-14 16:28:49.000000 threads-api-1.1.8/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:34:23.898443 threads-api-1.1.8/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.8/threads_api/tests/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      305 2023-07-13 17:43:17.000000 threads-api-1.1.8/threads_api/tests/get_post_id_test.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      592 2023-07-13 21:53:08.000000 threads-api-1.1.8/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:34:23.898443 threads-api-1.1.8/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    15158 2023-07-14 16:34:23.000000 threads-api-1.1.8/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      404 2023-07-14 16:34:23.000000 threads-api-1.1.8/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-14 16:34:23.000000 threads-api-1.1.8/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-14 16:34:23.000000 threads-api-1.1.8/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-14 16:34:23.000000 threads-api-1.1.8/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-15 21:58:40.475124 threads-api-1.1.9/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.9/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15158 2023-07-15 21:58:40.475124 threads-api-1.1.9/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    14543 2023-07-14 16:36:44.000000 threads-api-1.1.9/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      472 2023-07-15 21:58:06.000000 threads-api-1.1.9/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-15 21:58:40.475124 threads-api-1.1.9/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      853 2023-07-15 21:57:59.000000 threads-api-1.1.9/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-15 21:58:40.467125 threads-api-1.1.9/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.9/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-15 21:58:40.471125 threads-api-1.1.9/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.9/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      946 2023-07-15 17:43:17.000000 threads-api-1.1.9/threads_api/src/anotherlogger.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3072 2023-07-15 21:56:50.000000 threads-api-1.1.9/threads_api/src/settings.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    42618 2023-07-15 21:57:15.000000 threads-api-1.1.9/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-15 21:58:40.471125 threads-api-1.1.9/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.9/threads_api/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      305 2023-07-13 17:43:17.000000 threads-api-1.1.9/threads_api/tests/get_post_id_test.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      592 2023-07-13 21:53:08.000000 threads-api-1.1.9/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-15 21:58:40.471125 threads-api-1.1.9/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15158 2023-07-15 21:58:40.000000 threads-api-1.1.9/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      465 2023-07-15 21:58:40.000000 threads-api-1.1.9/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-15 21:58:40.000000 threads-api-1.1.9/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-15 21:58:40.000000 threads-api-1.1.9/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-15 21:58:40.000000 threads-api-1.1.9/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.1.8/LICENSE` & `threads-api-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.8/PKG-INFO` & `threads-api-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.8
+Version: 1.1.9
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Daniel Saad
 Author-email: danielsaad777@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `threads-api-1.1.8/README.md` & `threads-api-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.8/setup.py` & `threads-api-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.1.8',
+    version='1.1.9',
     description='Unofficial Python client for Meta Threads.net API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Daniel Saad',
     author_email='danielsaad777@gmail.com',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
```

### Comparing `threads-api-1.1.8/threads_api/src/threads_api.py` & `threads-api-1.1.9/threads_api/src/threads_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,18 @@
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 
 from instagrapi import Client
 
 import logging
 import sys
-
+from threads_api.src.anotherlogger import log
 from colorama import init, Fore, Style
+import functools
+from threads_api.src.settings import Settings
 
 BASE_URL = "https://i.instagram.com/api/v1"
 LOGIN_URL = BASE_URL + "/bloks/apps/com.bloks.www.bloks.caa.login.async.send_login_request/"
 POST_URL_TEXTONLY = BASE_URL + "/media/configure_text_only_post/"
 POST_URL_IMAGE = BASE_URL + "/media/configure_text_post_app_feed/"
 DEFAULT_HEADERS = {
             'Authority': 'www.threads.net',
@@ -53,16 +55,14 @@
                 'AppleWebKit/605.1.15 (KHTML, like Gecko) Version/11.1.2 Safari/605.1.15'
             ),
             'X-ASBD-ID': '129477',
             'X-FB-LSD': 'NjppQDEgONsU_1LCzrmp6q',
             'X-IG-App-ID': '238260118697367',
         }
 
-# This will help debugging flow failures
-
 class SimpleEncDec:
     backend = default_backend()
     iterations = 100_000
 
     @staticmethod
     def _derive_key(password: bytes, salt: bytes, iterations: int = iterations) -> bytes:
         """Derive a secret key from a given password and salt"""
@@ -92,14 +92,22 @@
         return Fernet(key).decrypt(token)
 
 class LoggedOutException(Exception):
      def __init__(self, message):            
         # Call the base class constructor with the parameters it needs
         super().__init__(message)
 
+def require_login(func):
+    @functools.wraps(func)
+    async def wrapper(self, *args, **kwargs):
+        if not self.is_logged_in:
+            raise Exception(f"The action '{func.__name__}' can only be perfomed while logged-in")
+        return await func(self, *args, **kwargs)
+    return wrapper
+
 class ThreadsAPI:
     def __init__(self):
         
         # Get the log level from the environment variable
         log_level_env = os.environ.get("LOG_LEVEL", "WARNING")
 
         # Set the log level based on the environment variable
@@ -109,51 +117,83 @@
         
         self.log_level = log_level
         
         self.set_log_level(self.log_level)
 
         self.logger = logging.getLogger()
         
-
+        self._auth_session = None
+        self._settings = Settings()
         self.token = None
         self.user_id = None
         self.is_logged_in = False
         self.auth_headers = None
 
         self.FBLSDToken = 'NjppQDEgONsU_1LCzrmp6q'
 
-        self.instagrapi_client = Client()
-        
+        self.instagrapi_client = None
+
     def set_log_level(self, log_level):
         self.log_level = log_level
         logging.basicConfig(level=self.log_level, format='%(levelname)s:%(message)s')
 
     def log_request(self, type, url, header, payload=""):
         self.logger.debug(f'{Fore.GREEN}-\nRequest [{Style.RESET_ALL}{type}{Fore.GREEN}] -> URL: [{Style.RESET_ALL}{url}{Fore.GREEN}]\nHeader: [{Style.RESET_ALL}{header}{Fore.GREEN}]\nRequest Payload: [{Style.RESET_ALL}{payload}{Fore.GREEN}]\n-{Style.RESET_ALL}')
 
     def log_response(self, url, resp):
         self.logger.debug(f'{Fore.GREEN}-\nResponse -> URL: [{Style.RESET_ALL}{url}{Fore.GREEN}]\nResponse Payload: [{Style.RESET_ALL}{resp}{Fore.GREEN}]\n-{Style.RESET_ALL}')
         return resp
 
+    @require_login
+    async def _private_post(self, **kwargs):
+        log(title='PRIVATE REQUEST', type='POST', **kwargs)
+        async with self._auth_session.post(**kwargs) as response:
+            try:
+                text = await response.text()
+                resp = json.loads(text)
+                log(title='PRIVATE RESPONSE', response=resp)
+
+                if resp['status'] == 'fail':
+                    raise Exception(f"Request Failed: [{resp['message']}]")
+            except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                raise Exception('Failed to decode response as JSON')
+            
+            return resp
+
+    @require_login
+    async def _private_get(self, **kwargs):
+        log(title='PRIVATE REQUEST', type='GET', **kwargs)
+        async with self._auth_session.get(**kwargs) as response:
+            try:
+                text = await response.text()
+                resp = json.loads(text)
+                log(title='PRIVATE RESPONSE', response=resp)
+
+                if resp['status'] == 'fail':
+                    raise Exception(f"Request Failed: [{resp['message']}]")
+            except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                raise Exception('Failed to decode response as JSON')
+            
+            return resp
 
     async def _get_public_headers(self) -> str:
         default_headers = copy.deepcopy(DEFAULT_HEADERS)
         default_headers['X-FB-LSD'] = await self._refresh_public_token()
         return default_headers
     
     async def _refresh_public_token(self) -> str:
         self.logger.info("Refreshing public token")
         modified_default_headers = copy.deepcopy(DEFAULT_HEADERS)
         del modified_default_headers['X-FB-LSD']
         url = 'https://www.instagram.com/instagram'
         async with aiohttp.ClientSession() as session:
-            self.log_request('GET', url, modified_default_headers)
+            #self.log_request('GET', url, modified_default_headers)
             async with session.get(url, headers=modified_default_headers) as response:
                 data = await response.text()
-                self.log_response(url, data)
+                #self.log_response(url, data)
                 token_key_value = re.search('LSD",\\[\\],{"token":"(.*?)"},\\d+\\]', data).group()
                 token_key_value = token_key_value.replace('LSD",[],{"token":"', '')
                 token = token_key_value.split('"')[0]
 
         self.FBLSDToken = token
         return self.FBLSDToken
     
@@ -169,36 +209,45 @@
             bool: True if the login is successful, False otherwise.
 
         Raises:
             Exception: If the username or password are invalid, or if an error occurs during login.
         """
         def _save_token_to_cache(cached_token_path, token, password):
             with open(cached_token_path, "wb") as fd:
-                fd.write(SimpleEncDec.password_encrypt(token.encode(), password))
+                encrypted_token = SimpleEncDec.password_encrypt(token.encode(), password)
+                fd.write(encrypted_token)
+
+                # Sync token between original token cache and the settings file
+                self._settings.set_encrypted_token(encrypted_token)
                 self.logger.info("Saved token to cache")
             return
 
         def _get_token_from_cache(cached_token_path, password):
             with open(cached_token_path, "rb") as fd:
                 encrypted_token = fd.read()
-                self.logger.info("Loaded token from cache")
+                
+                # Sync token between original token cache and the settings file
+                self._settings.set_encrypted_token(encrypted_token)
 
-            return SimpleEncDec.password_decrypt(encrypted_token, password).decode()
+                decrypted_token = SimpleEncDec.password_decrypt(encrypted_token, password).decode()
+                self.logger.info("Loaded token from cache")
+            return decrypted_token
         
         async def _set_logged_in_state(username, token):
             self.token = token
             self.auth_headers = {
                 'Authorization': f'Bearer IGT:2:{self.token}',
                 'User-Agent': 'Barcelona 289.0.0.77.109 Android',
                 'Sec-Fetch-Site': 'same-origin',
                 'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
             }
             self.is_logged_in = True
             self.user_id = await self.get_user_id_from_username(username)
             self.logger.info("Set logged-in state successfully. All set!")
+            self._auth_session = aiohttp.ClientSession()
             return
         
         if username is None or password is None:
             raise Exception("Username or password are invalid")
 
         self.username = username
 
@@ -212,27 +261,39 @@
             except LoggedOutException as e:
                 print(f"[Error] {e}. Attempting to re-login.")
                 pass
 
         try:
             
             self.logger.info("Attempting to login")
+            if self.instagrapi_client is None:
+                self.instagrapi_client = Client()
             self.instagrapi_client.login(username, password)
             token = self.instagrapi_client.private.headers['Authorization'].split("Bearer IGT:2:")[1]
             
             await _set_logged_in_state(username, token)
                     
             if cached_token_path is not None:
                 _save_token_to_cache(cached_token_path, token, password)
         except Exception as e:
             print("[ERROR] ", e)
             raise
 
         return True
 
+    async def close_gracefully(self):
+        if self._auth_session is not None:
+            await self._auth_session.close()
+            self._auth_session = None
+        if self.instagrapi_client is not None:
+            self.instagrapi_client = None
+        self.user_id = None
+        self.is_logged_in = False
+        self.token = None
+
     async def __auth_required_post_request(self, url: str):
         async with aiohttp.ClientSession() as session:
             self.log_request('POST', url, self.auth_headers)
             async with session.post(url, headers=self.auth_headers) as response:
                 resp = await response.json()
                 self.log_response(url, resp)
 
@@ -285,18 +346,18 @@
         else:
             self.logger.info(f"Fetching user_id for user [{username}] anonymously")
             url = f"https://www.threads.net/@{username}"
             
             headers = await self._get_public_headers()
 
             async with aiohttp.ClientSession() as session:
-                self.log_request('GET', url, headers)
+                #self.log_request('GET', url, headers)
                 async with session.get(url, headers=headers) as response:
                     text = await response.text()
-                    self.log_response(url, text)
+                    #self.log_response(url, text)
 
             text = text.replace('\\s', "").replace('\\n', "")
             user_id = re.search(r'"props":{"user_id":"(\d+)"},', text)
 
             return user_id.group(1) if user_id else None
 
     async def get_user_profile(self, user_id: str):
@@ -341,111 +402,131 @@
                 text = await response.text()
                 data = json.loads(text)
                 self.log_response(url, data)
                
         user = data['data']['userData']['user']
         return user
 
-    async def get_user_threads(self, user_id: str):
+    async def get_user_threads(self, user_id: str, count=10, max_id=None):
         """
         Retrieves the threads associated with a user with the provided user ID.
 
         Args:
             user_id (str): The user ID for which to retrieve the threads.
 
         Returns:
             list: A list of dictionaries representing the threads associated with the user.
 
         Raises:
             Exception: If an error occurs during the thread retrieval process.
         """
-        url = 'https://www.threads.net/api/graphql'
-        
-        modified_headers = copy.deepcopy(await self._get_public_headers())
+        if self.is_logged_in:
+            if max_id is not None:
+                params = {'count': count, 'max_id':max_id}
+            else:
+                params = {'count': count}
+            resp = await self._private_get(url=f'{BASE_URL}/text_feed/{user_id}/profile/', headers=self.auth_headers,data=params)
 
-        modified_headers.update({
-            'sec-fetch-dest': 'empty',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-site': 'same-origin',
-            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
-            'x-fb-friendly-name': 'BarcelonaProfileThreadsTabQuery',
-            'x-fb-lsd': self.FBLSDToken,
-        })
-        
-        payload = {
-                'lsd': self.FBLSDToken,
-                'variables': json.dumps(
-                    {
-                        'userID': user_id,
-                    }
-                ),
-                'doc_id': '6232751443445612'
-            }
-        
-        async with aiohttp.ClientSession() as session:
-            self.log_request('POST', url, modified_headers, payload)
-            async with session.post(url, headers=modified_headers, data=payload) as response:
-                try:
-                    text = await response.text()
-                    data = json.loads(text)
-                    self.log_response(url, data)
-                except (aiohttp.ContentTypeError, json.JSONDecodeError):
-                    raise Exception('Failed to decode response as JSON')
+            return resp
+        # Public API for getting user threads is minimal. 'count' and 'max_id' are not used.
+        else:
+            url = 'https://www.threads.net/api/graphql'
+            
+            modified_headers = copy.deepcopy(await self._get_public_headers())
 
-        threads = data['data']['mediaData']['threads']
-        return threads
+            modified_headers.update({
+                'sec-fetch-dest': 'empty',
+                'sec-fetch-mode': 'cors',
+                'sec-fetch-site': 'same-origin',
+                'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
+                'x-fb-friendly-name': 'BarcelonaProfileThreadsTabQuery',
+                'x-fb-lsd': self.FBLSDToken,
+            })
+            
+            payload = {
+                    'lsd': self.FBLSDToken,
+                    'variables': json.dumps(
+                        {
+                            'userID': user_id,
+                        }
+                    ),
+                    'doc_id': '6232751443445612'
+                }
+            
+            async with aiohttp.ClientSession() as session:
+                self.log_request('POST', url, modified_headers, payload)
+                async with session.post(url, headers=modified_headers, data=payload) as response:
+                    try:
+                        text = await response.text()
+                        data = json.loads(text)
+                        self.log_response(url, data)
+                    except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                        raise Exception('Failed to decode response as JSON')
+
+            threads = data['data']['mediaData']['threads']
+            return threads
     
-    async def get_user_replies(self, user_id: str):
+    async def get_user_replies(self, user_id: str, count=10, max_id=None):
         """
         Retrieves the replies associated with a user with the provided user ID.
 
         Args:
             user_id (str): The user ID for which to retrieve the replies.
 
         Returns:
             list: A list of dictionaries representing the replies associated with the user.
 
         Raises:
             Exception: If an error occurs during the thread retrieval process.
         """
-        url = 'https://www.threads.net/api/graphql'
+        if self.is_logged_in:
+            if max_id is not None:
+                params = {'count': count, 'max_id':max_id}
+            else:
+                params = {'count': count}
+            resp = await self._private_get(url=f'{BASE_URL}/text_feed/{user_id}/profile/replies', headers=self.auth_headers,data=params)
 
-        modified_headers = copy.deepcopy(await self._get_public_headers())
+            return resp
+        # Public API for getting user threads is minimal. 'count' and 'max_id' are not used.
+        else:
+            url = 'https://www.threads.net/api/graphql'
 
-        modified_headers.update({
-            'sec-fetch-dest': 'empty',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-site': 'same-origin',
-            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
-            'x-fb-friendly-name': 'BarcelonaProfileRepliesTabQuery',
-            'x-fb-lsd': self.FBLSDToken,
-        })
-        
-        payload = {
-                'lsd': self.FBLSDToken,
-                'variables': json.dumps(
-                    {
-                        'userID': user_id,
-                    }
-                ),
-                'doc_id': '6307072669391286'
-            }
+            modified_headers = copy.deepcopy(await self._get_public_headers())
 
-        async with aiohttp.ClientSession() as session:
-            self.log_request('POST', url, modified_headers, payload)
-            async with session.post(url, headers=modified_headers, data=payload) as response:
-                try:
-                    text = await response.text()
-                    data = json.loads(text)
-                    self.log_response(url, data)
-                except (aiohttp.ContentTypeError, json.JSONDecodeError):
-                    raise Exception('Failed to decode response as JSON')
+            modified_headers.update({
+                'sec-fetch-dest': 'empty',
+                'sec-fetch-mode': 'cors',
+                'sec-fetch-site': 'same-origin',
+                'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
+                'x-fb-friendly-name': 'BarcelonaProfileRepliesTabQuery',
+                'x-fb-lsd': self.FBLSDToken,
+            })
+            
+            payload = {
+                    'lsd': self.FBLSDToken,
+                    'variables': json.dumps(
+                        {
+                            'userID': user_id,
+                        }
+                    ),
+                    'doc_id': '6307072669391286'
+                }
 
-        threads = data['data']['mediaData']['threads']
-        return threads
+            async with aiohttp.ClientSession() as session:
+                self.log_request('POST', url, modified_headers, payload)
+                async with session.post(url, headers=modified_headers, data=payload) as response:
+                    try:
+                        text = await response.text()
+                        data = json.loads(text)
+                        self.log_response(url, data)
+                    except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                        raise Exception('Failed to decode response as JSON')
+
+            threads = data['data']['mediaData']['threads']
+            return threads
 
     async def get_user_followers(self, user_id: str) -> bool:
         if not self.is_logged_in:
             raise Exception("The action 'get_user_followers' can only be perfomed while logged-in")
         
         res = await self.__auth_required_get_request(f"{BASE_URL}/friendships/{user_id}/followers")
         return res
@@ -453,107 +534,97 @@
     async def get_user_following(self, user_id: str) -> bool:
         if not self.is_logged_in:
             raise Exception("The action 'get_user_following' can only be perfomed while logged-in")
         
         res = await self.__auth_required_get_request(f"{BASE_URL}/friendships/{user_id}/following")
         return res
 
+    @require_login
     async def follow_user(self, user_id: str) -> bool:
         """
         Follows a user with the given user ID.
 
         Args:
             user_id (str): The ID of the user to follow.
 
         Returns:
             bool: True if the user was followed successfully, False otherwise.
 
         Raises:
             Exception: If an error occurs during the follow process.
-        """
-        if not self.is_logged_in:
-            raise Exception("The action 'follow_user' can only be perfomed while logged-in")
-        
-        res = await self.__auth_required_post_request(f"{BASE_URL}/friendships/create/{user_id}/")
+        """        
+        res = await self._private_post(url=f"{BASE_URL}/friendships/create/{user_id}/", headers=self.auth_headers)
         return res["status"] == "ok"
 
+    @require_login
     async def unfollow_user(self, user_id: str) -> bool:
         """
         Unfollows a user with the given user ID.
 
         Args:
             user_id (str): The ID of the user to unfollow.
 
         Returns:
             bool: True if the user was unfollowed successfully, False otherwise.
 
         Raises:
             Exception: If an error occurs during the unfollow process.
-        """
-        if not self.is_logged_in:
-            raise Exception("The action 'unfollow_user' can only be perfomed while logged-in")
-        
-        res = await self.__auth_required_post_request(f"{BASE_URL}/friendships/destroy/{user_id}/")
+        """        
+        res = await self._private_post(url=f"{BASE_URL}/friendships/destroy/{user_id}/", headers=self.auth_headers)
         return res["status"] == "ok"
 
+    @require_login
     async def like_post(self, post_id: str) -> bool:
         """
         Likes a post with the given ID.
 
         Args:
             user_id (str): The ID of the post to like.
 
         Returns:
             bool: True if the post was liked successfully, False otherwise.
 
         Raises:
             Exception: If an error occurs during the like process.
-        """
-        if not self.is_logged_in:
-            raise Exception("The action 'like_post' can only be perfomed while logged-in")
-        
-        res = await self.__auth_required_post_request(f"{BASE_URL}/media/{post_id}_{self.user_id}/like/")
+        """        
+        res = await self._private_post(url=f"{BASE_URL}/media/{post_id}_{self.user_id}/like/", headers=self.auth_headers)
         return res["status"] == "ok"
     
+    @require_login
     async def unlike_post(self, post_id: str) -> bool:
         """
         Unlikes a post with the given ID.
 
         Args:
             user_id (str): The ID of the post to unlike.
 
         Returns:
             bool: True if the post was unliked successfully, False otherwise.
 
         Raises:
             Exception: If an error occurs during the like process.
         """
-        if not self.is_logged_in:
-            raise Exception("The action 'unlike_post' can only be perfomed while logged-in")
-        
-        res = await self.__auth_required_post_request(f"{BASE_URL}/media/{post_id}_{self.user_id}/unlike/")
+        res = await self._private_post(url=f"{BASE_URL}/media/{post_id}_{self.user_id}/unlike/", headers=self.auth_headers)
         return res["status"] == "ok"
     
+    @require_login
     async def delete_post(self, post_id: str) -> bool:
         """
         Deletes a post with the given ID.
 
         Args:
             user_id (str): The ID of the post to delete.
 
         Returns:
             bool: True if the post was deleted successfully, False otherwise.
 
         Raises:
             Exception: If an error occurs during the deletion process.
         """
-        if not self.is_logged_in:
-            raise Exception("The action 'delete_post' can only be perfomed while logged-in")
-        
-        res = await self.__auth_required_post_request(f"{BASE_URL}/media/{post_id}_{self.user_id}/delete/?media_type=TEXT_POST")
+        res = await self._private_post(url=f"{BASE_URL}/media/{post_id}_{self.user_id}/delete/?media_type=TEXT_POST", headers=self.auth_headers)
         return res["status"] == "ok"
     
     async def get_post_id_from_url(self, post_url):
         """
         Retrieves the post ID from a given URL.
 
         Args:
@@ -669,58 +740,43 @@
                     data = json.loads(text)
                     self.log_response(url, data)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         return data['data']['likers']['users']
 
+    @require_login
     async def get_timeline(self, maxID=None):
         """
         Get timeline for the authenticated user
 
         Args:
             maxID (int): The ID token for the next batch of posts
 
         Returns:
             list: REST API JSON data response for the get_timeline request
 
         Raises:
             Exception: If an error occurs during the timeline retrieval process.
         """
-        if not self.is_logged_in:
-            raise Exception("The action 'get_timeline' can only be perfomed while logged-in")
-
         # Check if you have the ID of the next batch to fetch
         if maxID is None:
             parameters = {
                     'pagination_source': 'text_post_feed_threads',
             }
         else:
             parameters = {
                     'pagination_source': 'text_post_feed_threads',
-                    'maxID': maxID
+                    'max_id': maxID
             }
 
-        encoded_parameters = urllib.parse.urlencode(parameters)
-
-        url = f'{BASE_URL}/feed/text_post_app_timeline/?{encoded_parameters}'
-        async with aiohttp.ClientSession() as session:
-            self.log_request('POST', url, self.auth_headers)
-            async with session.post(url, 
-                                    headers=self.auth_headers) as response:
-                try:
-                    text = await response.text()
-                    data = json.loads(text)
-                    self.log_response(url, data)
-                except (aiohttp.ContentTypeError, json.JSONDecodeError):
-                    raise Exception('Failed to decode response as JSON')
-        
-        return data
-
+        res = await self._private_post(url=f'{BASE_URL}/feed/text_post_app_timeline/', headers=self.auth_headers,data=parameters)
+        return res
 
+    @require_login
     async def mute_user(self, user_id):
         """
         Mute a user
 
         Args:
             user_id (int): The ID of the user to mute.
 
@@ -736,29 +792,18 @@
                 'container_module': 'ig_text_feed_timeline',
             },
         )
 
         encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
         payload = f'signed_body=SIGNATURE.{encoded_parameters}'
 
-        url = f'{BASE_URL}/friendships/mute_posts_or_story_from_follow/'
-        async with aiohttp.ClientSession() as session:
-            self.log_request('POST', url, self.auth_headers, payload)
-            async with session.post(url, 
-                                    headers=self.auth_headers, 
-                                    data=payload) as response:
-                try:
-                    text = await response.text()
-                    data = json.loads(text)
-                    self.log_response(url, data)
-                except (aiohttp.ContentTypeError, json.JSONDecodeError):
-                    raise Exception('Failed to decode response as JSON')
-        
-        return data
+        res = await self._private_post(url=f'{BASE_URL}/friendships/mute_posts_or_story_from_follow/', headers=self.auth_headers, data=payload)
+        return res
 
+    @require_login
     async def unmute_user(self, user_id):
         """
         Unmute a user
 
         Args:
             user_id (int): The ID of the user to unmute.
 
@@ -774,30 +819,18 @@
                 'container_module': 'ig_text_feed_timeline',
             },
         )
 
         encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
         payload = f'signed_body=SIGNATURE.{encoded_parameters}'
 
-        url = f'{BASE_URL}/friendships/unmute_posts_or_story_from_follow/'
-
-        async with aiohttp.ClientSession() as session:
-            self.log_request('POST', url, self.auth_headers, payload)
-            async with session.post(url, 
-                                    headers=self.auth_headers, 
-                                    data=payload) as response:
-                try:
-                    text = await response.text()
-                    data = json.loads(text)
-                    self.log_response(url, data)
-                except (aiohttp.ContentTypeError, json.JSONDecodeError):
-                    raise Exception('Failed to decode response as JSON')
-        
-        return data
+        res = await self._private_post(url=f'{BASE_URL}/friendships/unmute_posts_or_story_from_follow/', headers=self.auth_headers, data=payload)
+        return res
     
+    @require_login
     async def restrict_user(self, user_id):
         """
         Restrict a user
 
         Args:
             user_id (int): The ID of the user to restrict.
 
@@ -813,29 +846,18 @@
                 'container_module': 'ig_text_feed_timeline',
             },
         )
 
         encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
         payload = f'signed_body=SIGNATURE.{encoded_parameters}'
 
-        url = f'{BASE_URL}/restrict_action/restrict_many/'
-        async with aiohttp.ClientSession() as session:
-            self.log_request('POST', url, self.auth_headers, payload)
-            async with session.post(url, 
-                                    headers=self.auth_headers, 
-                                    data=payload) as response:
-                try:
-                    text = await response.text()
-                    data = json.loads(text)
-                    self.log_response(url, data)
-                except (aiohttp.ContentTypeError, json.JSONDecodeError):
-                    raise Exception('Failed to decode response as JSON')
-        
-        return data
+        res = await self._private_post(url=f'{BASE_URL}/restrict_action/restrict_many/', headers=self.auth_headers, data=payload)
+        return res
     
+    @require_login
     async def unrestrict_user(self, user_id):
         """
         Unrestrict a user
 
         Args:
             user_id (int): The ID of the user to unrestrict.
 
@@ -850,30 +872,18 @@
                 'user_ids': user_id,
                 'container_module': 'ig_text_feed_timeline',
             },
         )
 
         encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
         payload = f'signed_body=SIGNATURE.{encoded_parameters}'
-        url = f'{BASE_URL}/restrict_action/unrestrict/'
-        
-        async with aiohttp.ClientSession() as session:
-            self.log_request('POST', url, self.auth_headers, payload)
-            async with session.post(url, 
-                                    headers=self.auth_headers, 
-                                    data=payload) as response:
-                try:
-                    text = await response.text()
-                    data = json.loads(text)
-                    self.log_response(url, data)
-                except (aiohttp.ContentTypeError, json.JSONDecodeError):
-                    raise Exception('Failed to decode response as JSON')
-        
-        return data
+        res = await self._private_post(url=f'{BASE_URL}/restrict_action/unrestrict/', headers=self.auth_headers, data=payload)
+        return res
     
+    @require_login
     async def block_user(self, user_id):
         """
         Block a user
 
         Args:
             user_id (int): The ID of the user to block.
 
@@ -889,30 +899,18 @@
                 'surface': 'ig_text_feed_timeline',
                 'is_auto_block_enabled': 'true',
             },
         )
 
         encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
         payload = f'signed_body=SIGNATURE.{encoded_parameters}'
-        url = f'{BASE_URL}/friendships/block/{user_id}/'
-
-        async with aiohttp.ClientSession() as session:
-            self.log_request('POST', url, self.auth_headers, payload)
-            async with session.post(url, 
-                                    headers=self.auth_headers, 
-                                    data=payload) as response:
-                try:
-                    text = await response.text()
-                    data = json.loads(text)
-                    self.log_response(url, data)
-                except (aiohttp.ContentTypeError, json.JSONDecodeError):
-                    raise Exception('Failed to decode response as JSON')
-        
-        return data
+        res = await self._private_post(url=f'{BASE_URL}/friendships/block/{user_id}/', headers=self.auth_headers, data=payload)
+        return res
     
+    @require_login
     async def unblock_user(self, user_id):
         """
         Unblock a user
 
         Args:
             user_id (int): The ID of the user to unblock.
 
@@ -927,30 +925,18 @@
                 'user_id': user_id,
                 'container_module': 'ig_text_feed_timeline',
             },
         )
 
         encoded_parameters = urllib.parse.quote(string=parameters, safe="!~*'()")
         payload = f'signed_body=SIGNATURE.{encoded_parameters}'
-        url = f'{BASE_URL}/friendships/unblock/{user_id}/'
-
-        async with aiohttp.ClientSession() as session:
-            self.log_request('POST', url, self.auth_headers, payload)
-            async with session.post(url, 
-                                    headers=self.auth_headers, 
-                                    data=payload) as response:
-                try:
-                    text = await response.text()
-                    data = json.loads(text)
-                    self.log_response(url, data)
-                except (aiohttp.ContentTypeError, json.JSONDecodeError):
-                    raise Exception('Failed to decode response as JSON')
-        
-        return data
+        res = await self._private_post(url=f'{BASE_URL}/friendships/unblock/{user_id}/', headers=self.auth_headers, data=payload)
+        return res
     
+    @require_login
     async def post(
         self, caption: str, image_path: str = None, url: str = None, parent_post_id: str = None
     ) -> bool:
         """
         Creates a new post with the given caption, image, URL, and parent post ID.
 
         Args:
@@ -978,27 +964,25 @@
             url_pattern = re.compile(
                 r"^(https?://)?"
                 r"((([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9-]*[a-zA-Z0-9])\.)+[a-zA-Z]{2,})"
                 r"(/?|/[-a-zA-Z0-9_%+.~!@#$^&*(){}[\]|/\\<>]*)$"
             )
             if re.match(url_pattern, url) is not None:
                 try:
-                    async with aiohttp.ClientSession() as session:
-                        async with session.head(url) as response:
-                            return response.status == 200
+                    async with self._auth_session.head(url) as response:
+                        return response.status == 200
                 except aiohttp.ClientError:
                     return False
             return False
 
         async def __download(url: str) -> bytes:
             try:
-                async with aiohttp.ClientSession() as session:
-                    async with session.get(url) as response:
-                        response.raise_for_status()
-                        return await response.read()
+                async with self._auth_session.get(url) as response:
+                    response.raise_for_status()
+                    return await response.read()
             except aiohttp.ClientError as e:
                 raise Exception("[ERROR] failed to load file: ", e)
 
         async def __upload_image(image_url: str, image_content: bytes) -> str:
             headers = __get_app_headers().copy()
 
             upload_id = int(time.time() * 1000)
@@ -1007,22 +991,21 @@
             mime_type = None
             if image_content is None:
                 with open(image_url, mode="rb") as f:
                     content = f.read()
                 mime_type, _ = mimetypes.guess_type(image_url)
             else:
                 content = image_content
-                async with aiohttp.ClientSession() as session:
-                    async with session.head(image_url) as response:
-                        content_type = response.headers.get("Content-Type")
-                        if not content_type:
-                            file_name = url.split("/")[-1]
-                            mime_type, _ = mimetypes.guess_type(file_name)
-                        if mime_type is None:
-                            mime_type = "jpeg"
+                async with self._auth_session.head(image_url) as response:
+                    content_type = response.headers.get("Content-Type")
+                    if not content_type:
+                        file_name = url.split("/")[-1]
+                        mime_type, _ = mimetypes.guess_type(file_name)
+                    if mime_type is None:
+                        mime_type = "jpeg"
 
             x_instagram_rupload_params = {
                 "upload_id": f"{upload_id}",
                 "media_type": "1",
                 "sticker_burnin_params": "[]",
                 "image_compression": json.dumps(
                     {"lib_name": "moz", "lib_version": "3.1.m", "quality": "80"}
@@ -1047,23 +1030,22 @@
                 "X-Entity-Length": f"{content_length}",
                 "Content-Type": "application/octet-stream",
                 "Content-Length": f"{content_length}",
                 "Accept-Encoding": "gzip",
             }
 
             headers.update(image_headers)
-            async with aiohttp.ClientSession() as session:
-                self.log_request('POST', url, headers, content)
-                async with session.post(url, headers=headers, data=content) as response:
-                    if response.status == 200:
-                        resp = await response.json()
-                        self.log_response(url, resp)
-                        return resp
-                    else:
-                        raise Exception("Failed to upload image")
+            self.log_request('POST', url, headers, content)
+            async with self._auth_session.post(url, headers=headers, data=content) as response:
+                if response.status == 200:
+                    resp = await response.json()
+                    self.log_response(url, resp)
+                    return resp
+                else:
+                    raise Exception("Failed to upload image")
 
         if not self.is_logged_in:
             raise Exception("You need to login before posting")
         
         now = datetime.now()
         timezone_offset = (datetime.now() - datetime.utcnow()).seconds
 
@@ -1104,21 +1086,17 @@
         if parent_post_id is not None:
             params["text_post_app_info"]["reply_id"] = parent_post_id
         params = json.dumps(params)
         payload = f"signed_body=SIGNATURE.{urllib.parse.quote(params)}"
         headers = __get_app_headers().copy()
 
         try:
-            async with aiohttp.ClientSession() as session:
-                self.log_request('POST', post_url, headers, payload)
-                async with session.post(post_url, headers=headers, data=payload) as response:
-                    data = await response.json()
-                    self.log_response(url, data)
+            res = await self._private_post(url=post_url, headers=headers,data=payload)
 
-                    if 'media' in data and 'pk' in data['media']:
-                        # Return the newly created post_id
-                        return data['media']['pk']
-                    else:
-                        raise Exception("Failed to post. Got response:\n" + str(response))
+            if 'media' in res and 'pk' in res['media']:
+                # Return the newly created post_id
+                return res['media']['pk']
+            else:
+                raise Exception("Failed to post. Got response:\n" + str(res))
         except Exception as e:
             print("[ERROR] ", e)
             raise
```

### Comparing `threads-api-1.1.8/threads_api/tests/get_threads_test.py` & `threads-api-1.1.9/threads_api/tests/get_threads_test.py`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.8/threads_api.egg-info/PKG-INFO` & `threads-api-1.1.9/threads_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.8
+Version: 1.1.9
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Daniel Saad
 Author-email: danielsaad777@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

