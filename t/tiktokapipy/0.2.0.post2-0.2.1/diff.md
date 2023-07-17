# Comparing `tmp/tiktokapipy-0.2.0.post2.tar.gz` & `tmp/tiktokapipy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktokapipy-0.2.0.post2.tar", last modified: Fri Jul  7 13:48:51 2023, max compression
+gzip compressed data, was "tiktokapipy-0.2.1.tar", last modified: Mon Jul 17 20:27:13 2023, max compression
```

## Comparing `tiktokapipy-0.2.0.post2.tar` & `tiktokapipy-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.773075 tiktokapipy-0.2.0.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/src/tiktokapipy/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/async_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/raw_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/src/tiktokapipy/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/util/deferred_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/util/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/util/signing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-07 13:48:51.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-07 13:48:51.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:48:51.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 13:48:51.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 13:48:51.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/tests/test_challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/tests/test_slideshow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.218665 tiktokapipy-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-17 20:27:13.218665 tiktokapipy-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:27:13.218665 tiktokapipy-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.210665 tiktokapipy-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.214665 tiktokapipy-0.2.1/src/tiktokapipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/async_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.214665 tiktokapipy-0.2.1/src/tiktokapipy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/raw_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.218665 tiktokapipy-0.2.1/src/tiktokapipy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/util/deferred_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/util/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/util/signing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.214665 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-17 20:27:13.000000 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-17 20:27:13.000000 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:27:13.000000 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 20:27:13.000000 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 20:27:13.000000 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.218665 tiktokapipy-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/tests/test_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/tests/test_slideshow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/tests/test_video.py
```

### Comparing `tiktokapipy-0.2.0.post2/LICENSE` & `tiktokapipy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/PKG-INFO` & `tiktokapipy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.2.0.post2
+Version: 0.2.1
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.0.post2 Summary: Asyncio
-TikTok data scraping tool Author-email: Russell Newton
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.1 Summary: Asyncio TikTok
+data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tiktokapipy-0.2.0.post2/README.md` & `tiktokapipy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/pyproject.toml` & `tiktokapipy-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tiktokapipy"
-version = "0.2.0post2"
+version = "0.2.1"
 authors = [
     { name="Russell Newton", email="russell.newton01@gmail.com" },
 ]
 description = "Asyncio TikTok data scraping tool"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/__init__.py` & `tiktokapipy-0.2.1/src/tiktokapipy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,56 @@
+from collections import defaultdict
+
+
 class TikTokAPIError(Exception):
     """Raised when the API encounters an error"""
 
     pass
 
 
 class TikTokAPIWarning(RuntimeWarning):
     pass
 
 
-ERROR_CODES = {
-    0: "OK",
-    450: "CLIENT_PAGE_ERROR",
-    10000: "VERIFY_CODE",
-    10101: "SERVER_ERROR_NOT_500",
-    10102: "USER_NOT_LOGIN",
-    10111: "NET_ERROR",
-    10113: "SHARK_SLIDE",
-    10114: "SHARK_BLOCK",
-    10119: "LIVE_NEED_LOGIN",
-    10202: "USER_NOT_EXIST",
-    10203: "MUSIC_NOT_EXIST",
-    10204: "VIDEO_NOT_EXIST",
-    10205: "HASHTAG_NOT_EXIST",
-    10208: "EFFECT_NOT_EXIST",
-    10209: "HASHTAG_BLACK_LIST",
-    10210: "LIVE_NOT_EXIST",
-    10211: "HASHTAG_SENSITIVITY_WORD",
-    10212: "HASHTAG_UNSHELVE",
-    10213: "VIDEO_LOW_AGE_M",
-    10214: "VIDEO_LOW_AGE_T",
-    10215: "VIDEO_ABNORMAL",
-    10216: "VIDEO_PRIVATE_BY_USER",
-    10217: "VIDEO_FIRST_REVIEW_UNSHELVE",
-    10218: "MUSIC_UNSHELVE",
-    10219: "MUSIC_NO_COPYRIGHT",
-    10220: "VIDEO_UNSHELVE_BY_MUSIC",
-    10221: "USER_BAN",
-    10222: "USER_PRIVATE",
-    10223: "USER_FTC",
-    10224: "GAME_NOT_EXIST",
-    10225: "USER_UNIQUE_SENSITIVITY",
-    10227: "VIDEO_NEED_RECHECK",
-    10228: "VIDEO_RISK",
-    10229: "VIDEO_R_MASK",
-    10230: "VIDEO_RISK_MASK",
-    10231: "VIDEO_GEOFENCE_BLOCK",
-    10404: "FYP_VIDEO_LIST_LIMIT",
-    "undefined": "MEDIA_ERROR",
-}
+ERROR_CODES = defaultdict(
+    lambda: "Unknown Error",
+    {
+        0: "OK",
+        450: "CLIENT_PAGE_ERROR",
+        10000: "VERIFY_CODE",
+        10101: "SERVER_ERROR_NOT_500",
+        10102: "USER_NOT_LOGIN",
+        10111: "NET_ERROR",
+        10113: "SHARK_SLIDE",
+        10114: "SHARK_BLOCK",
+        10119: "LIVE_NEED_LOGIN",
+        10202: "USER_NOT_EXIST",
+        10203: "MUSIC_NOT_EXIST",
+        10204: "VIDEO_NOT_EXIST",
+        10205: "HASHTAG_NOT_EXIST",
+        10208: "EFFECT_NOT_EXIST",
+        10209: "HASHTAG_BLACK_LIST",
+        10210: "LIVE_NOT_EXIST",
+        10211: "HASHTAG_SENSITIVITY_WORD",
+        10212: "HASHTAG_UNSHELVE",
+        10213: "VIDEO_LOW_AGE_M",
+        10214: "VIDEO_LOW_AGE_T",
+        10215: "VIDEO_ABNORMAL",
+        10216: "VIDEO_PRIVATE_BY_USER",
+        10217: "VIDEO_FIRST_REVIEW_UNSHELVE",
+        10218: "MUSIC_UNSHELVE",
+        10219: "MUSIC_NO_COPYRIGHT",
+        10220: "VIDEO_UNSHELVE_BY_MUSIC",
+        10221: "USER_BAN",
+        10222: "USER_PRIVATE",
+        10223: "USER_FTC",
+        10224: "GAME_NOT_EXIST",
+        10225: "USER_UNIQUE_SENSITIVITY",
+        10227: "VIDEO_NEED_RECHECK",
+        10228: "VIDEO_RISK",
+        10229: "VIDEO_R_MASK",
+        10230: "VIDEO_RISK_MASK",
+        10231: "VIDEO_GEOFENCE_BLOCK",
+        10404: "FYP_VIDEO_LIST_LIMIT",
+        "undefined": "MEDIA_ERROR",
+    },
+)
```

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/api.py` & `tiktokapipy-0.2.1/src/tiktokapipy/api.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/async_api.py` & `tiktokapipy-0.2.1/src/tiktokapipy/async_api.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/__init__.py` & `tiktokapipy-0.2.1/src/tiktokapipy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/challenge.py` & `tiktokapipy-0.2.1/src/tiktokapipy/models/challenge.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/comment.py` & `tiktokapipy-0.2.1/src/tiktokapipy/models/comment.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/raw_data.py` & `tiktokapipy-0.2.1/src/tiktokapipy/models/raw_data.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/user.py` & `tiktokapipy-0.2.1/src/tiktokapipy/models/user.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/video.py` & `tiktokapipy-0.2.1/src/tiktokapipy/models/video.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Video data models"""
 
 from __future__ import annotations
 
 from datetime import datetime
 from functools import cached_property
-from io import BytesIO
 from typing import Any, ForwardRef, List, Optional, Union
 
 from playwright.async_api import BrowserContext as AsyncBrowserContext
-from playwright.sync_api import BrowserContext as SyncBrowserContext
 from pydantic import AliasChoices, Field, computed_field
 from tiktokapipy import TikTokAPIError
 from tiktokapipy.models import CamelCaseModel, TitleCaseModel
 from tiktokapipy.util.deferred_collectors import (
     DeferredChallengeIterator,
     DeferredCommentIterator,
     DeferredUserGetterAsync,
@@ -80,15 +78,15 @@
 
 
 class MusicData(CamelCaseModel):
     """Contains data about the music within a video"""
 
     id: int
     title: str
-    play_url: str
+    play_url: Optional[str] = None
     author_name: Optional[str] = None
     duration: int
     original: bool
     album: Optional[str] = None
 
     cover_large: str
     cover_medium: str
@@ -252,89 +250,19 @@
             self.author if isinstance(self.author, str) else self.author.unique_id
         )
         if isinstance(self._api.context, AsyncBrowserContext):
             return DeferredUserGetterAsync(self._api, unique_id)
         else:
             return DeferredUserGetterSync(self._api, unique_id)
 
-    async def download_async(self) -> BytesIO:
-        if self.image_post:
-            raise TikTokAPIError(
-                "Downloading slide shows is not directly supported yet."
-            )
-        if self._api is None:
-            raise TikTokAPIError(
-                "A TikTokAPI must be attached to video._api before retrieving creator data."
-            )
-        if isinstance(self._api.context, SyncBrowserContext):
-            raise TikTokAPIError(
-                "Attempting to use TikTokAPI in an asynchronous context. Use `download_sync()` instead."
-            )
-
-        from playwright.async_api import Page
-
-        page: Page = await self._api.context.new_page()
-        response = await page.goto(
-            self.video.download_addr, referer="https://www.tiktok.com"
-        )
-        return BytesIO(await response.body())
-
-    def download_sync(self) -> BytesIO:
-        if self.image_post:
-            raise TikTokAPIError(
-                "Downloading slide shows is not directly supported yet."
-            )
-        if self._api is None:
-            raise TikTokAPIError(
-                "A TikTokAPI must be attached to video._api before retrieving creator data."
-            )
-        if isinstance(self._api.context, AsyncBrowserContext):
-            raise TikTokAPIError(
-                "Attempting to use AsyncTikTokAPI in a synchronous context. Use `await download_async()` instead."
-            )
-
-        from playwright.sync_api import Page
-
-        page: Page = self._api.context.new_page()
-        page.add_init_script(
-            """
-    if (navigator.webdriver === false) {
-    // Post Chrome 89.0.4339.0 and already good
-    } else if (navigator.webdriver === undefined) {
-    // Pre Chrome 89.0.4339.0 and already good
-    } else {
-    // Pre Chrome 88.0.4291.0 and needs patching
-    delete Object.getPrototypeOf(navigator).webdriver
-    }
-    """
-        )
-        # response = page.goto(self.video.download_addr)
-        print(page.context.cookies())
-        if len(page.context.cookies()) == 0:
-            page.goto("https://www.tiktok.com")
-            page.reload()
-            page.wait_for_timeout(5000)
-        print(page.context.cookies())
-        cookie_header = "; ".join(
-            f"{cookie['name']}={cookie['value']}"
-            for cookie in page.context.cookies()
-            if cookie["domain"] == ".tiktok.com"
-        )
-        response2 = page.request.get(
-            self.video.download_addr,
-            headers={
-                "Referer": "https://www.tiktok.com",
-                "Sec-Fetch-Dest": "video",
-                "Sec-Fetch-Mode": "no-cors",
-                "Sec-Fetch-Site": "same-site",
-                "Cookie": cookie_header,
-            },
-        )
-        page.close()
-        return BytesIO(response2.body())
+    @computed_field(repr=False)
+    @cached_property
+    def url(self) -> str:
+        """The url to the video on TikTok."""
+        return video_link(self.id)
 
 
 del Challenge, LightChallenge, Comment, LightUser, User, UserStats
 
 
 from tiktokapipy.models.challenge import Challenge, LightChallenge  # noqa E402
 from tiktokapipy.models.comment import Comment  # noqa E402
```

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/util/deferred_collectors.py` & `tiktokapipy-0.2.1/src/tiktokapipy/util/deferred_collectors.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/util/queries.py` & `tiktokapipy-0.2.1/src/tiktokapipy/util/queries.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy/util/signing.py` & `tiktokapipy-0.2.1/src/tiktokapipy/util/signing.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/PKG-INFO` & `tiktokapipy-0.2.1/src/tiktokapipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.2.0.post2
+Version: 0.2.1
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.0.post2 Summary: Asyncio
-TikTok data scraping tool Author-email: Russell Newton
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.1 Summary: Asyncio TikTok
+data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/SOURCES.txt` & `tiktokapipy-0.2.1/src/tiktokapipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/tests/test_challenge.py` & `tiktokapipy-0.2.1/tests/test_challenge.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/tests/test_slideshow.py` & `tiktokapipy-0.2.1/tests/test_slideshow.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/tests/test_user.py` & `tiktokapipy-0.2.1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post2/tests/test_video.py` & `tiktokapipy-0.2.1/tests/test_video.py`

 * *Files identical despite different names*

