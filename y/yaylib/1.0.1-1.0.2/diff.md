# Comparing `tmp/yaylib-1.0.1.tar.gz` & `tmp/yaylib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-1.0.1.tar", last modified: Mon Jul 17 02:51:32 2023, max compression
+gzip compressed data, was "yaylib-1.0.2.tar", last modified: Mon Jul 17 07:00:31 2023, max compression
```

## Comparing `yaylib-1.0.1.tar` & `yaylib-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 02:51:32.668216 yaylib-1.0.1/
--rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    10834 2023-07-17 02:51:32.667009 yaylib-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9970 2023-07-16 09:12:13.000000 yaylib-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 02:51:32.668216 yaylib-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-07-16 09:10:03.000000 yaylib-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:51:32.617283 yaylib-1.0.1/tests/
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_call.py
--rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_cassandra.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_chat.py
--rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_group.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_misc.py
--rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_post.py
--rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_review.py
--rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_thread.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.1/tests/test_user.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:51:32.625679 yaylib-1.0.1/yaylib/
--rw-rw-rw-   0        0        0      519 2023-07-09 07:25:01.000000 yaylib-1.0.1/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:51:32.665852 yaylib-1.0.1/yaylib/api/
--rw-rw-rw-   0        0        0      697 2023-07-09 07:25:01.000000 yaylib-1.0.1/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-07-16 09:33:07.000000 yaylib-1.0.1/yaylib/api/api.py
--rw-rw-rw-   0        0        0     8657 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/call.py
--rw-rw-rw-   0        0        0     2699 2023-07-16 08:40:55.000000 yaylib-1.0.1/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    14881 2023-07-17 02:44:35.000000 yaylib-1.0.1/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    23695 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/group.py
--rw-rw-rw-   0        0        0     8244 2023-07-16 09:33:16.000000 yaylib-1.0.1/yaylib/api/login.py
--rw-rw-rw-   0        0        0     7401 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    33692 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/post.py
--rw-rw-rw-   0        0        0     4488 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/review.py
--rw-rw-rw-   0        0        0     5945 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    24484 2023-07-16 08:42:11.000000 yaylib-1.0.1/yaylib/api/user.py
--rw-rw-rw-   0        0        0    86196 2023-07-17 02:37:50.000000 yaylib-1.0.1/yaylib/client.py
--rw-rw-rw-   0        0        0    19214 2023-07-17 02:44:43.000000 yaylib-1.0.1/yaylib/config.py
--rw-rw-rw-   0        0        0     2131 2023-07-16 04:28:15.000000 yaylib-1.0.1/yaylib/errors.py
--rw-rw-rw-   0        0        0    53336 2023-07-09 07:25:01.000000 yaylib-1.0.1/yaylib/models.py
--rw-rw-rw-   0        0        0    33222 2023-07-09 07:25:01.000000 yaylib-1.0.1/yaylib/responses.py
--rw-rw-rw-   0        0        0     4600 2023-07-16 09:33:56.000000 yaylib-1.0.1/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:51:32.652664 yaylib-1.0.1/yaylib.egg-info/
--rw-rw-rw-   0        0        0    10834 2023-07-17 02:51:32.000000 yaylib-1.0.1/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-07-17 02:51:32.000000 yaylib-1.0.1/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 02:51:32.000000 yaylib-1.0.1/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-17 02:51:32.000000 yaylib-1.0.1/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-17 02:51:32.000000 yaylib-1.0.1/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 07:00:31.115517 yaylib-1.0.2/
+-rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    10834 2023-07-17 07:00:31.115517 yaylib-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9970 2023-07-16 09:12:13.000000 yaylib-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 07:00:31.115517 yaylib-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-07-16 09:10:03.000000 yaylib-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:00:31.079666 yaylib-1.0.2/tests/
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_call.py
+-rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_chat.py
+-rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_group.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_post.py
+-rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_review.py
+-rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_thread.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_user.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:00:31.086984 yaylib-1.0.2/yaylib/
+-rw-rw-rw-   0        0        0      519 2023-07-09 07:25:01.000000 yaylib-1.0.2/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:00:31.114515 yaylib-1.0.2/yaylib/api/
+-rw-rw-rw-   0        0        0      697 2023-07-09 07:25:01.000000 yaylib-1.0.2/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0    10401 2023-07-17 06:36:16.000000 yaylib-1.0.2/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     8657 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     2699 2023-07-16 08:40:55.000000 yaylib-1.0.2/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    14881 2023-07-17 02:44:35.000000 yaylib-1.0.2/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    23695 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     8244 2023-07-16 09:33:16.000000 yaylib-1.0.2/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     7393 2023-07-17 06:13:19.000000 yaylib-1.0.2/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    33692 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     4488 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     5945 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    24492 2023-07-17 06:58:52.000000 yaylib-1.0.2/yaylib/api/user.py
+-rw-rw-rw-   0        0        0    86196 2023-07-17 02:37:50.000000 yaylib-1.0.2/yaylib/client.py
+-rw-rw-rw-   0        0        0    19214 2023-07-17 06:59:15.000000 yaylib-1.0.2/yaylib/config.py
+-rw-rw-rw-   0        0        0     2131 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/errors.py
+-rw-rw-rw-   0        0        0    53336 2023-07-09 07:25:01.000000 yaylib-1.0.2/yaylib/models.py
+-rw-rw-rw-   0        0        0    33222 2023-07-09 07:25:01.000000 yaylib-1.0.2/yaylib/responses.py
+-rw-rw-rw-   0        0        0     4600 2023-07-16 09:33:56.000000 yaylib-1.0.2/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:00:31.103398 yaylib-1.0.2/yaylib.egg-info/
+-rw-rw-rw-   0        0        0    10834 2023-07-17 07:00:30.000000 yaylib-1.0.2/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-07-17 07:00:31.000000 yaylib-1.0.2/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 07:00:30.000000 yaylib-1.0.2/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-17 07:00:30.000000 yaylib-1.0.2/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-17 07:00:30.000000 yaylib-1.0.2/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-1.0.1/LICENSE` & `yaylib-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/PKG-INFO` & `yaylib-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.1
+Version: 1.0.2
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
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.1 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.2 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
```

### Comparing `yaylib-1.0.1/README.md` & `yaylib-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/setup.py` & `yaylib-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/tests/test_call.py` & `yaylib-1.0.2/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/tests/test_cassandra.py` & `yaylib-1.0.2/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/tests/test_chat.py` & `yaylib-1.0.2/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/tests/test_group.py` & `yaylib-1.0.2/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/tests/test_misc.py` & `yaylib-1.0.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/tests/test_post.py` & `yaylib-1.0.2/tests/test_post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/tests/test_review.py` & `yaylib-1.0.2/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/tests/test_thread.py` & `yaylib-1.0.2/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/tests/test_user.py` & `yaylib-1.0.2/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/__init__.py` & `yaylib-1.0.2/yaylib/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/api/__init__.py` & `yaylib-1.0.2/yaylib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/api/api.py` & `yaylib-1.0.2/yaylib/api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,19 +203,19 @@
             "Received API response:\n\n"
             f"Status Code: {response.status_code}\n\n"
             f"Headers: {response.headers}\n\n"
             f"Response: {response.text}\n"
         )
 
         try:
-            json_response = response.json()
+            formatted_response = response.json()
         except JSONDecodeError:
-            return response.text
+            formatted_response = response.text
 
-        return self._handle_response(response, json_response)
+        return self._handle_response(response, formatted_response)
 
     def _make_request(
         self,
         method: str,
         endpoint: str,
         params: dict = None,
         payload: dict = None,
@@ -241,31 +241,34 @@
         return data
 
     def _check_authorization(self, access_token) -> None:
         if self.session.headers.get("Authorization") is None and access_token is None:
             message = "Authorization is not present in the header."
             raise AuthenticationError(message)
 
-    def _handle_response(self, response, json_response):
-        translated_response = self._translate_error_message(json_response)
+    def _handle_response(self, response, formatted_response):
+        translated_response = formatted_response
+        if isinstance(formatted_response, dict):
+            translated_response = self._translate_error_message(formatted_response)
+
         if response.status_code == 400:
             raise BadRequestError(translated_response)
         if response.status_code == 401:
             raise AuthenticationError(translated_response)
         if response.status_code == 403:
             raise ForbiddenError(translated_response)
         if response.status_code == 404:
             raise NotFoundError(translated_response)
         if response.status_code == 429:
             raise RateLimitError(translated_response)
         if response.status_code == 500:
             raise YayServerError(translated_response)
         if response.status_code and not 200 <= response.status_code < 300:
             raise HTTPError(translated_response)
-        return json_response
+        return formatted_response
 
     def _translate_error_message(self, response):
         if self.err_lang == "ja":
             try:
                 error_code = response.get("error_code", None)
                 if error_code is not None:
                     error_type = ErrorType(error_code)
```

### Comparing `yaylib-1.0.1/yaylib/api/call.py` & `yaylib-1.0.2/yaylib/api/call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/api/cassandra.py` & `yaylib-1.0.2/yaylib/api/cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/api/chat.py` & `yaylib-1.0.2/yaylib/api/chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/api/group.py` & `yaylib-1.0.2/yaylib/api/group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/api/login.py` & `yaylib-1.0.2/yaylib/api/login.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/api/misc.py` & `yaylib-1.0.2/yaylib/api/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,19 +216,19 @@
 
     presigned_urls = get_file_upload_presigned_urls(
         self, [original_url, thumb_url], access_token=access_token
     )
 
     with open(image_path, "rb") as f:
         response = httpx.put(presigned_urls[0].url, data=f.read())
-        self._handle_response(response)
+        response.raise_for_status()
 
     with open(image_path, "rb") as f:
         response = httpx.put(presigned_urls[1].url, data=f.read())
-        self._handle_response(response)
+        response.raise_for_status()
 
     self.logger.info(f"Image '{filename}{ext}' is uploaded")
 
     return presigned_urls[0].filename
 
 
 def upload_video(self, video_path: str, access_token: str = None):
```

### Comparing `yaylib-1.0.1/yaylib/api/post.py` & `yaylib-1.0.2/yaylib/api/post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/api/review.py` & `yaylib-1.0.2/yaylib/api/review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/api/thread.py` & `yaylib-1.0.2/yaylib/api/thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/api/user.py` & `yaylib-1.0.2/yaylib/api/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,23 +423,23 @@
 
 
 def reduce_kenta_penalty(self, user_id: int, access_token: str = None):
     self._check_authorization(access_token)
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
-        endpoint=f"{Configs.YAY_API_URL}api/v3/users/{user_id}/reduce_penalty",
+        endpoint=f"{Configs.YAY_API_URL}/api/v3/users/{user_id}/reduce_penalty",
         payload={
-            "uuid": self.uuid,
-            "api_key": self.api_key,
+            "app_version": self.api_version,
             "timestamp": timestamp,
+            "api_key": self.api_key,
             "signed_info": signed_info_calculating(self.device_uuid, timestamp),
             "signed_version": signed_version_calculating(),
+            "uuid": self.uuid,
         },
-        data_type=CreatePostResponse,
         access_token=access_token,
     )
     self.logger.info("Penalty has been reduced.")
     return response
 
 
 def refresh_counter(self, counter: str, access_token: str = None):
```

### Comparing `yaylib-1.0.1/yaylib/client.py` & `yaylib-1.0.2/yaylib/client.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/config.py` & `yaylib-1.0.2/yaylib/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 SOFTWARE.
 """
 
 from enum import Enum
 
 
 class Configs:
-    YAYLIB_VERSION = "1.0.1"
+    YAYLIB_VERSION = "1.0.2"
     YAY_API_VERSION = "3.16"
     YAY_VERSION_NAME = "3.16.1"
     YAY_API_VERSION_KEY = "e83a1d2588918c2061280427c88e6f56"
     YAY_API_KEY = "ccd59ee269c01511ba763467045c115779fcae3050238a252f1bd1a4b65cfec6"
     YAY_SHARED_KEY = "yayZ1"
     YAY_STORE_KEY = "yayZ1payment"
     ID_CARD_CHECK_SECRET_KEY = "4aa6d1c301a97154bc1098c2"
```

### Comparing `yaylib-1.0.1/yaylib/errors.py` & `yaylib-1.0.2/yaylib/errors.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/models.py` & `yaylib-1.0.2/yaylib/models.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/responses.py` & `yaylib-1.0.2/yaylib/responses.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib/utils.py` & `yaylib-1.0.2/yaylib/utils.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.1/yaylib.egg-info/PKG-INFO` & `yaylib-1.0.2/yaylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.1
+Version: 1.0.2
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
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.1 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.2 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
```

### Comparing `yaylib-1.0.1/yaylib.egg-info/SOURCES.txt` & `yaylib-1.0.2/yaylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

