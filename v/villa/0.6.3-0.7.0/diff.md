# Comparing `tmp/villa-0.6.3.tar.gz` & `tmp/villa-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.6.3.tar", max compression
+gzip compressed data, was "villa-0.7.0.tar", max compression
```

## Comparing `villa-0.6.3.tar` & `villa-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-07-12 12:19:47.928516 villa-0.6.3/LICENSE
--rw-r--r--   0        0        0     3617 2023-07-12 12:19:47.928516 villa-0.6.3/README.md
--rw-r--r--   0        0        0     2127 2023-07-12 12:19:47.928516 villa-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      277 2023-07-12 12:19:47.928516 villa-0.6.3/villa/__init__.py
--rw-r--r--   0        0        0    37466 2023-07-12 12:19:47.928516 villa-0.6.3/villa/bot.py
--rw-r--r--   0        0        0    12215 2023-07-12 12:19:47.928516 villa-0.6.3/villa/event.py
--rw-r--r--   0        0        0      728 2023-07-12 12:19:47.928516 villa-0.6.3/villa/exception.py
--rw-r--r--   0        0        0     3337 2023-07-12 12:19:47.928516 villa-0.6.3/villa/handle.py
--rw-r--r--   0        0        0     1537 2023-07-12 12:19:47.928516 villa-0.6.3/villa/log.py
--rw-r--r--   0        0        0    21359 2023-07-12 12:19:47.932516 villa-0.6.3/villa/message.py
--rw-r--r--   0        0        0     9304 2023-07-12 12:19:47.932516 villa-0.6.3/villa/models.py
--rw-r--r--   0        0        0      935 2023-07-12 12:19:47.932516 villa-0.6.3/villa/store.py
--rw-r--r--   0        0        0      240 2023-07-12 12:19:47.932516 villa-0.6.3/villa/typing.py
--rw-r--r--   0        0        0      968 2023-07-12 12:19:47.932516 villa-0.6.3/villa/utils.py
--rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 villa-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-17 10:09:09.644517 villa-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3747 2023-07-17 10:09:09.644517 villa-0.7.0/README.md
+-rw-r--r--   0        0        0     2140 2023-07-17 10:09:09.644517 villa-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      277 2023-07-17 10:09:09.644517 villa-0.7.0/villa/__init__.py
+-rw-r--r--   0        0        0    40806 2023-07-17 10:09:09.644517 villa-0.7.0/villa/bot.py
+-rw-r--r--   0        0        0    12215 2023-07-17 10:09:09.644517 villa-0.7.0/villa/event.py
+-rw-r--r--   0        0        0     1835 2023-07-17 10:09:09.644517 villa-0.7.0/villa/exception.py
+-rw-r--r--   0        0        0     3337 2023-07-17 10:09:09.644517 villa-0.7.0/villa/handle.py
+-rw-r--r--   0        0        0     1537 2023-07-17 10:09:09.644517 villa-0.7.0/villa/log.py
+-rw-r--r--   0        0        0    21359 2023-07-17 10:09:09.644517 villa-0.7.0/villa/message.py
+-rw-r--r--   0        0        0     9304 2023-07-17 10:09:09.644517 villa-0.7.0/villa/models.py
+-rw-r--r--   0        0        0      935 2023-07-17 10:09:09.644517 villa-0.7.0/villa/store.py
+-rw-r--r--   0        0        0      240 2023-07-17 10:09:09.644517 villa-0.7.0/villa/typing.py
+-rw-r--r--   0        0        0      968 2023-07-17 10:09:09.644517 villa-0.7.0/villa/utils.py
+-rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 villa-0.7.0/PKG-INFO
```

### Comparing `villa-0.6.3/LICENSE` & `villa-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.6.3/README.md` & `villa-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -34,33 +34,38 @@
 
 - 使用 pip: `pip install villa`
 - 使用 poetry: `poetry add villa`
 - 使用 pdm: `pdm add villa`
 
 ## 快速开始
 
-你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的 Bot，可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)(ID: `OpenVilla`)申请，取得`bot_id`、`bot_secret`。
+你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的 Bot，可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)(ID: `OpenVilla`)申请，取得`bot_id`、`bot_secret`和`pub_key`。
 
 ```python
 from villa import Bot
 from villa.event import SendMessageEvent
 
-bot = Bot(bot_id="your_bot_id", bot_secret="your_bot_secret", callback_url="your_callback_url_endpoint")
-# 初始化Bot，填写你的bot_id、密钥以及回调地址endpoint
+bot = Bot(
+    bot_id="your_bot_id",
+    bot_secret="your_bot_secret",
+    pub_key="-----BEGIN PUBLIC KEY-----\nyour_pub_key\n-----END PUBLIC KEY-----\n",
+    callback_url="your_callback_url_endpoint",
+)
+# 初始化Bot，填写你的bot_id、密钥、pub_key以及回调地址endpoint
 # 举例：若申请时提供的回调地址为https://域名/callback，这里的callback_url就填`/callback`
 
 @bot.on_startswith("hello")
 async def handler(event: SendMessageEvent):
     await event.send("world!")
     # 一个简单的处理函数，向你的Bot发送包含`hello`关键词的消息，它将会回复你`world`！
 
 
 if __name__ == "__main__":
     bot.run(host="127.0.0.1", port=13350)
-    # 启动bot，注意，port端口号要和你的回调地址端口对上
+    # 启动bot，注意，port端口号要和你所使用的回调地址端口对上
 ```
 
 
 ## 示例
 
 详见 [example](https://github.com/CMHopeSunshine/villa-py/tree/main/example) 文件夹：
```

### Comparing `villa-0.6.3/pyproject.toml` & `villa-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.6.3"
+version = "0.7.0"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
@@ -12,14 +12,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = {extras = ["uvicorn"], version = "^0.96.0"}
 uvicorn = "^0.22.0"
 httpx = "^0.24.1"
 loguru = "^0.7.0"
+rsa = "^4.9"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.277"
 black = "^23.1.0"
 pre-commit = "^3.1.0"
```

### Comparing `villa-0.6.3/villa/bot.py` & `villa-0.7.0/villa/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 import asyncio
+import base64
 from collections import defaultdict
+import hashlib
+import hmac
 from itertools import product
 import re
 from typing import Any, DefaultDict, Dict, List, Literal, Optional, Set, Type, Union
-from urllib.parse import urlparse
+from urllib.parse import urlencode, urlparse
 
 from .event import Event, event_classes, pre_handle_event, SendMessageEvent
-from .exception import ActionFailed, StopPropagation
+from .exception import (
+    ActionFailed,
+    BotNotAdded,
+    InsufficientPermission,
+    InvalidBotAuthInfo,
+    InvalidMemberBotAccessToken,
+    InvalidRequest,
+    PermissionDenied,
+    StopPropagation,
+    UnknownServerError,
+    UnsupportedMsgType,
+)
 from .handle import EventHandler
 from .log import _log_patcher, logger
 from .message import (
     Image as ImageSegment,
     Link as LinkSegment,
     MentionAll as MentionAllSegment,
     MentionRobot as MentionRobotSegment,
@@ -21,19 +35,20 @@
     Text as TextSegment,
 )
 from .models import *
 from .store import get_app, get_bot, store_bot
 from .typing import T_Func, T_Handler
 from .utils import escape_tag
 
-from fastapi import BackgroundTasks, FastAPI
+from fastapi import BackgroundTasks, FastAPI, Request
 from fastapi.responses import JSONResponse
 import httpx
 from httpx._types import TimeoutTypes
 from pydantic import parse_obj_as
+import rsa
 import uvicorn
 
 
 class Bot:
     """Villa Bot"""
 
     _event_handlers: DefaultDict[int, List[EventHandler]] = defaultdict(list)
@@ -50,29 +65,44 @@
     _bot_info: Optional[Robot] = None
     """机器人信息"""
 
     def __init__(
         self,
         bot_id: str,
         bot_secret: str,
+        pub_key: Union[str, bytes],
         callback_url: Optional[str] = None,
         wait_util_complete: bool = False,
         api_timeout: TimeoutTypes = 10,
+        verify_event: bool = True,
     ):
         """初始化一个 Bot 实例
 
         参数:
             bot_id: 机器人 ID
             bot_secret: 机器人密钥
+            pub_key: 机器人 pub_key
             callback_url: 事件回调地址
+            wait_util_complete: 是否等待事件处理完成后响应
+            api_timeout: API 调用超时时间
+            verify_event: 是否对事件进行验证
         """
+        if isinstance(pub_key, str):
+            pub_key = pub_key.encode()
         self.bot_id = bot_id
         self.bot_secret = bot_secret
+        self.pub_key = rsa.PublicKey.load_pkcs1_openssl_pem(pub_key)
+        self.bot_secret_encrypt = hmac.new(
+            pub_key,
+            bot_secret.encode(),
+            hashlib.sha256,
+        ).hexdigest()
+        self.verify_event = verify_event
         if callback_url is not None:
-            self.callback_endpoint = urlparse(callback_url).path
+            self.callback_endpoint = urlparse(callback_url).path or "/"
         self.wait_util_complete = wait_util_complete
         self._client = httpx.AsyncClient(
             base_url="https://bbs-api.miyoushe.com/vila/api/bot/platform/",
             timeout=api_timeout,
         )
         store_bot(self)
 
@@ -855,26 +885,46 @@
                     "pass_through": pass_through,
                     "room_id": room_id,
                     "uid": uid,
                 },
             )
         )["audit_id"]
 
+    async def transfer_image(self, url: str) -> str:
+        """将非米游社的三方图床图片转存到米游社官方图床
+
+        参数:
+            url: 三方图床的图片链接
+
+        返回:
+            str: 新的米游社官方图床的图片链接
+        """
+        return (
+            await self._request(
+                "POST",
+                "transferImage",
+                None,
+                json={
+                    "url": url,
+                },
+            )
+        )["new_url"]
+
     def _get_headers(self, villa_id: Optional[int] = None) -> Dict[str, str]:
         """获取鉴权请求头
 
         参数:
             villa_id: 大别野 ID，部分无需
 
         返回:
             Dict[str, str]: 请求头
         """
         return {
             "x-rpc-bot_id": self.bot_id,
-            "x-rpc-bot_secret": self.bot_secret,
+            "x-rpc-bot_secret": self.bot_secret_encrypt,
             "x-rpc-bot_villa_id": str(villa_id) if villa_id else "",
         }
 
     async def _request(
         self,
         method: Literal["GET", "POST"],
         api: str,
@@ -907,18 +957,50 @@
                 headers=self._get_headers(villa_id),
                 json=json,
                 **kwargs,
             )
             resp = ApiResponse.parse_raw(resp.content)
             if resp.retcode == 0:
                 return resp.data
+            if resp.retcode == -502:
+                raise UnknownServerError(resp)
+            if resp.retcode == -1:
+                raise InvalidRequest(resp)
+            if resp.retcode == 10318001:
+                raise InsufficientPermission(resp)
+            if resp.retcode == 10322002:
+                raise BotNotAdded(resp)
+            if resp.retcode == 10322003:
+                raise PermissionDenied(resp)
+            if resp.retcode == 10322004:
+                raise InvalidMemberBotAccessToken(resp)
+            if resp.retcode == 10322005:
+                raise InvalidBotAuthInfo(resp)
+            if resp.retcode == 10322006:
+                raise UnsupportedMsgType(resp)
             raise ActionFailed(resp.retcode, resp)
         except Exception as e:
             raise e
 
+    def _verify_signature(
+        self,
+        body: str,
+        bot_sign: str,
+    ):
+        sign = base64.b64decode(bot_sign)
+        sign_data = urlencode(
+            {"body": body.rstrip("\n"), "secret": self.bot_secret},
+        ).encode()
+        try:
+            rsa.verify(sign_data, sign, self.pub_key)
+        except rsa.VerificationError as e:
+            logger.exception(e)
+            return False
+        return True
+
     async def _close_client(self) -> None:
         """关闭 HTTP Client"""
         await self._client.aclose()
 
     async def _handle_event(self, event: Event):
         """处理事件
 
@@ -959,17 +1041,19 @@
         post = message["post", 0]
 
         if images_msg := (message["image"] or None):  # type: ignore
             images_msg: List[ImageSegment]
             images = [
                 Image(
                     url=seg.url,
-                    size=ImageSize(width=seg.width, height=seg.height)
-                    if seg.width and seg.height
-                    else None,
+                    size=(
+                        ImageSize(width=seg.width, height=seg.height)
+                        if seg.width and seg.height
+                        else None
+                    ),
                     file_size=seg.file_size,
                 )
                 for seg in images_msg
             ]
         else:
             images = None
 
@@ -1077,24 +1161,24 @@
         if not (mentioned.type == MentionType.ALL and mentioned.user_id_list):
             mentioned = None
 
         if not (message_text or entities):
             if images:
                 if len(images) > 1:
                     content = TextMessageContent(
-                        text="\u200B",
+                        text="\u200b",
                         images=images,
                         preview_link=preview_link,
                         badge=badge,
                     )
                 else:
                     content = ImageMessageContent(**images[0].dict())
             elif preview_link:
                 content = TextMessageContent(
-                    text="\u200B",
+                    text="\u200b",
                     preview_link=preview_link,
                     badge=badge,
                 )
             elif post:
                 content = PostMessageContent(post_id=post.post_id)
             else:
                 raise ValueError("message content is empty")
@@ -1109,16 +1193,18 @@
 
         return MessageContentInfo(content=content, mentionedInfo=mentioned, quote=quote)
 
     def init_app(self, app: FastAPI):
         if self.callback_endpoint is not None:
             logger.opt(colors=True).info(f"Initializing Bot <m>{self.bot_id}</m>...")
             logger.opt(colors=True).debug(
-                f"With Secret: <m>{self.bot_secret}</m> "
-                f"and Callback Endpoint: <m>{self.callback_endpoint}</m>",
+                (
+                    f"With Secret: <m>{self.bot_secret}</m> "
+                    f"and Callback Endpoint: <m>{self.callback_endpoint}</m>"
+                ),
             )
             app.post(self.callback_endpoint, status_code=200)(handle_event)
             app.on_event("shutdown")(self._close_client)
         else:
             logger.opt(colors=True).warning(
                 f"Bot <m>{self.bot_id}</m> missing callback url endpoint.",
             )
@@ -1190,42 +1276,59 @@
         },
         **uvicorn_kwargs,
     )
 
 
 async def handle_event(
     data: Dict[str, Any],
+    request: Request,
     backgroud_tasks: BackgroundTasks,
+    # bot_sign: str = Header(..., alias="x-rpc-bot_sign"),
 ) -> JSONResponse:
     """处理事件"""
     if not (payload_data := data.get("event", None)):
         logger.warning(f"Received invalid data: {escape_tag(str(data))}")
         return JSONResponse(
-            status_code=400,
-            content={"retcode": -1, "msg": "Invalid data"},
+            status_code=415,
+            content={"retcode": 415, "msg": "Invalid data"},
         )
     try:
         event = parse_obj_as(event_classes, pre_handle_event(payload_data))
         if (bot := get_bot(event.bot_id)) is None:
             raise ValueError(f"Bot {event.bot_id} not found")
+        if (
+            bot.verify_event
+            and (bot_sign := request.headers.get("x-rpc-bot_sign")) is not None
+            and not bot._verify_signature((await request.body()).decode(), bot_sign)
+        ):
+            logger.opt(colors=True).warning(
+                (
+                    f"Bot <b><m>{bot.bot_id}</m></b> "
+                    f"received invalid signature: <b><m>{bot_sign}</m></b>"
+                ),
+            )
+            return JSONResponse(
+                status_code=401,
+                content={"retcode": 401, "msg": "Invalid signature"},
+            )
         bot._bot_info = event.robot
         logger.opt(colors=True).success(
             (
                 f"<b><m>{bot.bot_id}</m></b>"
                 f" | <b><y>[{event.__class__.__name__}]</y></b>: "
-                f"{event.get_event_description()}",
+                f"{event.get_event_description()}"
             ),
         )
     except Exception as e:
         logger.opt(exception=e).warning(
             f"Failed to parse payload {escape_tag(str(payload_data))}",
         )
         return JSONResponse(
-            status_code=400,
-            content={"retcode": -1, "msg": "Invalid data"},
+            status_code=415,
+            content={"retcode": 415, "msg": "Invalid data"},
         )
     else:
         if bot.wait_util_complete:
             await bot._handle_event(event=event)
         else:
             backgroud_tasks.add_task(bot._handle_event, event=event)
     return JSONResponse(status_code=200, content={"retcode": 0, "message": "success"})
```

### Comparing `villa-0.6.3/villa/event.py` & `villa-0.7.0/villa/event.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.3/villa/handle.py` & `villa-0.7.0/villa/handle.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.3/villa/log.py` & `villa-0.7.0/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.3/villa/message.py` & `villa-0.7.0/villa/message.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.3/villa/models.py` & `villa-0.7.0/villa/models.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.3/villa/store.py` & `villa-0.7.0/villa/store.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.3/villa/utils.py` & `villa-0.7.0/villa/utils.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.3/PKG-INFO` & `villa-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.6.3
+Version: 0.7.0
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi[uvicorn] (>=0.96.0,<0.97.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: rsa (>=4.9,<5.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Project-URL: Documentation, https://github.com/CMHopeSunshine/villa-py
 Project-URL: Repository, https://github.com/CMHopeSunshine/villa-py
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -58,33 +59,38 @@
 
 - 使用 pip: `pip install villa`
 - 使用 poetry: `poetry add villa`
 - 使用 pdm: `pdm add villa`
 
 ## 快速开始
 
-你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的 Bot，可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)(ID: `OpenVilla`)申请，取得`bot_id`、`bot_secret`。
+你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的 Bot，可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)(ID: `OpenVilla`)申请，取得`bot_id`、`bot_secret`和`pub_key`。
 
 ```python
 from villa import Bot
 from villa.event import SendMessageEvent
 
-bot = Bot(bot_id="your_bot_id", bot_secret="your_bot_secret", callback_url="your_callback_url_endpoint")
-# 初始化Bot，填写你的bot_id、密钥以及回调地址endpoint
+bot = Bot(
+    bot_id="your_bot_id",
+    bot_secret="your_bot_secret",
+    pub_key="-----BEGIN PUBLIC KEY-----\nyour_pub_key\n-----END PUBLIC KEY-----\n",
+    callback_url="your_callback_url_endpoint",
+)
+# 初始化Bot，填写你的bot_id、密钥、pub_key以及回调地址endpoint
 # 举例：若申请时提供的回调地址为https://域名/callback，这里的callback_url就填`/callback`
 
 @bot.on_startswith("hello")
 async def handler(event: SendMessageEvent):
     await event.send("world!")
     # 一个简单的处理函数，向你的Bot发送包含`hello`关键词的消息，它将会回复你`world`！
 
 
 if __name__ == "__main__":
     bot.run(host="127.0.0.1", port=13350)
-    # 启动bot，注意，port端口号要和你的回调地址端口对上
+    # 启动bot，注意，port端口号要和你所使用的回调地址端口对上
 ```
 
 
 ## 示例
 
 详见 [example](https://github.com/CMHopeSunshine/villa-py/tree/main/example) 文件夹：
```

