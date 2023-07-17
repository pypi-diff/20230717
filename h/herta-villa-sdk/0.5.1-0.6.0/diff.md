# Comparing `tmp/herta_villa_sdk-0.5.1.tar.gz` & `tmp/herta_villa_sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.5.1.tar", last modified: Fri Jul 14 10:04:15 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.6.0.tar", last modified: Mon Jul 17 10:53:00 2023, max compression
```

## Comparing `herta_villa_sdk-0.5.1.tar` & `herta_villa_sdk-0.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1068 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/LICENSE
--rw-r--r--   0        0        0     4060 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/README.md
--rw-r--r--   0        0        0      668 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/__init__.py
--rw-r--r--   0        0        0      782 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/auth.py
--rw-r--r--   0        0        0     1491 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/base.py
--rw-r--r--   0        0        0      520 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/emoticon.py
--rw-r--r--   0        0        0      611 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/img.py
--rw-r--r--   0        0        0     2174 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/member.py
--rw-r--r--   0        0        0     2710 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/message.py
--rw-r--r--   0        0        0     4422 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/apis/role.py
--rw-r--r--   0        0        0     4190 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/apis/room.py
--rw-r--r--   0        0        0      645 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/apis/villa.py
--rw-r--r--   0        0        0     7296 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/bot.py
--rw-r--r--   0        0        0     5398 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/event.py
--rw-r--r--   0        0        0     1016 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/exception.py
--rw-r--r--   0        0        0     1481 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/match.py
--rw-r--r--   0        0        0      353 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/__init__.py
--rw-r--r--   0        0        0     3799 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/chain.py
--rw-r--r--   0        0        0     1414 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/image.py
--rw-r--r--   0        0        0      927 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/post.py
--rw-r--r--   0        0        0     6289 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/text.py
--rw-r--r--   0        0        0      442 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/types.py
--rw-r--r--   0        0        0     6280 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/model.py
--rw-r--r--   0        0        0      970 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/server/__init__.py
--rw-r--r--   0        0        0     1287 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/server/aiohttp.py
--rw-r--r--   0        0        0     1548 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/server/fastapi.py
--rw-r--r--   0        0        0     2888 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/server/internal.py
--rw-r--r--   0        0        0      564 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/typing.py
--rw-r--r--   0        0        0      563 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/version.py
--rw-r--r--   0        0        0     2234 2023-07-14 10:04:15.456239 herta_villa_sdk-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      528 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/tests/test_utils.py
--rw-r--r--   0        0        0     4818 1970-01-01 00:00:00.000000 herta_villa_sdk-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4420 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/README.md
+-rw-r--r--   0        0        0      668 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/__init__.py
+-rw-r--r--   0        0        0      782 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/auth.py
+-rw-r--r--   0        0        0     1739 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/base.py
+-rw-r--r--   0        0        0      520 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/emoticon.py
+-rw-r--r--   0        0        0      611 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/img.py
+-rw-r--r--   0        0        0     2174 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/member.py
+-rw-r--r--   0        0        0     2710 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/message.py
+-rw-r--r--   0        0        0     4422 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/role.py
+-rw-r--r--   0        0        0     4190 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/room.py
+-rw-r--r--   0        0        0      645 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/villa.py
+-rw-r--r--   0        0        0     7869 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/bot.py
+-rw-r--r--   0        0        0     5398 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/event.py
+-rw-r--r--   0        0        0     1060 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/exception.py
+-rw-r--r--   0        0        0     1481 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/match.py
+-rw-r--r--   0        0        0      353 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     3799 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1414 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/image.py
+-rw-r--r--   0        0        0      927 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6289 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/text.py
+-rw-r--r--   0        0        0      442 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/types.py
+-rw-r--r--   0        0        0     6280 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/model.py
+-rw-r--r--   0        0        0      970 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/server/__init__.py
+-rw-r--r--   0        0        0     1383 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/server/aiohttp.py
+-rw-r--r--   0        0        0     1653 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/server/fastapi.py
+-rw-r--r--   0        0        0     3081 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/server/internal.py
+-rw-r--r--   0        0        0      564 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/typing.py
+-rw-r--r--   0        0        0      563 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/utils.py
+-rw-r--r--   0        0        0       58 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/version.py
+-rw-r--r--   0        0        0     2278 2023-07-17 10:53:00.129792 herta_villa_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      528 2023-07-17 10:52:21.361139 herta_villa_sdk-0.6.0/tests/test_utils.py
+-rw-r--r--   0        0        0     5202 1970-01-01 00:00:00.000000 herta_villa_sdk-0.6.0/PKG-INFO
```

### Comparing `herta_villa_sdk-0.5.1/LICENSE` & `herta_villa_sdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/README.md` & `herta_villa_sdk-0.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -28,18 +28,30 @@
 ## 快速开始
 
 你需要拥有一个[大别野](https://dby.miyoushe.com/chat)机器人。可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)（`OpenVilla`）申请。
 
 ```python
 from hertavilla import MessageChain, SendMessageEvent, VillaBot, run
 
+
+PUB_KEY = """-----BEGIN PUBLIC KEY-----
+aaa
+bbb
+ccc
+-----END PUBLIC KEY-----
+"""  # 开放平台 pub_key
+# 需要注意 `-----BEGIN PUBLIC KEY-----` 前没有换行符
+#  `-----END PUBLIC KEY-----` 后有一个换行符
+# 目前从网页端复制下来的时候会为一串 pub_key，需要将空格转为换行
+
 bot = VillaBot(
     "bot_id",  # 这里填写 bot_id
     "bot_secret",  # 这里填写 secret
     "/",  # bot 回调 endpoint
+    PUB_KEY,  # 开放平台提供的 pub_key
 )
 
 
 @bot.startswith("/")  # 注册一个消息匹配器，匹配前缀为 / 的消息
 async def _(event: SendMessageEvent, bot: VillaBot):
     message = event.message
     if str(message[1]) == "/hello":
```

### Comparing `herta_villa_sdk-0.5.1/hertavilla/__init__.py` & `herta_villa_sdk-0.6.0/hertavilla/__init__.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/apis/auth.py` & `herta_villa_sdk-0.6.0/hertavilla/apis/auth.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/apis/base.py` & `herta_villa_sdk-0.6.0/hertavilla/apis/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 from __future__ import annotations
 
+import hashlib
+import hmac
 import logging
 from typing import Any, Literal
 
-from hertavilla.exception import HTTPStatusError, raise_exception
+from hertavilla.exception import (
+    HTTPStatusError,
+    raise_exception,
+)
 
 from aiohttp import ClientSession
 
 logger = logging.getLogger("hertavilla.api")
 BASE_API = "https://bbs-api.miyoushe.com/vila/api/bot/platform"
 
 
 class _BaseAPIMixin:
-    def __init__(self, bot_id: str, secret: str):
+    def __init__(
+        self,
+        bot_id: str,
+        secret: str,
+        pub_key: str,
+    ):
         self.bot_id = bot_id
         self.secret = secret
+        self.pub_key = pub_key
 
     def _make_header(self, villa_id: int) -> dict[str, str]:
+        secret = hmac.new(
+            self.pub_key.encode(),
+            self.secret.encode(),
+            hashlib.sha256,
+        ).hexdigest()
         return {
             "x-rpc-bot_id": self.bot_id,
-            "x-rpc-bot_secret": self.secret,
+            "x-rpc-bot_secret": secret,
             "x-rpc-bot_villa_id": str(villa_id),
         }
 
-    async def base_request(  # noqa: PLR0913
+    async def base_request(
         self,
         api: str,
         method: Literal["POST"] | Literal["GET"],
         /,
         villa_id: int | None = None,
         *,
         data: dict[str, Any] | None = None,
```

### Comparing `herta_villa_sdk-0.5.1/hertavilla/apis/emoticon.py` & `herta_villa_sdk-0.6.0/hertavilla/apis/emoticon.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/apis/img.py` & `herta_villa_sdk-0.6.0/hertavilla/apis/img.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/apis/member.py` & `herta_villa_sdk-0.6.0/hertavilla/apis/member.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/apis/message.py` & `herta_villa_sdk-0.6.0/hertavilla/apis/message.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/apis/role.py` & `herta_villa_sdk-0.6.0/hertavilla/apis/role.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/apis/room.py` & `herta_villa_sdk-0.6.0/hertavilla/apis/room.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/apis/villa.py` & `herta_villa_sdk-0.6.0/hertavilla/apis/villa.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/bot.py` & `herta_villa_sdk-0.6.0/hertavilla/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from __future__ import annotations
 
 import asyncio
+import base64
 from dataclasses import dataclass
 import logging
 import re
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Coroutine,
     Generic,
     NamedTuple,
     TypeVar,
 )
+import urllib.parse
 
 from hertavilla.apis.auth import AuthAPIMixin
 from hertavilla.apis.img import ImgAPIMixin
 from hertavilla.apis.member import MemberAPIMixin
 from hertavilla.apis.message import MessageAPIMixin
 from hertavilla.apis.role import RoleAPIMixin
 from hertavilla.apis.room import RoomAPIMixin
 from hertavilla.apis.villa import VillaAPIMixin
 from hertavilla.match import Endswith, Keywords, Match, Regex, Startswith
 
+import rsa
+
 if TYPE_CHECKING:
     from hertavilla.event import Command, Event, SendMessageEvent, Template
     from hertavilla.message import MessageChain
 
 
 TE = TypeVar("TE", bound="Event")
 
@@ -71,20 +75,23 @@
     ImgAPIMixin,
 ):
     def __init__(
         self,
         bot_id: str,
         secret: str,
         callback_endpoint: str,
+        pub_key: str,
         bot_info: "Template" | None = None,
     ) -> None:
         from hertavilla.event import SendMessageEvent
 
-        self.bot_id = bot_id
-        self.secret = secret
+        super().__init__(bot_id, secret, pub_key)
+        self.rsa_pub_key = rsa.PublicKey.load_pkcs1_openssl_pem(
+            pub_key.encode(),
+        )
         self._bot_info = bot_info
         self.callback_endpoint = callback_endpoint
         self.handlers: list[Handler] = []
         self.message_handlers: list[MessageHandler] = []
         self.register_handler(SendMessageEvent, self.message_handler)
 
     @property
@@ -127,14 +134,30 @@
                 self.bot_id == __value.bot_id and self.secret == __value.secret
             )
         return self.bot_id == __value
 
     def __hash__(self) -> int:
         return hash(self.bot_id)
 
+    def verify(
+        self,
+        sign: str,
+        body: str,
+    ) -> bool:
+        sign_ = base64.b64decode(sign)
+        sign_msg = urllib.parse.urlencode(
+            {"body": body, "secret": self.secret},
+        ).encode()
+        try:
+            rsa.verify(sign_msg, sign_, self.rsa_pub_key)
+        except rsa.VerificationError:
+            return False
+        else:
+            return True
+
     async def send(
         self,
         villa_id: int,
         room_id: int,
         chain: "MessageChain",
     ) -> str:
         """通用发送消息方法
```

### Comparing `herta_villa_sdk-0.5.1/hertavilla/event.py` & `herta_villa_sdk-0.6.0/hertavilla/event.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/exception.py` & `herta_villa_sdk-0.6.0/hertavilla/exception.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from __future__ import annotations
 
 from typing import Any
 
 
+class PubkeyNoneWarning(Warning):
+    ...
+
+
 class SDKException(Exception):
     ...
 
 
 class HTTPStatusError(SDKException):
     def __init__(
         self,
```

### Comparing `herta_villa_sdk-0.5.1/hertavilla/match.py` & `herta_villa_sdk-0.6.0/hertavilla/match.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/message/chain.py` & `herta_villa_sdk-0.6.0/hertavilla/message/chain.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/message/image.py` & `herta_villa_sdk-0.6.0/hertavilla/message/image.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/message/post.py` & `herta_villa_sdk-0.6.0/hertavilla/message/post.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/message/text.py` & `herta_villa_sdk-0.6.0/hertavilla/message/text.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/model.py` & `herta_villa_sdk-0.6.0/hertavilla/model.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/server/__init__.py` & `herta_villa_sdk-0.6.0/hertavilla/server/__init__.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/server/aiohttp.py` & `herta_villa_sdk-0.6.0/hertavilla/server/aiohttp.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,18 @@
     def run(
         self,
         *bots_: VillaBot,
         host: str | None = None,
         port: int | None = None,
     ):
         async def http_handle(request: web.Request):
-            resp = await self._run_handles(await request.json())
+            resp = await self._run_handles(
+                request.headers.get("x-rpc-bot_sign"),
+                (await request.text()).strip(),
+            )
             return web.json_response(
                 {"retcode": resp.retcode, "message": resp.message},
                 status=resp.status_code,
             )
 
         self._register_bots(
             bots_,
```

### Comparing `herta_villa_sdk-0.5.1/hertavilla/server/fastapi.py` & `herta_villa_sdk-0.6.0/hertavilla/server/fastapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,18 @@
     def run(
         self,
         *bots_: VillaBot,
         host: str | None = None,
         port: int | None = None,
     ):
         async def http_handle(request: Request) -> JSONResponse:
-            resp = await self._run_handles(await request.json())
+            resp = await self._run_handles(
+                request.headers.get("x-rpc-bot_sign"),
+                (await request.body()).decode().strip(),
+            )
             return JSONResponse(
                 {"retcode": resp.retcode, "message": resp.message},
                 status_code=resp.status_code,
             )
 
         self._register_bots(
             bots_,
```

### Comparing `herta_villa_sdk-0.5.1/hertavilla/server/internal.py` & `herta_villa_sdk-0.6.0/hertavilla/server/internal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import abc
 import asyncio
 from dataclasses import dataclass
+import json
 import logging
 from typing import Any, Callable, Sequence
 
 from hertavilla.bot import VillaBot
 from hertavilla.event import parse_event
 
 background_tasks = set()
@@ -15,14 +16,19 @@
 @dataclass
 class ResponseData:
     status_code: int = 200
     retcode: int = 0
     message: str = ""
 
 
+INVALID_EVENT = ResponseData(400, -1, "event body is invalid")
+VERIFY_FAILED = ResponseData(401, -2, "verify failed")
+NO_BOT = ResponseData(404, 1, "no bot with this id")
+
+
 class BaseBackend(abc.ABC):
     def __init__(self, host: str = "0.0.0.0", port: int = 8080, **kwargs: Any):
         self.host = host
         self.port = port
         self.backend_extra_config = kwargs
         self.bots: dict[str, VillaBot] = {}
         self.logger = logging.getLogger(
@@ -55,28 +61,34 @@
             self.bots[bot.bot_id] = bot
             endpoint = bot.callback_endpoint
             add_router_callback(endpoint)
             self.logger.info(
                 f"Register endpoint {endpoint} for bot {bot.bot_id}",
             )
 
-    async def _run_handles(self, payload: dict[str, Any]) -> ResponseData:
+    async def _run_handles(
+        self,
+        sign: str | None,
+        body: str,
+    ) -> ResponseData:
+        payload = json.loads(body)
         if not (event_payload := payload.get("event")):
-            # 当数据不符合结构时返回 400 Bad Request
-            # retcode: -1
-            # message: event body is invalid
             self.logger.warning("Event is invalid")
-            return ResponseData(400, -1, "event body is invalid")
+            return INVALID_EVENT
         try:
             event = parse_event(event_payload)
         except ValueError:
             self.logger.warning("Event is invalid")
-            return ResponseData(400, -1, "event body is invalid")
+            return INVALID_EVENT
 
         if bot := self.bots.get(event.robot.template.id):
+            if sign is None or not bot.verify(sign, body):
+                logging.warn("Event verify check is failed. Reject handling.")
+                return VERIFY_FAILED
+
             self.logger.info(
                 (
                     f"[RECV] {event.__class__.__name__} "
                     f"on bot {event.robot.template.name}"
                     f"({event.robot.template.id}) "
                     f"in villa {event.robot.villa_id}"
                 ),
@@ -86,8 +98,8 @@
             task = asyncio.create_task(bot.handle_event(event))
             background_tasks.add(task)
             task.add_done_callback(background_tasks.discard)
             return ResponseData()
         self.logger.warning(
             f"Received event but no bot with id {event.robot.template.id}",
         )
-        return ResponseData(404, 1, "no bot with this id")
+        return NO_BOT
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `herta_villa_sdk-0.5.1/hertavilla/typing.py` & `herta_villa_sdk-0.6.0/hertavilla/typing.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/hertavilla/utils.py` & `herta_villa_sdk-0.6.0/hertavilla/utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/pyproject.toml` & `herta_villa_sdk-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 description = "大别野「黑塔」Python SDK"
 authors = [
     { name = "MingxuanGame", email = "MingxuanGame@outlook.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.4",
     "pydantic>=1.10.8,<2.0",
+    "rsa>=4.9",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "mihoyo",
     "miyoushe",
     "bot",
     "villa",
 ]
 dynamic = []
-version = "0.5.1"
+version = "0.6.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/Herta-villa/Herta-villa-SDK"
 Documentation = "https://github.com/Herta-villa/Herta-villa-SDK"
@@ -80,14 +81,17 @@
     "ISC",
     "C4",
     "COM",
     "A",
     "B",
     "ASYNC",
 ]
+ignore = [
+    "PLR0913",
+]
 allowed-confusables = [
     "，",
     "。",
     "（",
     "）",
     "；",
 ]
```

### Comparing `herta_villa_sdk-0.5.1/tests/test_utils.py` & `herta_villa_sdk-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.1/PKG-INFO` & `herta_villa_sdk-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: herta-villa-sdk
-Version: 0.5.1
+Version: 0.6.0
 Summary: 大别野「黑塔」Python SDK
 Keywords: mihoyo miyoushe bot villa
 Author-Email: MingxuanGame <MingxuanGame@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Documentation, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Repository, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Bug tracker, https://github.com/Herta-villa/Herta-villa-SDK/issues
 Requires-Python: >=3.8
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: pydantic<2.0,>=1.10.8
+Requires-Dist: rsa>=4.9
 Requires-Dist: fastapi>=0.100.0; extra == "fastapi"
 Requires-Dist: uvicorn>=0.22.0; extra == "fastapi"
 Provides-Extra: fastapi
 Description-Content-Type: text/markdown
 
 # Herta-villa-SDK
 
@@ -47,18 +48,30 @@
 ## 快速开始
 
 你需要拥有一个[大别野](https://dby.miyoushe.com/chat)机器人。可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)（`OpenVilla`）申请。
 
 ```python
 from hertavilla import MessageChain, SendMessageEvent, VillaBot, run
 
+
+PUB_KEY = """-----BEGIN PUBLIC KEY-----
+aaa
+bbb
+ccc
+-----END PUBLIC KEY-----
+"""  # 开放平台 pub_key
+# 需要注意 `-----BEGIN PUBLIC KEY-----` 前没有换行符
+#  `-----END PUBLIC KEY-----` 后有一个换行符
+# 目前从网页端复制下来的时候会为一串 pub_key，需要将空格转为换行
+
 bot = VillaBot(
     "bot_id",  # 这里填写 bot_id
     "bot_secret",  # 这里填写 secret
     "/",  # bot 回调 endpoint
+    PUB_KEY,  # 开放平台提供的 pub_key
 )
 
 
 @bot.startswith("/")  # 注册一个消息匹配器，匹配前缀为 / 的消息
 async def _(event: SendMessageEvent, bot: VillaBot):
     message = event.message
     if str(message[1]) == "/hello":
```

