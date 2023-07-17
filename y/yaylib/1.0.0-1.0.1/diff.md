# Comparing `tmp/yaylib-1.0.0.tar.gz` & `tmp/yaylib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-1.0.0.tar", last modified: Sun Jul 16 09:15:39 2023, max compression
+gzip compressed data, was "yaylib-1.0.1.tar", last modified: Mon Jul 17 02:51:32 2023, max compression
```

## Comparing `yaylib-1.0.0.tar` & `yaylib-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 09:15:39.775312 yaylib-1.0.0/
--rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    10834 2023-07-16 09:15:39.773997 yaylib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     9970 2023-07-16 09:12:13.000000 yaylib-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 09:15:39.775312 yaylib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-07-16 09:10:03.000000 yaylib-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:15:39.726106 yaylib-1.0.0/tests/
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_call.py
--rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_cassandra.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_chat.py
--rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_group.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_misc.py
--rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_post.py
--rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_review.py
--rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_thread.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_user.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:15:39.733817 yaylib-1.0.0/yaylib/
--rw-rw-rw-   0        0        0      519 2023-07-09 07:25:01.000000 yaylib-1.0.0/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:15:39.773997 yaylib-1.0.0/yaylib/api/
--rw-rw-rw-   0        0        0      697 2023-07-09 07:25:01.000000 yaylib-1.0.0/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0    10272 2023-07-16 08:55:57.000000 yaylib-1.0.0/yaylib/api/api.py
--rw-rw-rw-   0        0        0     8657 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/call.py
--rw-rw-rw-   0        0        0     2699 2023-07-16 08:40:55.000000 yaylib-1.0.0/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    14793 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    23695 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/group.py
--rw-rw-rw-   0        0        0     8260 2023-07-16 08:52:39.000000 yaylib-1.0.0/yaylib/api/login.py
--rw-rw-rw-   0        0        0     7401 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    33692 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/post.py
--rw-rw-rw-   0        0        0     4488 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/review.py
--rw-rw-rw-   0        0        0     5945 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    24484 2023-07-16 08:42:11.000000 yaylib-1.0.0/yaylib/api/user.py
--rw-rw-rw-   0        0        0    86196 2023-07-16 08:15:00.000000 yaylib-1.0.0/yaylib/client.py
--rw-rw-rw-   0        0        0    19214 2023-07-16 09:09:09.000000 yaylib-1.0.0/yaylib/config.py
--rw-rw-rw-   0        0        0     2131 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/errors.py
--rw-rw-rw-   0        0        0    53336 2023-07-09 07:25:01.000000 yaylib-1.0.0/yaylib/models.py
--rw-rw-rw-   0        0        0    33222 2023-07-09 07:25:01.000000 yaylib-1.0.0/yaylib/responses.py
--rw-rw-rw-   0        0        0     4612 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:15:39.761319 yaylib-1.0.0/yaylib.egg-info/
--rw-rw-rw-   0        0        0    10834 2023-07-16 09:15:39.000000 yaylib-1.0.0/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-07-16 09:15:39.000000 yaylib-1.0.0/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 09:15:39.000000 yaylib-1.0.0/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-16 09:15:39.000000 yaylib-1.0.0/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 09:15:39.000000 yaylib-1.0.0/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 02:51:32.668216 yaylib-1.0.1/
+-rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    10834 2023-07-17 02:51:32.667009 yaylib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9970 2023-07-16 09:12:13.000000 yaylib-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 02:51:32.668216 yaylib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-07-16 09:10:03.000000 yaylib-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:51:32.617283 yaylib-1.0.1/tests/
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_call.py
+-rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_chat.py
+-rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_group.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_post.py
+-rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_review.py
+-rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_thread.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_user.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:51:32.625679 yaylib-1.0.1/yaylib/
+-rw-rw-rw-   0        0        0      519 2023-07-09 07:25:01.000000 yaylib-1.0.1/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:51:32.665852 yaylib-1.0.1/yaylib/api/
+-rw-rw-rw-   0        0        0      697 2023-07-09 07:25:01.000000 yaylib-1.0.1/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-07-16 09:33:07.000000 yaylib-1.0.1/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     8657 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     2699 2023-07-16 08:40:55.000000 yaylib-1.0.1/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    14881 2023-07-17 02:44:35.000000 yaylib-1.0.1/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    23695 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     8244 2023-07-16 09:33:16.000000 yaylib-1.0.1/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     7401 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    33692 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     4488 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     5945 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    24484 2023-07-16 08:42:11.000000 yaylib-1.0.1/yaylib/api/user.py
+-rw-rw-rw-   0        0        0    86196 2023-07-17 02:37:50.000000 yaylib-1.0.1/yaylib/client.py
+-rw-rw-rw-   0        0        0    19214 2023-07-17 02:44:43.000000 yaylib-1.0.1/yaylib/config.py
+-rw-rw-rw-   0        0        0     2131 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/errors.py
+-rw-rw-rw-   0        0        0    53336 2023-07-09 07:25:01.000000 yaylib-1.0.1/yaylib/models.py
+-rw-rw-rw-   0        0        0    33222 2023-07-09 07:25:01.000000 yaylib-1.0.1/yaylib/responses.py
+-rw-rw-rw-   0        0        0     4600 2023-07-16 09:33:56.000000 yaylib-1.0.1/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:51:32.652664 yaylib-1.0.1/yaylib.egg-info/
+-rw-rw-rw-   0        0        0    10834 2023-07-17 02:51:32.000000 yaylib-1.0.1/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-07-17 02:51:32.000000 yaylib-1.0.1/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 02:51:32.000000 yaylib-1.0.1/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-17 02:51:32.000000 yaylib-1.0.1/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-17 02:51:32.000000 yaylib-1.0.1/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-1.0.0/LICENSE` & `yaylib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/PKG-INFO` & `yaylib-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.0
+Version: 1.0.1
 Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.0 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.1 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
```

### Comparing `yaylib-1.0.0/README.md` & `yaylib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/setup.py` & `yaylib-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/tests/test_call.py` & `yaylib-1.0.1/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/tests/test_cassandra.py` & `yaylib-1.0.1/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/tests/test_chat.py` & `yaylib-1.0.1/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/tests/test_group.py` & `yaylib-1.0.1/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/tests/test_misc.py` & `yaylib-1.0.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/tests/test_post.py` & `yaylib-1.0.1/tests/test_post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/tests/test_review.py` & `yaylib-1.0.1/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/tests/test_thread.py` & `yaylib-1.0.1/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/tests/test_user.py` & `yaylib-1.0.1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/__init__.py` & `yaylib-1.0.1/yaylib/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/api/__init__.py` & `yaylib-1.0.1/yaylib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/api/api.py` & `yaylib-1.0.1/yaylib/api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     BadRequestError,
     AuthenticationError,
     ForbiddenError,
     NotFoundError,
     RateLimitError,
     YayServerError,
 )
-from ..utils import Configs, generate_uuid, load_credentials, save_credentials, decrypt
+from ..utils import Configs, generate_uuid, load_session, save_session, decrypt
 
 
 current_path = os.path.abspath(os.getcwd())
 
 
 class API:
     def __init__(
@@ -148,27 +148,27 @@
                     message = "Refresh token expired. Try logging in again."
                     raise AuthenticationError(message)
 
                 auth_retry_count += 1
                 self.logger.debug("Access token expired. Refreshing tokens...")
 
                 if auth_retry_count < max_auth_retries:
-                    credentials = load_credentials(base_path=self.base_path)
+                    credentials = load_session(base_path=self.base_path)
 
                     if credentials is not None and self.fernet is not None:
                         credentials = decrypt(
                             fernet=self.fernet, credentials=credentials
                         )
                         refresh_token = credentials["refresh_token"]
                         response = get_token(
                             self,
                             grant_type="refresh_token",
                             refresh_token=refresh_token,
                         )
-                        save_credentials(
+                        save_session(
                             base_path=self.base_path,
                             fernet=self.fernet,
                             access_token=response.access_token,
                             refresh_token=response.refresh_token,
                             user_id=response.user_id,
                         )
                         self.session.headers[
```

### Comparing `yaylib-1.0.0/yaylib/api/call.py` & `yaylib-1.0.1/yaylib/api/call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/api/cassandra.py` & `yaylib-1.0.1/yaylib/api/cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/api/chat.py` & `yaylib-1.0.1/yaylib/api/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,18 +370,19 @@
         data_type=ChatRoomsResponse,
         access_token=access_token,
     )
 
 
 def remove_chat_rooms(self, chat_room_ids: List[int], access_token: str = None):
     self._check_authorization(access_token)
+    chat_room_ids = [chat_room_ids] if isinstance(chat_room_ids, int) else chat_room_ids
     response = self._make_request(
         "POST",
-        endpoint=f"{Endpoints.CHAT_ROOMS_V2}/mass_destroy",
-        payload={"chat_room_ids[]": chat_room_ids},
+        endpoint=f"{Endpoints.CHAT_ROOMS_V1}/mass_destroy",
+        payload={"chat_room_ids": chat_room_ids},
         access_token=access_token,
     )
     self.logger.info(f"Chatrooms have been removed.")
     return response
 
 
 def report_chat_room(
```

### Comparing `yaylib-1.0.0/yaylib/api/group.py` & `yaylib-1.0.1/yaylib/api/group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/api/login.py` & `yaylib-1.0.1/yaylib/api/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
 from ..config import Configs, Endpoints
 from ..errors import AuthenticationError, ForbiddenError
 from ..responses import LoginUserResponse, LoginUpdateResponse, TokenResponse
 from ..utils import (
     Colors,
     console_print,
-    load_credentials,
-    save_credentials,
+    load_session,
+    save_session,
     decrypt,
     signed_info_calculating,
 )
 
 
 def change_email(
     self,
@@ -111,15 +111,15 @@
         return False
 
 
 def login_with_email(
     self, email: str, password: str, secret_key: str = None
 ) -> LoginUserResponse:
     if self.save_session:
-        credentials = load_credentials(base_path=self.base_path, check_email=email)
+        credentials = load_session(base_path=self.base_path, check_email=email)
         if credentials is not None and secret_key is not None:
             self.secret_key = secret_key
             self.fernet = Fernet(secret_key)
             credentials = decrypt(fernet=self.fernet, credentials=credentials)
             self.session.headers.setdefault(
                 "Authorization", f"Bearer {credentials['access_token']}"
             )
@@ -154,15 +154,15 @@
 
         console_print(
             f"Your 'secret_key' for {Colors.BOLD + email + Colors.RESET} is: {Colors.OKGREEN + secret_key.decode() + Colors.RESET}",
             "Please copy and securely store this key in a safe location.",
             "For more information, visit: https://github.com/qvco/yaylib/blob/master/docs/API-Reference/login/login.md",
         )
 
-        save_credentials(
+        save_session(
             base_path=self.base_path,
             fernet=self.fernet,
             access_token=response.access_token,
             refresh_token=response.refresh_token,
             user_id=response.user_id,
             email=email,
         )
```

### Comparing `yaylib-1.0.0/yaylib/api/misc.py` & `yaylib-1.0.1/yaylib/api/misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/api/post.py` & `yaylib-1.0.1/yaylib/api/post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/api/review.py` & `yaylib-1.0.1/yaylib/api/review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/api/thread.py` & `yaylib-1.0.1/yaylib/api/thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/api/user.py` & `yaylib-1.0.1/yaylib/api/user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/client.py` & `yaylib-1.0.1/yaylib/client.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/config.py` & `yaylib-1.0.1/yaylib/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 SOFTWARE.
 """
 
 from enum import Enum
 
 
 class Configs:
-    YAYLIB_VERSION = "1.0.0"
+    YAYLIB_VERSION = "1.0.1"
     YAY_API_VERSION = "3.16"
     YAY_VERSION_NAME = "3.16.1"
     YAY_API_VERSION_KEY = "e83a1d2588918c2061280427c88e6f56"
     YAY_API_KEY = "ccd59ee269c01511ba763467045c115779fcae3050238a252f1bd1a4b65cfec6"
     YAY_SHARED_KEY = "yayZ1"
     YAY_STORE_KEY = "yayZ1payment"
     ID_CARD_CHECK_SECRET_KEY = "4aa6d1c301a97154bc1098c2"
```

### Comparing `yaylib-1.0.0/yaylib/errors.py` & `yaylib-1.0.1/yaylib/errors.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/models.py` & `yaylib-1.0.1/yaylib/models.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/responses.py` & `yaylib-1.0.1/yaylib/responses.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.0/yaylib/utils.py` & `yaylib-1.0.1/yaylib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,23 +84,23 @@
             "access_token": fernet.decrypt(credentials.get("access_token")).decode(),
             "refresh_token": fernet.decrypt(credentials.get("refresh_token")).decode(),
         }
     )
     return credentials
 
 
-def save_credentials(
+def save_session(
     base_path: str,
     fernet,
     access_token: str,
     refresh_token: str,
     user_id: int,
     email: str = None,
 ):
-    credentials = load_credentials(base_path=base_path)
+    credentials = load_session(base_path=base_path)
     updated_credentials = {
         "access_token": access_token,
         "refresh_token": refresh_token,
         "user_id": user_id,
         "email": email,
     }
     if email is None:
@@ -108,15 +108,15 @@
 
     updated_credentials = encrypt(fernet, updated_credentials)
 
     with open(base_path + "credentials.json", "w") as f:
         json.dump(updated_credentials, f)
 
 
-def load_credentials(base_path: str, fernet=None, check_email: str = None):
+def load_session(base_path: str, fernet=None, check_email: str = None):
     if not os.path.exists(base_path + "credentials.json"):
         return None
 
     with open(base_path + "credentials.json", "r") as f:
         credentials = json.load(f)
 
     result = all(
```

### Comparing `yaylib-1.0.0/yaylib.egg-info/PKG-INFO` & `yaylib-1.0.1/yaylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.0
+Version: 1.0.1
 Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.0 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.1 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
```

### Comparing `yaylib-1.0.0/yaylib.egg-info/SOURCES.txt` & `yaylib-1.0.1/yaylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

