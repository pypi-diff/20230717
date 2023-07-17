# Comparing `tmp/nonebot_adapter_villa-0.5.6.tar.gz` & `tmp/nonebot_adapter_villa-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.5.6.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.6.0.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.5.6.tar` & `nonebot_adapter_villa-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/LICENSE
--rw-r--r--   0        0        0     6796 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/README.md
--rw-r--r--   0        0        0      235 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    10977 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0       25 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0     2911 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/client.pyi
--rw-r--r--   0        0        0    12460 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9443 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    13338 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      649 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    11651 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0    10115 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0     1435 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/permission.py
--rw-r--r--   0        0        0       76 2023-07-13 15:07:19.857204 nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-07-13 15:07:19.861204 nonebot_adapter_villa-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7323 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/README.md
+-rw-r--r--   0        0        0      228 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    12154 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0     3293 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/client.pyi
+-rw-r--r--   0        0        0    13152 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9488 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1734 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    14561 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      713 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    11808 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     2717 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     9952 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0     1449 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/permission.py
+-rw-r--r--   0        0        0       76 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     2125 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8249 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.6.0/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.5.6/LICENSE` & `nonebot_adapter_villa-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.6/README.md` & `nonebot_adapter_villa-0.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
 <a href="https://pypi.python.org/pypi/nonebot-adapter-villa">
   <img src="https://img.shields.io/pypi/dm/nonebot-adapter-villa" alt="pypi download">
 </a>
 <a href="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/838e7f55-f8b8-49ff-aec0-29ad264931cf">
   <img src="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/838e7f55-f8b8-49ff-aec0-29ad264931cf.svg" alt="wakatime">
 </a>
+<a href="https://github.com/astral-sh/ruff">
+  <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="ruff">
+</a>
 
 </div>
 
 ## 安装
 
 在`nb create`创建项目时选择`Villa`适配器
 
@@ -44,42 +47,50 @@
 
 ```dotenv
 DRIVER=~fastapi+~httpx
 ```
 
 ### VILLA_BOTS
 
-配置 Bot 帐号列表，每个bot有3个必填配置，可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)(ID: `OpenVilla`)申请，取得以下配置：
+配置 Bot 帐号列表，每个bot有4个必填配置，可前往[「大别野开放平台」](https://open.miyoushe.com/#/login)(ID: `OpenVilla`)申请，取得以下配置：
 
 - `bot_id`: 机器人id，以`bot_`开头
 - `bot_secret`: 机器人密钥
+- `pub_key`: 加密和验证所需的pub_key
 - `callback_url`: http回调地址 endpoint，例如申请bot时给的回调地址是`http://域名/your/callback/url`，那么配置里的`callback_url`填写`/your/callback/url`
 
+此外还有以下选填配置：
+
+- `verify_event`：是否对回调事件签名进行验证
+
 例如：
 
 ```dotenv
 VILLA_BOTS='
 [
   {
     "bot_id": "bot_123456789",
     "bot_secret": "abc123def456",
-    "callback_url": "/your/callback/url"
+    "pub_key": "-----BEGIN PUBLIC KEY-----\nyour_pub_key\n-----END PUBLIC KEY-----\n",
+    "callback_url": "/your/callback/url",
+    "verify_event": true
   }
 ]
 '
 ```
 
-> 注意，当前大别野只能接收到有@Bot(在哪个位置皆可)的消息事件，且不能有多个@(即使是@两次Bot都不行)
-
 ## 已支持消息段
 
+> 注意，当前大别野只能接收到有@Bot(在哪个位置皆可)的消息事件，且不能有多个@(即使是@两次Bot都不行)
+
 - `MessageSegment.text`: 纯文本
   + 米游社自带表情也是用text来发送，以[表情名]格式，例如MessageSegment.text("[爱心]")
 - `MessageSegment.mention_robot`: @机器人
 - `MessageSegment.mention_user`: @用户
+  + `user_name`和`villa_id`必须给出其中之一，给`villa_id`时，调用api来获取用户名
 - `MessageSegment.mention_all`: @全体成员
 - `MessageSegment.room_link`: #房间跳转链接
 - `MessageSegment.link`: 超链接
   + 使用link的话链接能够点击进行跳转，使用text的话不能点击
   + 字段`show_text`是指链接显示的文字，但若指定了该字段，Web端大别野会无法正常跳转
   + 字段`requires_bot_access_token`为true时，跳转链接会带上含有用户信息的token
 - `MessageSegment.quote`: 引用(回复)消息
@@ -166,13 +177,13 @@
 使用命令`@bot /test 纯文本`时，bot会回复`这是一段纯文本`
 
 
 ## 交流、建议和反馈
 
 大别野 Bot 和本适配器均为开发测试中，如遇问题请提出 [issue](https://github.com/CMHopeSunshine/nonebot-adapter-villa/issues) ，感谢支持！
 
-也欢迎来我的大别野[「尘世闲游」]((https://dby.miyoushe.com/chat/1047/21652))(ID: `wgiJNaU`)进行交流~ 
+也欢迎来我的大别野[「尘世闲游」]((https://dby.miyoushe.com/chat/1047/21652))(ID: `wgiJNaU`)进行交流~
 
 ## 相关项目
 
 - [NoneBot2](https://github.com/nonebot/nonebot2): 非常好用的Python跨平台机器人框架！
-- [villa-py](https://github.com/CMHopeSunshine/villa-py): 大别野 Bot Python SDK。
+- [villa-py](https://github.com/CMHopeSunshine/villa-py): 大别野 Bot Python SDK。
```

#### html2text {}

```diff
@@ -1,35 +1,40 @@
                             [nonebot-adapter-villa]
  # NoneBot-Adapter-Villa _â¨ å¤§å«é åè®®éé â¨_ [license] [version]
-                      [python] [pypi_download] [wakatime]
+                  [python] [pypi_download] [wakatime] [ruff]
 ## å®è£ å¨`nb create`åå»ºé¡¹ç®æ¶éæ©`Villa`ééå¨
 æå¨ç°æ`NoneBot2`é¡¹ç®ç®å½ä¸ä½¿ç¨èææ¶å®è£ï¼ ``` nb adapter
 install nonebot-adapter-villa ``` ## éç½® ä¿®æ¹ NoneBot éç½®æä»¶ `.env`
 æè `.env.*`ã ### Driver
 æ¬ééå¨åæ¶éè¦`ReverseDriver`å`ForwardDriver`ï¼åè [driver]
 (https://v2.nonebot.dev/docs/next/advanced/
 driver#%E9%A9%B1%E5%8A%A8%E5%99%A8%E7%B1%BB%E5%9E%8B) éç½®é¡¹ã ä¾å¦ï¼
 ```dotenv DRIVER=~fastapi+~httpx ``` ### VILLA_BOTS éç½® Bot
-å¸å·åè¡¨ï¼æ¯ä¸ªbotæ3ä¸ªå¿å¡«éç½®ï¼å¯åå¾å¤§å«é
-[ãæºå¨äººå¼åèç¤¾åºã](https://dby.miyoushe.com/chat/463/20020)(ID:
+å¸å·åè¡¨ï¼æ¯ä¸ªbotæ4ä¸ªå¿å¡«éç½®ï¼å¯åå¾
+[ãå¤§å«éå¼æ¾å¹³å°ã](https://open.miyoushe.com/#/login)(ID:
 `OpenVilla`)ç³è¯·ï¼åå¾ä»¥ä¸éç½®ï¼ - `bot_id`:
-æºå¨äººidï¼ä»¥`bot_`å¼å¤´ - `bot_secret`: æºå¨äººå¯é¥ - `callback_url`:
-httpåè°å°å endpointï¼ä¾å¦ç³è¯·botæ¶ç»çåè°å°åæ¯`http://
-åå/your/callback/url`ï¼é£ä¹éç½®éç`callback_url`å¡«å`/your/
-callback/url` ä¾å¦ï¼ ```dotenv VILLA_BOTS=' [ { "bot_id": "bot_123456789",
-"bot_secret": "abc123def456", "callback_url": "/your/callback/url" } ] ' ``` >
-æ³¨æï¼å½åå¤§å«éåªè½æ¥æ¶å°æ@Bot
+æºå¨äººidï¼ä»¥`bot_`å¼å¤´ - `bot_secret`: æºå¨äººå¯é¥ - `pub_key`:
+å å¯åéªè¯æéçpub_key - `callback_url`: httpåè°å°å
+endpointï¼ä¾å¦ç³è¯·botæ¶ç»çåè°å°åæ¯`http://åå/your/callback/
+url`ï¼é£ä¹éç½®éç`callback_url`å¡«å`/your/callback/url`
+æ­¤å¤è¿æä»¥ä¸éå¡«éç½®ï¼ -
+`verify_event`ï¼æ¯å¦å¯¹åè°äºä»¶ç­¾åè¿è¡éªè¯ ä¾å¦ï¼ ```dotenv
+VILLA_BOTS=' [ { "bot_id": "bot_123456789", "bot_secret": "abc123def456",
+"pub_key": "-----BEGIN PUBLIC KEY-----\nyour_pub_key\n-----END PUBLIC KEY-----
+\n", "callback_url": "/your/callback/url", "verify_event": true } ] ' ``` ##
+å·²æ¯ææ¶æ¯æ®µ > æ³¨æï¼å½åå¤§å«éåªè½æ¥æ¶å°æ@Bot
 (å¨åªä¸ªä½ç½®çå¯)çæ¶æ¯äºä»¶ï¼ä¸ä¸è½æå¤ä¸ª@
-(å³ä½¿æ¯@ä¸¤æ¬¡Boté½ä¸è¡) ## å·²æ¯ææ¶æ¯æ®µ - `MessageSegment.text`:
-çº¯ææ¬ + ç±³æ¸¸ç¤¾èªå¸¦è¡¨æä¹æ¯ç¨textæ¥åéï¼ä»¥
+(å³ä½¿æ¯@ä¸¤æ¬¡Boté½ä¸è¡) - `MessageSegment.text`: çº¯ææ¬ +
+ç±³æ¸¸ç¤¾èªå¸¦è¡¨æä¹æ¯ç¨textæ¥åéï¼ä»¥
 [è¡¨æå]æ ¼å¼ï¼ä¾å¦MessageSegment.text("[ç±å¿]") -
 `MessageSegment.mention_robot`: @æºå¨äºº - `MessageSegment.mention_user`:
-@ç¨æ· - `MessageSegment.mention_all`: @å¨ä½æå -
-`MessageSegment.room_link`: #æ¿é´è·³è½¬é¾æ¥ - `MessageSegment.link`:
-è¶é¾æ¥ +
+@ç¨æ· +
+`user_name`å`villa_id`å¿é¡»ç»åºå¶ä¸­ä¹ä¸ï¼ç»`villa_id`æ¶ï¼è°ç¨apiæ¥è·åç¨æ·å
+- `MessageSegment.mention_all`: @å¨ä½æå - `MessageSegment.room_link`:
+#æ¿é´è·³è½¬é¾æ¥ - `MessageSegment.link`: è¶é¾æ¥ +
 ä½¿ç¨linkçè¯é¾æ¥è½å¤ç¹å»è¿è¡è·³è½¬ï¼ä½¿ç¨textçè¯ä¸è½ç¹å» +
 å­æ®µ`show_text`æ¯æé¾æ¥æ¾ç¤ºçæå­ï¼ä½è¥æå®äºè¯¥å­æ®µï¼Webç«¯å¤§å«éä¼æ æ³æ­£å¸¸è·³è½¬
 +
 å­æ®µ`requires_bot_access_token`ä¸ºtrueæ¶ï¼è·³è½¬é¾æ¥ä¼å¸¦ä¸å«æç¨æ·ä¿¡æ¯çtoken
 - `MessageSegment.quote`: å¼ç¨(åå¤)æ¶æ¯ +
 ä¸è½**åç¬**ä½¿ç¨ï¼è¦ä¸å¶ä»æ¶æ¯æ®µä¸èµ·ä½¿ç¨ -
 `MessageSegment.image`: URLå¾ç + ææ¶åªæ¯æurlå¾ç +
```

### Comparing `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,69 @@
-import json
 import asyncio
+import json
 from typing import Any, List, Optional, cast
+from typing_extensions import override
 
-from pydantic import parse_obj_as
-from nonebot.typing import overrides
-from nonebot.utils import escape_tag
-from nonebot.exception import WebSocketClosed
+from nonebot.adapters import Adapter as BaseAdapter
 from nonebot.drivers import (
     URL,
     Driver,
+    ForwardDriver,
+    HTTPServerSetup,
     Request,
     Response,
-    ForwardDriver,
     ReverseDriver,
-    HTTPServerSetup,
 )
+from nonebot.exception import WebSocketClosed
+from nonebot.utils import escape_tag
 
-from nonebot.adapters import Adapter as BaseAdapter
+from pydantic import parse_obj_as
 
+from .api import API_HANDLERS
 from .bot import Bot
-from .utils import log
 from .config import Config
-from .api import API_HANDLERS
-from .exception import ApiNotAvailable
 from .event import event_classes, pre_handle_event
+from .exception import ApiNotAvailable
+from .utils import log
 
 
 class Adapter(BaseAdapter):
-    @overrides(BaseAdapter)
+    @override
     def __init__(self, driver: Driver, **kwargs: Any):
         super().__init__(driver, **kwargs)
         self.villa_config: Config = Config(**self.config.dict())
         self.tasks: List[asyncio.Task] = []
         self.base_url: URL = URL("https://bbs-api.miyoushe.com")
         self._setup()
 
     @classmethod
-    @overrides(BaseAdapter)
+    @override
     def get_name(cls) -> str:
         return "大别野"
 
     def _setup(self):
         # ReverseDriver用于接收回调事件，ForwardDriver用于调用API
         if not (
             isinstance(self.driver, ReverseDriver)
             and isinstance(self.driver, ForwardDriver)
         ):
             raise RuntimeError(
-                f"Current driver {self.config.driver} doesn't support connections!"
-                "Villa Adapter need a ReverseDriver and ForwardDriver to work."
+                (
+                    f"Current driver {self.config.driver} doesn't support connections!"
+                    "Villa Adapter need a ReverseDriver and ForwardDriver to work."
+                ),
             )
         self.driver.on_startup(self._forward_http)
         self.driver.on_startup(self._start_forward)
         self.driver.on_shutdown(self._stop_forward)
 
     async def _forward_http(self):
         for bot_info in self.villa_config.villa_bots:
             if bot_info.callback_url:
-                bot = Bot(self, bot_info.bot_id, bot_info.bot_secret)
+                bot = Bot(self, bot_info)
                 self.bot_connect(bot)
                 log("INFO", f"<y>Bot {bot.self_id} connected</y>")
                 http_setup = HTTPServerSetup(
                     URL(bot_info.callback_url),
                     "POST",
                     f"大别野 {bot_info.bot_id} HTTP",
                     self._handle_http,
@@ -73,64 +75,79 @@
             json_data = json.loads(data)
             if payload_data := json_data.get("event"):
                 try:
                     event = parse_obj_as(event_classes, pre_handle_event(payload_data))
                     bot_id = event.bot_id
                     if (bot := self.bots.get(bot_id, None)) is None:
                         if (
-                            bot_secret := next(
+                            bot_info := next(
                                 (
-                                    bot.bot_secret
+                                    bot
                                     for bot in self.villa_config.villa_bots
                                     if bot.bot_id == bot_id
                                 ),
                                 None,
                             )
                         ) is not None:
-                            bot = Bot(self, bot_id, bot_secret)
+                            bot = Bot(
+                                self,
+                                bot_info,
+                            )
                             self.bot_connect(bot)
                             log("INFO", f"<y>Bot {bot.self_id} connected</y>")
                         else:
                             log(
                                 "WARNING",
-                                f"<r>Missing bot secret for bot {bot_id}</r>, event will not be handle",
+                                (
+                                    f"<r>Missing bot secret for bot {bot_id}</r>, "
+                                    "event will not be handle"
+                                ),
                             )
                             return Response(
                                 200,
                                 content=json.dumps(
-                                    {"retcode": 0, "message": "NoneBot2 Get it!"}
+                                    {"retcode": 0, "message": "NoneBot2 Get it!"},
                                 ),
                             )
                     bot = cast(Bot, bot)
+                    if bot.verify_event and (
+                        (bot_sign := request.headers.get("x-rpc-bot_sign")) is None
+                        or not bot._verify_signature(
+                            data.decode() if isinstance(data, bytes) else data,
+                            bot_sign,
+                        )
+                    ):
+                        log("WARNING", f"Received invalid signature {bot_sign}.")
+                        return Response(401, content="Invalid Signature")
                     bot._bot_info = event.robot
                 except Exception as e:
                     log(
                         "WARNING",
                         f"Failed to parse event {escape_tag(str(payload_data))}",
                         e,
                     )
                 else:
                     asyncio.create_task(bot.handle_event(event))
                 return Response(
                     200,
                     content=json.dumps({"retcode": 0, "message": "NoneBot2 Get it!"}),
                 )
-            return Response(400, content="Invalid Request Body")
-        return Response(400, content="Invalid Request Body")
+            return Response(415, content="Invalid Request Body")
+        return Response(415, content="Invalid Request Body")
 
     async def _start_forward(self) -> None:
         for bot_info in self.villa_config.villa_bots:
             if bot_info.ws_url:
-                bot = Bot(self, bot_info.bot_id, bot_info.bot_secret)
+                bot = Bot(self, bot_info)
                 self.bot_connect(bot)
                 log("INFO", f"<y>Bot {bot.self_id} connected</y>")
                 self.tasks.append(
                     asyncio.create_task(
-                        self._forward_ws(URL(bot_info.ws_url), bot_info.ws_secret)
-                    )
+                        self._forward_ws(URL(bot_info.ws_url), bot_info.ws_secret),
+                    ),
                 )
 
     async def _forward_ws(self, url: URL, secret: Optional[str] = None):
         if secret is not None:
             request = Request("GET", url, headers={"ws-secret": secret}, timeout=30)
         else:
             request = Request("GET", url, timeout=30)
@@ -145,105 +162,118 @@
                     try:
                         while True:
                             data = await ws.receive()
                             json_data = json.loads(data)
                             if payload_data := json_data.get("event"):
                                 try:
                                     event = parse_obj_as(
-                                        event_classes, pre_handle_event(payload_data)
+                                        event_classes,
+                                        pre_handle_event(payload_data),
                                     )
                                     bot_id = event.bot_id
-                                    if (bot := self.bots.get(bot_id, None)) is None:  # type: ignore
+                                    if (bot := self.bots.get(bot_id, None)) is None:  # type: ignore  # noqa: E501
                                         if (
-                                            bot_secret := next(
+                                            bot_info := next(
                                                 (
-                                                    bot.bot_secret
-                                                    for bot in self.villa_config.villa_bots
+                                                    bot
+                                                    for bot in self.villa_config.villa_bots  # noqa: E501
                                                     if bot.bot_id == bot_id
                                                 ),
                                                 None,
                                             )
                                         ) is not None:
                                             bot = Bot(
                                                 self,
-                                                bot_id,
-                                                bot_secret=bot_secret,
+                                                bot_info,
                                             )
                                             self.bot_connect(bot)
                                             log(
                                                 "INFO",
                                                 f"<y>Bot {bot.self_id} connected</y>",
                                             )
                                         else:
                                             log(
                                                 "WARNING",
-                                                f"<r>Missing bot secret for bot {bot_id}</r>, event will not be handle",
+                                                (
+                                                    "<r>Missing bot secret for bot"
+                                                    f" {bot_id}</r>, event won't be"
+                                                    " handle"
+                                                ),
                                             )
                                             await ws.send(
                                                 json.dumps(
                                                     {
                                                         "retcode": 0,
                                                         "message": "NoneBot2 Get it!",
-                                                    }
-                                                )
+                                                    },
+                                                ),
                                             )
                                     bot = cast(Bot, bot)
                                     bot._bot_info = event.robot
                                 except Exception as e:
                                     log(
                                         "WARNING",
-                                        f"Failed to parse event {escape_tag(str(payload_data))}",
+                                        (
+                                            "Failed to parse event "
+                                            f"{escape_tag(str(payload_data))}"
+                                        ),
                                         e,
                                     )
                                 else:
                                     asyncio.create_task(bot.handle_event(event))
                                 await ws.send(
                                     json.dumps(
-                                        {"retcode": 0, "message": "NoneBot2 Get it!"}
-                                    )
+                                        {"retcode": 0, "message": "NoneBot2 Get it!"},
+                                    ),
                                 )
                             else:
                                 await ws.send(
                                     json.dumps(
                                         {
                                             "retcode": -100,
                                             "message": "Invalid Request Body",
-                                        }
-                                    )
+                                        },
+                                    ),
                                 )
                     except WebSocketClosed as e:
                         log(
                             "ERROR",
                             "<r><bg #f8bbd0>WebSocket Closed</bg #f8bbd0></r>",
                             e,
                         )
                     except Exception as e:
                         log(
                             "ERROR",
-                            "<r><bg #f8bbd0>Error while process data from websocket "
-                            f"{escape_tag(str(url))}. Trying to reconnect...</bg #f8bbd0></r>",
+                            (  # noqa: E501
+                                "<r><bg #f8bbd0>Error while process data from"
+                                f" websocket {escape_tag(str(url))}. Trying to"
+                                " reconnect...</bg #f8bbd0></r>"
+                            ),
                             e,
                         )
                     finally:
                         if bot:
                             self.bot_disconnect(bot)
             except Exception as e:
                 log(
                     "ERROR",
-                    "<r><bg #f8bbd0>Error while setup websocket to "
-                    f"{escape_tag(str(url))}. Trying to reconnect...</bg #f8bbd0></r>",
+                    (
+                        "<r><bg #f8bbd0>Error while setup websocket to"
+                        f" {escape_tag(str(url))}. Trying to reconnect...</bg"
+                        " #f8bbd0></r>"
+                    ),
                     e,
                 )
                 await asyncio.sleep(3.0)
 
     async def _stop_forward(self) -> None:
         for task in self.tasks:
             if not task.done():
                 task.cancel()
 
-    @overrides(BaseAdapter)
+    @override
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> Any:
         log("DEBUG", f"Calling API <y>{api}</y>")
         log("TRACE", f"With Data <y>{escape_tag(str(data))}</y>")
         if (api_handler := API_HANDLERS.get(api)) is None:
             raise ApiNotAvailable(api)
         return await api_handler(self, bot, **data)
```

### Comparing `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/client.pyi` & `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,123 @@
-from typing import List, Union
-
 from .models import *
 
 class ApiClient:
     async def check_member_bot_access_token(
-        self, *, villa_id: int, token: str
+        self,
+        *,
+        villa_id: int,
+        token: str,
     ) -> CheckMemberBotAccessTokenReturn: ...
     async def get_villa(self, *, villa_id: int) -> Villa: ...
-    async def get_member(self, *, uid: int) -> Member: ...
+    async def get_member(self, *, villa_id: int, uid: int) -> Member: ...
     async def get_villa_members(
-        self, *, villa_id: int, offset: int, size: int
+        self,
+        *,
+        villa_id: int,
+        offset: int,
+        size: int,
     ) -> MemberListReturn: ...
     async def delete_villa_member(self, *, villa_id: int, uid: int) -> None: ...
     async def pin_message(
         self,
         *,
         villa_id: int,
         msg_uid: str,
         is_cancel: bool,
         room_id: int,
         send_at: int,
     ) -> None: ...
     async def recall_message(
-        self, *, villa_id: int, msg_uid: str, room_id: int, msg_time: int
+        self,
+        *,
+        villa_id: int,
+        msg_uid: str,
+        room_id: int,
+        msg_time: int,
     ) -> None: ...
     async def send_message(
         self,
         *,
         villa_id: int,
         room_id: int,
         object_name: str,
-        msg_content: Union[str, MessageContentInfo],
+        msg_content: str | MessageContentInfo,
     ) -> str: ...
     async def create_group(self, *, villa_id: int, group_name: str) -> int: ...
     async def edit_group(
-        self, *, villa_id: int, group_id: int, group_name: str
+        self,
+        *,
+        villa_id: int,
+        group_id: int,
+        group_name: str,
     ) -> None: ...
     async def delete_group(self, *, villa_id: int, group_id: int) -> None: ...
-    async def get_group_list(self, *, villa_id: int) -> List[Group]: ...
-    async def sort_group_list(self, *, villa_id: int, group_ids: List[int]) -> None: ...
+    async def get_group_list(self, *, villa_id: int) -> list[Group]: ...
+    async def sort_group_list(self, *, villa_id: int, group_ids: list[int]) -> None: ...
     async def edit_room(
-        self, *, villa_id: int, room_id: int, room_name: str
+        self,
+        *,
+        villa_id: int,
+        room_id: int,
+        room_name: str,
     ) -> None: ...
     async def delete_room(self, *, villa_id: int, room_id: int) -> None: ...
     async def get_room(self, *, villa_id: int, room_id: int) -> Room: ...
-    async def get_villa_group_room_list(self, *, villa_id: int) -> List[GroupRoom]: ...
+    async def get_villa_group_room_list(self, *, villa_id: int) -> list[GroupRoom]: ...
     async def sort_room_list(
-        self, *, villa_id: int, room_list: List[RoomSort]
+        self,
+        *,
+        villa_id: int,
+        room_list: list[RoomSort],
     ) -> None: ...
     async def operate_member_to_role(
-        self, *, villa_id: int, role_id: int, uid: int, is_add: bool
+        self,
+        *,
+        villa_id: int,
+        role_id: int,
+        uid: int,
+        is_add: bool,
     ) -> None: ...
     async def create_member_role(
-        self, *, villa_id: int, name: str, color: str, permissions: List[Permission]
+        self,
+        *,
+        villa_id: int,
+        name: str,
+        color: str,
+        permissions: list[Permission],
     ) -> int: ...
     async def edit_member_role(
         self,
         *,
         villa_id: int,
         role_id: int,
         name: str,
         color: str,
-        permissions: List[Permission],
+        permissions: list[Permission],
     ) -> None: ...
     async def delete_member_role(self, *, villa_id: int, role_id: int) -> None: ...
     async def get_member_role(
-        self, *, villa_id: int, role_id: int
+        self,
+        *,
+        villa_id: int,
+        role_id: int,
     ) -> MemberRoleDetail: ...
     async def get_villa_member_roles(
-        self, *, villa_id: int
-    ) -> List[MemberRoleDetail]: ...
-    async def get_all_emoticon(self) -> List[Emoticon]: ...
+        self,
+        *,
+        villa_id: int,
+    ) -> list[MemberRoleDetail]: ...
+    async def get_all_emoticon(self) -> list[Emoticon]: ...
     async def audit(
         self,
         *,
         villa_id: int,
         audit_content: str,
         pass_through: str,
         room_id: int,
         uid: int,
     ) -> str: ...
+    async def transfer_image(
+        self,
+        *,
+        url: str,
+    ) -> str: ...
```

### Comparing `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/handle.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,86 @@
-from typing import TYPE_CHECKING, List, Union
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, Dict, List, Union
 
-from pydantic import parse_obj_as
 from nonebot.drivers import Request
 
+from pydantic import parse_obj_as
+
 from .models import *
 from .request import _request
 
 if TYPE_CHECKING:
-    from ..bot import Bot
     from ..adapter import Adapter
+    from ..bot import Bot
 
 
 async def _check_member_bot_access_token(
-    adapter: "Adapter", bot: "Bot", villa_id: int, token: str
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    token: str,
 ) -> CheckMemberBotAccessTokenReturn:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/checkMemberBotAccessToken",
         headers=bot.get_authorization_header(
-            villa_id
-        ),  # TODO: 文档中说无需鉴权，但不带header会报错，有待确认
+            villa_id,
+        ),
         json={"token": token},
     )
     return parse_obj_as(
-        CheckMemberBotAccessTokenReturn, await _request(adapter, bot, request)
+        CheckMemberBotAccessTokenReturn,
+        await _request(adapter, bot, request),
     )
 
 
 async def _get_villa(adapter: "Adapter", bot: "Bot", villa_id: int) -> Villa:
     request = Request(
         method="GET",
         url=adapter.base_url / "vila/api/bot/platform/getVilla",
         headers=bot.get_authorization_header(villa_id),
     )
     return parse_obj_as(Villa, (await _request(adapter, bot, request))["villa"])
 
 
 async def _get_member(
-    adapter: "Adapter", bot: "Bot", villa_id: int, uid: int
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    uid: int,
 ) -> Member:
     request = Request(
         method="GET",
         url=adapter.base_url / "vila/api/bot/platform/getMember",
         headers=bot.get_authorization_header(villa_id),
         json={"uid": uid},
     )
     return parse_obj_as(Member, (await _request(adapter, bot, request))["member"])
 
 
 async def _get_villa_members(
-    adapter: "Adapter", bot: "Bot", villa_id: int, offset: int, size: int
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    offset: int,
+    size: int,
 ) -> MemberListReturn:
     request = Request(
         method="GET",
         url=adapter.base_url / "vila/api/bot/platform/getVillaMembers",
         headers=bot.get_authorization_header(villa_id),
         json={"offset": offset, "size": size},
     )
     return parse_obj_as(MemberListReturn, await _request(adapter, bot, request))
 
 
 async def _delete_villa_member(
-    adapter: "Adapter", bot: "Bot", villa_id: int, uid: int
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    uid: int,
 ) -> None:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/deleteVillaMember",
         headers=bot.get_authorization_header(villa_id),
         json={"uid": uid},
     )
@@ -130,39 +145,49 @@
         headers=bot.get_authorization_header(villa_id),
         json={"room_id": room_id, "object_name": object_name, "msg_content": content},
     )
     return (await _request(adapter, bot, request))["bot_msg_id"]
 
 
 async def _create_group(
-    adapter: "Adapter", bot: "Bot", villa_id: int, group_name: str
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    group_name: str,
 ) -> int:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/createGroup",
         headers=bot.get_authorization_header(villa_id),
         json={"group_name": group_name},
     )
     return (await _request(adapter, bot, request))["group_id"]
 
 
 async def _edit_group(
-    adapter: "Adapter", bot: "Bot", villa_id: int, group_id: int, group_name: str
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    group_id: int,
+    group_name: str,
 ) -> None:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/editGroup",
         headers=bot.get_authorization_header(villa_id),
         json={"group_id": group_id, "group_name": group_name},
     )
     await _request(adapter, bot, request)
 
 
 async def _delete_group(
-    adapter: "Adapter", bot: "Bot", villa_id: int, group_id: int
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    group_id: int,
 ) -> None:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/deleteGroup",
         headers=bot.get_authorization_header(villa_id),
         json={"group_id": group_id},
     )
@@ -175,88 +200,112 @@
         url=adapter.base_url / "vila/api/bot/platform/getGroupList",
         headers=bot.get_authorization_header(villa_id),
     )
     return parse_obj_as(List[Group], (await _request(adapter, bot, request))["list"])
 
 
 async def _sort_group_list(
-    adapter: "Adapter", bot: "Bot", villa_id: int, group_ids: List[int]
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    group_ids: List[int],
 ) -> None:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/sortGroupList",
         headers=bot.get_authorization_header(villa_id),
         json={"villa_id": villa_id, "group_ids": group_ids},
     )
     await _request(adapter, bot, request)
 
 
 async def _edit_room(
-    adapter: "Adapter", bot: "Bot", villa_id: int, room_id: int, room_name: str
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    room_id: int,
+    room_name: str,
 ) -> None:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/editRoom",
         headers=bot.get_authorization_header(villa_id),
         json={"room_id": room_id, "room_name": room_name},
     )
     await _request(adapter, bot, request)
 
 
 async def _delete_room(
-    adapter: "Adapter", bot: "Bot", villa_id: int, room_id: int
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    room_id: int,
 ) -> None:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/deleteRoom",
         headers=bot.get_authorization_header(villa_id),
         json={"room_id": room_id},
     )
     await _request(adapter, bot, request)
 
 
 async def _get_room(
-    adapter: "Adapter", bot: "Bot", villa_id: int, room_id: int
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    room_id: int,
 ) -> Room:
     request = Request(
         method="GET",
         url=adapter.base_url / "vila/api/bot/platform/getRoom",
         headers=bot.get_authorization_header(villa_id),
         json={"room_id": room_id},
     )
     return parse_obj_as(Room, (await _request(adapter, bot, request))["room"])
 
 
 async def _get_villa_group_room_list(
-    adapter: "Adapter", bot: "Bot", villa_id: int
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
 ) -> List[GroupRoom]:
     request = Request(
         method="GET",
         url=adapter.base_url / "vila/api/bot/platform/getVillaGroupRoomList",
         headers=bot.get_authorization_header(villa_id),
     )
     return parse_obj_as(
-        List[GroupRoom], (await _request(adapter, bot, request))["list"]
+        List[GroupRoom],
+        (await _request(adapter, bot, request))["list"],
     )
 
 
 async def _sort_room_list(
-    adapter: "Adapter", bot: "Bot", villa_id: int, room_list: List[RoomSort]
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    room_list: List[RoomSort],
 ) -> None:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/sortRoomList",
         headers=bot.get_authorization_header(villa_id),
         json={"villa_id": villa_id, "room_list": [room.dict() for room in room_list]},
     )
     await _request(adapter, bot, request)
 
 
 async def _operate_member_to_role(
-    adapter: "Adapter", bot: "Bot", villa_id: int, role_id: int, uid: int, is_add: bool
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    role_id: int,
+    uid: int,
+    is_add: bool,
 ) -> None:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/operateMemberToRole",
         headers=bot.get_authorization_header(villa_id),
         json={"role_id": role_id, "uid": uid, "is_add": is_add},
     )
@@ -300,55 +349,66 @@
             "permissions": permissions,
         },
     )
     await _request(adapter, bot, request)
 
 
 async def _delete_member_role(
-    adapter: "Adapter", bot: "Bot", villa_id: int, role_id: int
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    role_id: int,
 ) -> None:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/deleteMemberRole",
         headers=bot.get_authorization_header(villa_id),
         json={"id": role_id},
     )
     await _request(adapter, bot, request)
 
 
 async def _get_member_role_info(
-    adapter: "Adapter", bot: "Bot", villa_id: int, role_id: int
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
+    role_id: int,
 ) -> MemberRoleDetail:
     request = Request(
         method="GET",
         url=adapter.base_url / "vila/api/bot/platform/getMemberRoleInfo",
         headers=bot.get_authorization_header(villa_id),
         json={"role_id": role_id},
     )
     return parse_obj_as(
-        MemberRoleDetail, (await _request(adapter, bot, request))["role"]
+        MemberRoleDetail,
+        (await _request(adapter, bot, request))["role"],
     )
 
 
 async def _get_villa_member_roles(
-    adapter: "Adapter", bot: "Bot", villa_id: int
+    adapter: "Adapter",
+    bot: "Bot",
+    villa_id: int,
 ) -> List[MemberRoleDetail]:
     request = Request(
         method="GET",
         url=adapter.base_url / "vila/api/bot/platform/getVillaMemberRoles",
         headers=bot.get_authorization_header(villa_id),
     )
     return parse_obj_as(
-        List[MemberRoleDetail], (await _request(adapter, bot, request))["list"]
+        List[MemberRoleDetail],
+        (await _request(adapter, bot, request))["list"],
     )
 
 
 async def _get_all_emoticons(adapter: "Adapter", bot: "Bot") -> List[Emoticon]:
     request = Request(
-        method="GET", url=adapter.base_url / "vila/api/bot/platform/getAllEmoticons"
+        method="GET",
+        url=adapter.base_url / "vila/api/bot/platform/getAllEmoticons",
     )
     return parse_obj_as(List[Emoticon], (await _request(adapter, bot, request))["list"])
 
 
 async def _audit(
     adapter: "Adapter",
     bot: "Bot",
@@ -368,15 +428,31 @@
             "room_id": room_id,
             "uid": uid,
         },
     )
     return (await _request(adapter, bot, request))["audit_id"]
 
 
-API_HANDLERS = {
+async def _transfer_image(
+    adapter: "Adapter",
+    bot: "Bot",
+    url: str,
+) -> str:
+    request = Request(
+        method="POST",
+        url=adapter.base_url / "vila/api/bot/platform/transferImage",
+        headers=bot.get_authorization_header(),
+        json={
+            "url": url,
+        },
+    )
+    return (await _request(adapter, bot, request))["new_url"]
+
+
+API_HANDLERS: Dict[str, Callable[..., Awaitable[Any]]] = {
     "check_member_bot_access_token": _check_member_bot_access_token,
     "get_villa": _get_villa,
     "get_member": _get_member,
     "get_villa_members": _get_villa_members,
     "delete_villa_member": _delete_villa_member,
     "pin_message": _pin_message,
     "recall_message": _recall_message,
@@ -395,8 +471,9 @@
     "create_member_role": _create_member_role,
     "edit_member_role": _edit_member_role,
     "delete_member_role": _delete_member_role,
     "get_member_role_info": _get_member_role_info,
     "get_villa_member_roles": _get_villa_member_roles,
     "get_all_emoticons": _get_all_emoticons,
     "audit": _audit,
+    "transfer_image": _transfer_image,
 }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import sys
-import json
-import inspect
 from enum import Enum, IntEnum
-from typing import Any, Dict, List, Union, Literal, Optional
+import inspect
+import json
+import sys
+from typing import Any, Dict, List, Literal, Optional, Union
 
-from pydantic import Field, BaseModel, validator
+from pydantic import BaseModel, Field, validator
 
 
 class ApiResponse(BaseModel):
     retcode: int
     message: str
     data: Any
 
@@ -79,15 +79,15 @@
     basic: MemberBasic
     role_id_list: List[int]
     joined_at: int
     role_list: List["MemberRole"]
 
 
 class MemberListReturn(BaseModel):
-    list: List[Member]
+    list: List[Member]  # noqa: A003
     next_offset: int
 
 
 # 消息部分
 # see https://webstatic.mihoyo.com/vila/bot/doc/message_api/
 class MentionType(IntEnum):
     ALL = 1
@@ -166,14 +166,15 @@
     url: str
 
 
 class PostMessageContent(BaseModel):
     post_id: str
 
     @validator("post_id")
+    @classmethod
     def __deal_post_id(cls, v: str):
         s = v.split("/")[-1]
         if s.isdigit():
             return s
         raise ValueError(f"Invalid post_id: {v}, post_id must be a number.")
 
 
@@ -206,14 +207,15 @@
     extra: Dict[str, Any]
     name: str
     alias: str
     id: str
     portrait: str
 
     @validator("extra", pre=True)
+    @classmethod
     def extra_str_to_dict(cls, v: Any):
         if isinstance(v, str):
             return json.loads(v)
         return v
 
 
 class Trace(BaseModel):
@@ -387,15 +389,15 @@
 # see https://webstatic.mihoyo.com/vila/bot/doc/emoticon_api/
 class Emoticon(BaseModel):
     emoticon_id: int
     describe_text: str
     icon: str
 
 
-for name, obj in inspect.getmembers(sys.modules[__name__]):
+for _, obj in inspect.getmembers(sys.modules[__name__]):
     if inspect.isclass(obj) and issubclass(obj, BaseModel):
         obj.update_forward_refs()
 
 
 __all__ = [
     "ApiResponse",
     "BotAuth",
```

### Comparing `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Union, Optional
+import base64
+import hashlib
+import hmac
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from typing_extensions import override
+from urllib.parse import urlencode
 
-from nonebot.typing import overrides
+from nonebot.adapters import Bot as BaseBot
 from nonebot.message import handle_event
-from nonebot.internal.adapter.adapter import Adapter
 
-from nonebot.adapters import Bot as BaseBot
+import rsa
 
-from .utils import log
-from .message import Message, MessageSegment
-from .event import Event, SendMessageEvent, AddQuickEmoticonEvent
 from .api import (
-    Link,
+    ApiClient,
     Badge,
-    Image,
-    Robot,
     Command,
-    ApiClient,
-    QuoteInfo,
-    TextEntity,
-    MentionType,
-    PreviewLink,
+    Image,
+    ImageMessageContent,
+    Link,
     MentionedAll,
     MentionedInfo,
-    MentionedUser,
-    VillaRoomLink,
     MentionedRobot,
+    MentionedUser,
+    MentionType,
     MessageContentInfo,
     PostMessageContent,
+    PreviewLink,
+    QuoteInfo,
+    Robot,
+    TextEntity,
     TextMessageContent,
-    ImageMessageContent,
+    VillaRoomLink,
 )
+from .config import BotInfo
+from .event import AddQuickEmoticonEvent, Event, SendMessageEvent
+from .message import Message, MessageSegment
+from .utils import log
 
 if TYPE_CHECKING:
     from .adapter import Adapter
 
 
 async def _check_reply(bot: "Bot", event: SendMessageEvent):
     """检查事件是否有引用消息，如果有则设置 reply 字段。
@@ -102,22 +107,33 @@
 
 
 class Bot(BaseBot, ApiClient):
     """
     大别野协议 Bot 适配。
     """
 
-    @overrides(BaseBot)
-    def __init__(self, adapter: Adapter, self_id: str, bot_secret: str):
-        super().__init__(adapter, self_id)
+    @override
+    def __init__(
+        self,
+        adapter: "Adapter",
+        bot_info: BotInfo,
+    ) -> None:
+        super().__init__(adapter, bot_info.bot_id)
         self.adapter: Adapter = adapter
-        self.bot_secret: str = bot_secret
+        self.bot_secret: str = bot_info.bot_secret
+        self.bot_secret_encrypt = hmac.new(
+            bot_info.pub_key.encode(),
+            bot_info.bot_secret.encode(),
+            hashlib.sha256,
+        ).hexdigest()
+        self.pub_key = rsa.PublicKey.load_pkcs1_openssl_pem(bot_info.pub_key.encode())
+        self.verify_event = bot_info.verify_event
         self._bot_info: Optional[Robot] = None
 
-    @overrides(BaseBot)
+    @override
     def __repr__(self) -> str:
         return f"Bot(type={self.type!r}, self_id={self.self_id!r})"
 
     @property
     def nickname(self) -> str:
         """Bot 昵称"""
         if not self._bot_info:
@@ -154,38 +170,52 @@
     async def handle_event(self, event: Event):
         """处理事件"""
         if isinstance(event, SendMessageEvent):
             _check_at_me(self, event)
             # await _check_reply(self, event)
         await handle_event(self, event)
 
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
+        except rsa.VerificationError:
+            return False
+        return True
+
     def get_authorization_header(
-        self, villa_id: Optional[int] = None
+        self,
+        villa_id: Optional[int] = None,
     ) -> Dict[str, str]:
         """Bot 鉴权凭证请求头
 
         参数:
             villa_id: 大别野ID
 
         返回:
             Dict[str, str]: 请求头
         """
         return {
             "x-rpc-bot_id": self.self_id,
-            "x-rpc-bot_secret": self.bot_secret,
+            "x-rpc-bot_secret": self.bot_secret_encrypt,
             "x-rpc-bot_villa_id": str(villa_id or ""),
         }
 
-    @overrides(BaseBot)
+    @override
     async def send(
         self,
         event: Event,
         message: Union[str, Message, MessageSegment],
-        mention_sender: bool = False,
-        quote_message: bool = False,
         **kwargs: Any,
     ) -> str:
         """发送消息
 
         参数:
             event: 事件
             message: 消息
@@ -198,36 +228,40 @@
         返回:
             str: 消息ID
         """
         if not isinstance(event, (SendMessageEvent, AddQuickEmoticonEvent)):
             raise RuntimeError("Event cannot be replied to!")
         message = MessageSegment.text(message) if isinstance(message, str) else message
         message = message if isinstance(message, Message) else Message(message)
-        if mention_sender:
+        if kwargs.pop("mention_sender", False) or kwargs.pop("at_sender", False):
             message.insert(
                 0,
                 MessageSegment.mention_user(
-                    user_id=event.from_user_id
-                    if isinstance(event, SendMessageEvent)
-                    else event.uid,
-                    user_name=event.content.user.name
-                    if isinstance(event, SendMessageEvent)
-                    else None,
+                    user_id=(
+                        event.from_user_id
+                        if isinstance(event, SendMessageEvent)
+                        else event.uid
+                    ),
+                    user_name=(
+                        event.content.user.name
+                        if isinstance(event, SendMessageEvent)
+                        else None
+                    ),
                     villa_id=event.villa_id,
                 ),
             )
-        if quote_message:
+        if kwargs.pop("quote_message", False) or kwargs.pop("reply_message", False):
             message += MessageSegment.quote(event.msg_uid, event.send_at)
         content_info = await self.parse_message_content(message)
-        if isinstance(content_info.content, TextMessageContent):
-            object_name = "MHY:Text"
+        if isinstance(content_info.content, PostMessageContent):
+            object_name = "MHY:Post"
         elif isinstance(content_info.content, ImageMessageContent):
             object_name = "MHY:Image"
         else:
-            object_name = "MHY:Post"
+            object_name = "MHY:Text"
         return await self.send_message(
             villa_id=event.villa_id,
             room_id=event.room_id,
             object_name=object_name,
             msg_content=content_info.json(by_alias=True, exclude_none=True),
         )
 
@@ -261,15 +295,17 @@
         if preview_link_seg := message["preview_link"]:
             preview_link: Optional[PreviewLink] = preview_link_seg[-1].data[
                 "preview_link"
             ]
         else:
             preview_link = None
 
-        cal_len = lambda x: len(x.encode("utf-16")) // 2 - 1
+        def cal_len(x):
+            return len(x.encode("utf-16")) // 2 - 1
+
         message_text = ""
         message_offset = 0
         entities: List[TextEntity] = []
         mentioned = MentionedInfo(type=MentionType.PART)
         for seg in message:
             try:
                 if seg.type in ("quote", "image", "post", "badge", "preview_link"):
@@ -282,43 +318,48 @@
                     seg_text = f"@{mention_all.show_text} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
                             entity=mention_all,
-                        )
+                        ),
                     )
                     mentioned.type = MentionType.ALL
                 elif seg.type == "mention_robot":
                     mention_robot: MentionedRobot = seg.data["mention_robot"]
                     seg_text = f"@{mention_robot.bot_name} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
-                            offset=message_offset, length=length, entity=mention_robot
-                        )
+                            offset=message_offset,
+                            length=length,
+                            entity=mention_robot,
+                        ),
                     )
                     mentioned.user_id_list.append(mention_robot.bot_id)
                 elif seg.type == "mention_user":
                     mention_user: MentionedUser = seg.data["mention_user"]
                     if mention_user.user_name is None:
                         # 需要调用API获取被@的用户的昵称
                         user = await self.get_member(
-                            villa_id=seg.data["villa_id"], uid=int(mention_user.user_id)
+                            villa_id=seg.data["villa_id"],
+                            uid=int(mention_user.user_id),
                         )
                         seg_text = f"@{user.basic.nickname} "
                         mention_user.user_name = user.basic.nickname
                     else:
                         seg_text = f"@{mention_user.user_name} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
-                            offset=message_offset, length=length, entity=mention_user
-                        )
+                            offset=message_offset,
+                            length=length,
+                            entity=mention_user,
+                        ),
                     )
                     mentioned.user_id_list.append(str(mention_user.user_id))
                 elif seg.type == "room_link":
                     room_link: VillaRoomLink = seg.data["room_link"]
                     if room_link.room_name is None:
                         # 需要调用API获取房间的名称
                         room = await self.get_room(
@@ -328,46 +369,50 @@
                         seg_text = f"#{room.room_name} "
                         room_link.room_name = room.room_name
                     else:
                         seg_text = f"#{room_link.room_name} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
-                            offset=message_offset, length=length, entity=room_link
-                        )
+                            offset=message_offset,
+                            length=length,
+                            entity=room_link,
+                        ),
                     )
                 else:
                     link: Link = seg.data["link"]
                     seg_text = link.show_text
                     length = cal_len(seg_text)
                     entities.append(
-                        TextEntity(offset=message_offset, length=length, entity=link)
+                        TextEntity(offset=message_offset, length=length, entity=link),
                     )
                 message_offset += length
                 message_text += seg_text
             except Exception as e:
                 log("WARNING", "error when parse message content", e)
 
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
                     content = ImageMessageContent(**images[-1].dict())
             elif preview_link:
                 content = TextMessageContent(
-                    text="\u200B", preview_link=preview_link, badge=badge
+                    text="\u200b",
+                    preview_link=preview_link,
+                    badge=badge,
                 )
             elif post:
                 content = post
             else:
                 raise ValueError("message content is empty")
         else:
             content = TextMessageContent(
```

### Comparing `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/config.py` & `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from typing import List, Optional
 
-from pydantic import Extra, Field, BaseModel, root_validator
+from pydantic import BaseModel, Extra, Field, root_validator
 
 
 class BotInfo(BaseModel):
     bot_id: str
     bot_secret: str
+    pub_key: str
     callback_url: Optional[str] = None
     ws_url: Optional[str] = None
     ws_secret: Optional[str] = None
+    verify_event: bool = True
 
     # 不能同时存在 callback_url 和 ws_url
     @root_validator
+    @classmethod
     def check_url(cls, values):
         if values.get("callback_url") and values.get("ws_url"):
             raise ValueError("callback_url and ws_url cannot exist at the same time")
         return values
 
 
 class Config(BaseModel, extra=Extra.ignore):
```

### Comparing `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/event.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import json
 from enum import IntEnum
-from typing import Any, Dict, Union, Literal, Optional
+import json
+from typing import Any, Dict, Literal, Optional, Union
+from typing_extensions import override
 
-from pydantic import root_validator
-from nonebot.typing import overrides
+from nonebot.adapters import Event as BaseEvent
 from nonebot.utils import escape_tag
 
-from nonebot.adapters import Event as BaseEvent
+from pydantic import root_validator
 
+from .api import MessageContentInfoGet, Robot
 from .message import Message, MessageSegment
-from .api import Robot, MessageContentInfoGet
 
 
 class EventType(IntEnum):
     """事件类型"""
 
     JoinVilla = 1
     SendMessage = 2
@@ -49,53 +49,53 @@
     """事件回调时间"""
 
     @property
     def bot_id(self) -> str:
         """机器人ID"""
         return self.robot.template.id
 
-    @overrides(BaseEvent)
+    @override
     def get_event_name(self) -> str:
         return self.type.name
 
-    @overrides(BaseEvent)
+    @override
     def get_event_description(self) -> str:
         return escape_tag(repr(self.dict()))
 
-    @overrides(BaseEvent)
+    @override
     def get_message(self):
         raise ValueError("Event has no message!")
 
-    @overrides(BaseEvent)
+    @override
     def get_user_id(self) -> str:
         raise ValueError("Event has no context!")
 
-    @overrides(BaseEvent)
+    @override
     def get_session_id(self) -> str:
         raise ValueError("Event has no context!")
 
-    @overrides(BaseEvent)
+    @override
     def is_tome(self) -> bool:
         return False
 
 
 class NoticeEvent(Event):
     """通知事件"""
 
-    @overrides(BaseEvent)
+    @override
     def get_type(self) -> str:
         return "notice"
 
 
 class MessageEvent(Event):
     """消息事件
 
     但目前大别野只有SendMessageEvent这一种消息事件，所以推荐直接使用SendMessageEvent"""
 
-    @overrides(BaseEvent)
+    @override
     def get_type(self) -> str:
         return "message"
 
 
 class JoinVillaEvent(NoticeEvent):
     """新用户加入大别野事件
 
@@ -110,25 +110,28 @@
     """用户加入时间的时间戳"""
 
     @property
     def villa_id(self) -> int:
         """大别野ID"""
         return self.robot.villa_id
 
-    @overrides(BaseEvent)
+    @override
     def get_event_description(self) -> str:
         return escape_tag(
-            f"User(nickname={self.join_user_nickname},id={self.join_uid}) join Villa(id={self.villa_id})"
+            (
+                f"User(nickname={self.join_user_nickname},id={self.join_uid}) "
+                f"join Villa(id={self.villa_id})"
+            ),
         )
 
-    @overrides(BaseEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.join_uid)
 
-    @overrides(BaseEvent)
+    @override
     def get_session_id(self) -> str:
         return str(self.join_uid)
 
 
 class SendMessageEvent(MessageEvent):
     """用户@机器人发送消息事件
 
@@ -160,53 +163,59 @@
     """事件原始消息"""
 
     @property
     def villa_id(self) -> int:
         """大别野ID"""
         return self.robot.villa_id
 
-    @overrides(BaseEvent)
+    @override
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Message(id={self.msg_uid}) was sent from User(nickname={self.nickname},id={self.from_user_id}) in Room(id={self.room_id}) of Villa(id={self.villa_id}), content={repr(self.message)}"
+            (
+                f"Message(id={self.msg_uid}) was sent from"
+                f" User(nickname={self.nickname}, id={self.from_user_id}) in"
+                f" Room(id={self.room_id}) of Villa(id={self.villa_id}),"
+                f" content={repr(self.message)}"
+            ),
         )
 
-    @overrides(BaseEvent)
+    @override
     def get_message(self) -> Message:
         """获取事件消息"""
         return self.message
 
-    @overrides(Event)
+    @override
     def is_tome(self) -> bool:
         """是否和Bot有关"""
         return self.to_me
 
-    @overrides(BaseEvent)
+    @override
     def get_user_id(self) -> str:
         """获取用户ID"""
         return str(self.from_user_id)
 
-    @overrides(BaseEvent)
+    @override
     def get_session_id(self) -> str:
         """获取会话ID"""
         return f"{self.room_id}-{self.from_user_id}"
 
     @root_validator(pre=True)
+    @classmethod
     def _(cls, data: Dict[str, Any]):
         if not data.get("content"):
             return data
         msg = Message()
         data["content"] = json.loads(data["content"])
         msg_content_info = data["content"]
         if quote := msg_content_info.get("quote"):
             msg.append(
                 MessageSegment.quote(
                     message_id=quote["quoted_message_id"],
                     message_send_time=quote["quoted_message_send_time"],
-                )
+                ),
             )
 
         content = msg_content_info["content"]
         text = content["text"]
         entities = content["entities"]
         if not entities:
             return Message(MessageSegment.text(text))
@@ -218,45 +227,47 @@
             offset: int = entity["offset"]
             length: int = entity["length"]
             entity_detail = entity["entity"]
             if offset != end_offset:
                 msg.append(
                     MessageSegment.text(
                         text[((end_offset + 1) * 2) : ((offset + 1) * 2)].decode(
-                            "utf-16"
-                        )
-                    )
+                            "utf-16",
+                        ),
+                    ),
                 )
             entity_text = text[(offset + 1) * 2 : (offset + length + 1) * 2].decode(
-                "utf-16"
+                "utf-16",
             )
             if entity_detail["type"] == "mentioned_robot":
                 entity_detail["bot_name"] = entity_text.lstrip("@")[:-1]
                 msg.append(
                     MessageSegment.mention_robot(
-                        entity_detail["bot_id"], entity_detail["bot_name"]
-                    )
+                        entity_detail["bot_id"],
+                        entity_detail["bot_name"],
+                    ),
                 )
             elif entity_detail["type"] == "mentioned_user":
                 entity_detail["user_name"] = entity_text.lstrip("@")[:-1]
                 msg.append(
                     MessageSegment.mention_user(
-                        int(entity_detail["user_id"]), data["villa_id"]
-                    )
+                        int(entity_detail["user_id"]),
+                        data["villa_id"],
+                    ),
                 )
             elif entity_detail["type"] == "mention_all":
                 entity_detail["show_text"] = entity_text.lstrip("@")[:-1]
                 msg.append(MessageSegment.mention_all(entity_detail["show_text"]))
             elif entity_detail["type"] == "villa_room_link":
                 entity_detail["room_name"] = entity_text.lstrip("#")[:-1]
                 msg.append(
                     MessageSegment.room_link(
                         int(entity_detail["villa_id"]),
                         int(entity_detail["room_id"]),
-                    )
+                    ),
                 )
             else:
                 entity_detail["show_text"] = entity_text
                 msg.append(MessageSegment.link(entity_detail["url"], entity_text))
             last_offset = offset
             last_length = length
         end_offset = last_offset + last_length
@@ -272,34 +283,34 @@
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html###CreateRobot"""
 
     type: Literal[EventType.CreateRobot] = EventType.CreateRobot
     villa_id: int
     """大别野ID"""
 
-    @overrides(BaseEvent)
+    @override
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Bot(id={self.bot_id}) was added to Villa(id={self.villa_id})"
+            f"Bot(id={self.bot_id}) was added to Villa(id={self.villa_id})",
         )
 
 
 class DeleteRobotEvent(NoticeEvent):
     """大别野删除机器人实例事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html###DeleteRobot"""
 
     type: Literal[EventType.DeleteRobot] = EventType.DeleteRobot
     villa_id: int
     """大别野ID"""
 
-    @overrides(BaseEvent)
+    @override
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Bot(id={self.bot_id}) was removed from Villa(id={self.villa_id})"
+            f"Bot(id={self.bot_id}) was removed from Villa(id={self.villa_id})",
         )
 
 
 class AddQuickEmoticonEvent(NoticeEvent):
     """用户使用表情回复消息表态事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AddQuickEmoticon"""
@@ -318,18 +329,23 @@
     msg_uid: str
     """被回复的消息 id"""
     bot_msg_id: Optional[str]
     """如果被回复的消息从属于机器人，则该字段不为空字符串"""
     is_cancel: bool = False
     """是否是取消表情"""
 
-    @overrides(BaseEvent)
+    @override
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Emoticon(name={self.emoticon}, id={self.emoticon_id}) was {'removed from' if self.is_cancel else 'added to'} Message(id={self.msg_uid}) by User(id={self.uid}) in Room(id=Villa(id={self.room_id}) of Villa(id={self.villa_id})"
+            (
+                f"Emoticon(name={self.emoticon}, id={self.emoticon_id}) was "
+                f"{'removed from' if self.is_cancel else 'added to'} "
+                f"Message(id={self.msg_uid}) by User(id={self.uid}) in "
+                f"Room(id=Villa(id={self.room_id}) of Villa(id={self.villa_id})"
+            ),
         )
 
 
 class AuditCallbackEvent(NoticeEvent):
     """审核结果回调事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AuditCallback"""
@@ -346,18 +362,22 @@
     user_id: int
     """用户 id（和审核接口调用方传入的值一致）"""
     pass_through: str
     """透传数据（和审核接口调用方传入的值一致）"""
     audit_result: AuditResult
     """审核结果"""
 
-    @overrides(BaseEvent)
+    @override
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Audit(id={self.audit_id},result={self.audit_result}) of User(id={self.user_id}) in Room(id={self.room_id}) of Villa(id={self.villa_id})"
+            (
+                f"Audit(id={self.audit_id},result={self.audit_result}) of "
+                f"User(id={self.user_id}) in Room(id={self.room_id}) of "
+                f"Villa(id={self.villa_id})"
+            ),
         )
 
 
 event_classes = Union[
     JoinVillaEvent,
     SendMessageEvent,
     CreateRobotEvent,
@@ -366,15 +386,15 @@
     AuditCallbackEvent,
 ]
 
 
 def pre_handle_event(payload: Dict[str, Any]):
     if (event_type := EventType._value2member_map_.get(payload["type"])) is None:
         raise ValueError(
-            f"Unknown event type: {payload['type']} data={escape_tag(str(payload))}"
+            f"Unknown event type: {payload['type']} data={escape_tag(str(payload))}",
         )
     event_name = event_type.name
     if event_name not in payload["extend_data"]["EventData"]:
         raise ValueError("Cannot find event data for event type: {event_name}")
     payload.update(payload["extend_data"]["EventData"][event_name])
     payload.pop("extend_data")
     return payload
```

### Comparing `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-from typing import Type, Union, Iterable, Optional
+from typing import Iterable, Optional, Type, Union
+from typing_extensions import override
 
-from nonebot.typing import overrides
+from nonebot.adapters import (
+    Message as BaseMessage,
+    MessageSegment as BaseMessageSegment,
+)
 from nonebot.utils import escape_tag
 
-from nonebot.adapters import Message as BaseMessage
-from nonebot.adapters import MessageSegment as BaseMessageSegment
-
 from .api.models import *
 
 
 class MessageSegment(BaseMessageSegment["Message"]):
     @classmethod
-    @overrides(BaseMessageSegment)
+    @override
     def get_message_class(cls) -> Type["Message"]:
         return Message
 
-    @overrides(BaseMessageSegment)
+    @override
     def __repr__(self) -> str:
         return self.__str__()
 
-    @overrides(BaseMessageSegment)
+    @override
     def __add__(
-        self, other: Union[str, "MessageSegment", Iterable["MessageSegment"]]
+        self,
+        other: Union[str, "MessageSegment", Iterable["MessageSegment"]],
     ) -> "Message":
         return super().__add__(other)
 
-    @overrides(BaseMessageSegment)
+    @override
     def __radd__(
-        self, other: Union[str, "MessageSegment", Iterable["MessageSegment"]]
+        self,
+        other: Union[str, "MessageSegment", Iterable["MessageSegment"]],
     ) -> "Message":
         return super().__radd__(other)
 
-    @overrides(BaseMessageSegment)
+    @override
     def is_text(self) -> bool:
         return self.type == "text"
 
     @staticmethod
     def text(text: str) -> "TextSegment":
         """纯文本消息段
 
@@ -61,15 +64,17 @@
         return MentionRobotSegement(
             "mention_robot",
             {"mention_robot": MentionedRobot(bot_id=bot_id, bot_name=bot_name)},
         )
 
     @staticmethod
     def mention_user(
-        user_id: int, user_name: Optional[str] = None, villa_id: Optional[int] = None
+        user_id: int,
+        user_name: Optional[str] = None,
+        villa_id: Optional[int] = None,
     ) -> "MentionUserSegement":
         """@用户消息段
 
         user_name和villa_id必须有其中之一
 
         参数:
             user_id: 用户ID
@@ -81,15 +86,16 @@
         """
         if not (user_name or villa_id):
             raise ValueError("user_name and villa_id must have one of them")
         return MentionUserSegement(
             "mention_user",
             {
                 "mention_user": MentionedUser(
-                    user_id=str(user_id), user_name=user_name
+                    user_id=str(user_id),
+                    user_name=user_name,
                 ),
                 "villa_id": villa_id,
             },
         )
 
     @staticmethod
     def mention_all(show_text: str = "全体成员") -> "MentionAllSegement":
@@ -98,36 +104,41 @@
         参数:
             show_text: 展示文本. 默认为 "全体成员".
 
         返回:
             MentionAllSegement: 消息段对象
         """
         return MentionAllSegement(
-            "mention_all", {"mention_all": MentionedAll(show_text=show_text)}
+            "mention_all",
+            {"mention_all": MentionedAll(show_text=show_text)},
         )
 
     @staticmethod
     def room_link(
-        villa_id: int, room_id: int, room_name: Optional[str] = None
+        villa_id: int,
+        room_id: int,
+        room_name: Optional[str] = None,
     ) -> "RoomLinkSegment":
         """房间链接消息段，点击后可以跳转到指定房间
 
         参数:
             villa_id: 大别野ID
             room_id: 房间ID
 
         返回:
             VillaRoomLinkSegment: 消息段对象
         """
         return RoomLinkSegment(
             "room_link",
             {
                 "room_link": VillaRoomLink(
-                    villa_id=str(villa_id), room_id=str(room_id), room_name=room_name
-                )
+                    villa_id=str(villa_id),
+                    room_id=str(room_id),
+                    room_name=room_name,
+                ),
             },
         )
 
     @staticmethod
     def link(
         url: str,
         show_text: Optional[str] = None,
@@ -145,15 +156,15 @@
         return LinkSegment(
             "link",
             {
                 "link": Link(
                     url=url,
                     show_text=show_text or url,
                     requires_bot_access_token=requires_bot_access_token,
-                )
+                ),
             },
         )
 
     @staticmethod
     def quote(message_id: str, message_send_time: int) -> "QuoteSegment":
         """引用(回复)消息段
 
@@ -168,15 +179,15 @@
             "quote",
             {
                 "quote": QuoteInfo(
                     quoted_message_id=message_id,
                     quoted_message_send_time=message_send_time,
                     original_message_id=message_id,
                     original_message_send_time=message_send_time,
-                )
+                ),
             },
         )
 
     @staticmethod
     def image(
         url: str,
         width: Optional[int] = None,
@@ -195,19 +206,21 @@
             ImageSegment: 消息段对象
         """
         return ImageSegment(
             "image",
             {
                 "image": Image(
                     url=url,
-                    size=ImageSize(width=width, height=height)
-                    if width and height
-                    else None,
+                    size=(
+                        ImageSize(width=width, height=height)
+                        if width and height
+                        else None
+                    ),
                     file_size=file_size,
-                )
+                ),
             },
         )
 
     @staticmethod
     def post(post_id: str) -> "PostSegment":
         """帖子转发消息段
 
@@ -250,15 +263,15 @@
                     icon_url=icon_url,
                     image_url=image_url,
                     is_internal_link=is_internal_link,
                     title=title,
                     content=content,
                     url=url,
                     source_name=source_name,
-                )
+                ),
             },
         )
 
     @staticmethod
     def badge(
         icon_url: str,
         text: str,
@@ -277,104 +290,106 @@
         return BadgeSegment(
             "badge",
             {
                 "badge": Badge(
                     icon_url=icon_url,
                     text=text,
                     url=url,
-                )
+                ),
             },
         )
 
 
 class TextSegment(MessageSegment):
-    @overrides(MessageSegment)
+    @override
     def __str__(self) -> str:
         return escape_tag(self.data["text"])
 
 
 class MentionRobotSegement(MessageSegment):
-    @overrides(MessageSegment)
+    @override
     def __str__(self) -> str:
         return repr(self.data["mention_robot"])
 
 
 class MentionUserSegement(MessageSegment):
-    @overrides(MessageSegment)
+    @override
     def __str__(self) -> str:
         return repr(self.data["mention_user"])
 
 
 class MentionAllSegement(MessageSegment):
-    @overrides(MessageSegment)
+    @override
     def __str__(self) -> str:
         return repr(self.data["mention_all"])
 
 
 class RoomLinkSegment(MessageSegment):
-    @overrides(MessageSegment)
+    @override
     def __str__(self) -> str:
         return repr(self.data["room_link"])
 
 
 class LinkSegment(MessageSegment):
-    @overrides(MessageSegment)
+    @override
     def __str__(self) -> str:
         return repr(self.data["link"])
 
 
 class ImageSegment(MessageSegment):
-    @overrides(MessageSegment)
+    @override
     def __str__(self) -> str:
         return repr(self.data["image"])
 
 
 class QuoteSegment(MessageSegment):
-    @overrides(MessageSegment)
+    @override
     def __str__(self) -> str:
         return repr(self.data["quote"])
 
 
 class PostSegment(MessageSegment):
-    @overrides(MessageSegment)
+    @override
     def __str__(self) -> str:
         return repr(self.data["post"])
 
 
 class PreviewLinkSegment(MessageSegment):
-    @overrides
+    @override
     def __str__(self) -> str:
         return repr(self.data["preview_link"])
 
 
 class BadgeSegment(MessageSegment):
-    @overrides(MessageSegment)
+    @override
     def __str__(self) -> str:
         return repr(self.data["badge"])
 
 
 class Message(BaseMessage[MessageSegment]):
     @classmethod
-    @overrides(BaseMessage)
+    @override
     def get_segment_class(cls) -> Type[MessageSegment]:
         return MessageSegment
 
-    @overrides(BaseMessage)
+    @override
     def __add__(
-        self, other: Union[str, MessageSegment, Iterable[MessageSegment]]
+        self,
+        other: Union[str, MessageSegment, Iterable[MessageSegment]],
     ) -> "Message":
-        return super(Message, self).__add__(
-            MessageSegment.text(other) if isinstance(other, str) else other
+        return super().__add__(
+            MessageSegment.text(other) if isinstance(other, str) else other,
         )
 
-    @overrides(BaseMessage)
+    @override
     def __radd__(
-        self, other: Union[str, MessageSegment, Iterable[MessageSegment]]
+        self,
+        other: Union[str, MessageSegment, Iterable[MessageSegment]],
     ) -> "Message":
-        return super(Message, self).__radd__(
-            MessageSegment.text(other) if isinstance(other, str) else other
+        return super().__radd__(
+            MessageSegment.text(other) if isinstance(other, str) else other,
         )
 
     @staticmethod
-    @overrides(BaseMessage)
+    @override
     def _construct(msg: str) -> Iterable[MessageSegment]:
         yield MessageSegment.text(msg)
```

### Comparing `nonebot_adapter_villa-0.5.6/nonebot/adapters/villa/permission.py` & `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/permission.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from typing import Union
 
-from nonebot.permission import Permission
-
+from nonebot.adapters.villa import AddQuickEmoticonEvent, Bot, SendMessageEvent
 from nonebot.adapters.villa.api import RoleType
-from nonebot.adapters.villa import Bot, SendMessageEvent, AddQuickEmoticonEvent
+from nonebot.permission import Permission
 
 
 async def is_owner_or_admin(
-    bot: Bot, event: Union[SendMessageEvent, AddQuickEmoticonEvent]
+    bot: Bot,
+    event: Union[SendMessageEvent, AddQuickEmoticonEvent],
 ) -> bool:
     user_id = event.from_user_id if isinstance(event, SendMessageEvent) else event.uid
     user = await bot.get_member(villa_id=event.villa_id, uid=user_id)
     return any(
         role.role_type in (RoleType.OWNER, RoleType.ADMIN) for role in user.role_list
     )
 
 
 OWNER_OR_ADMIN = Permission(is_owner_or_admin)
 """别野房东或管理员权限"""
 
 
 async def is_owner(
-    bot: Bot, event: Union[SendMessageEvent, AddQuickEmoticonEvent]
+    bot: Bot,
+    event: Union[SendMessageEvent, AddQuickEmoticonEvent],
 ) -> bool:
     user_id = event.from_user_id if isinstance(event, SendMessageEvent) else event.uid
     user = await bot.get_member(villa_id=event.villa_id, uid=user_id)
     return any(role.role_type == RoleType.OWNER for role in user.role_list)
 
 
 OWNER = Permission(is_owner)
 """别野房东权限"""
 
 
 async def is_admin(
-    bot: Bot, event: Union[SendMessageEvent, AddQuickEmoticonEvent]
+    bot: Bot,
+    event: Union[SendMessageEvent, AddQuickEmoticonEvent],
 ) -> bool:
     user_id = event.from_user_id if isinstance(event, SendMessageEvent) else event.uid
     user = await bot.get_member(villa_id=event.villa_id, uid=user_id)
     return any(role.role_type == RoleType.ADMIN for role in user.role_list)
 
 
 ADMIN = Permission(is_admin)
```

### Comparing `nonebot_adapter_villa-0.5.6/PKG-INFO` & `nonebot_adapter_villa-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.5.6
+Version: 0.6.0
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot2 (>=2.0.0-beta.3,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: rsa (>=4.9,<5.0)
 Project-URL: Documentation, https://github.com/CMHopeSunshine/nonebot-adapter-villa
 Project-URL: Repository, https://github.com/CMHopeSunshine/nonebot-adapter-villa
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot-adapter-villa"></a>
 </p>
@@ -36,14 +37,17 @@
 <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
 <a href="https://pypi.python.org/pypi/nonebot-adapter-villa">
   <img src="https://img.shields.io/pypi/dm/nonebot-adapter-villa" alt="pypi download">
 </a>
 <a href="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/838e7f55-f8b8-49ff-aec0-29ad264931cf">
   <img src="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/838e7f55-f8b8-49ff-aec0-29ad264931cf.svg" alt="wakatime">
 </a>
+<a href="https://github.com/astral-sh/ruff">
+  <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="ruff">
+</a>
 
 </div>
 
 ## 安装
 
 在`nb create`创建项目时选择`Villa`适配器
 
@@ -65,42 +69,50 @@
 
 ```dotenv
 DRIVER=~fastapi+~httpx
 ```
 
 ### VILLA_BOTS
 
-配置 Bot 帐号列表，每个bot有3个必填配置，可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)(ID: `OpenVilla`)申请，取得以下配置：
+配置 Bot 帐号列表，每个bot有4个必填配置，可前往[「大别野开放平台」](https://open.miyoushe.com/#/login)(ID: `OpenVilla`)申请，取得以下配置：
 
 - `bot_id`: 机器人id，以`bot_`开头
 - `bot_secret`: 机器人密钥
+- `pub_key`: 加密和验证所需的pub_key
 - `callback_url`: http回调地址 endpoint，例如申请bot时给的回调地址是`http://域名/your/callback/url`，那么配置里的`callback_url`填写`/your/callback/url`
 
+此外还有以下选填配置：
+
+- `verify_event`：是否对回调事件签名进行验证
+
 例如：
 
 ```dotenv
 VILLA_BOTS='
 [
   {
     "bot_id": "bot_123456789",
     "bot_secret": "abc123def456",
-    "callback_url": "/your/callback/url"
+    "pub_key": "-----BEGIN PUBLIC KEY-----\nyour_pub_key\n-----END PUBLIC KEY-----\n",
+    "callback_url": "/your/callback/url",
+    "verify_event": true
   }
 ]
 '
 ```
 
-> 注意，当前大别野只能接收到有@Bot(在哪个位置皆可)的消息事件，且不能有多个@(即使是@两次Bot都不行)
-
 ## 已支持消息段
 
+> 注意，当前大别野只能接收到有@Bot(在哪个位置皆可)的消息事件，且不能有多个@(即使是@两次Bot都不行)
+
 - `MessageSegment.text`: 纯文本
   + 米游社自带表情也是用text来发送，以[表情名]格式，例如MessageSegment.text("[爱心]")
 - `MessageSegment.mention_robot`: @机器人
 - `MessageSegment.mention_user`: @用户
+  + `user_name`和`villa_id`必须给出其中之一，给`villa_id`时，调用api来获取用户名
 - `MessageSegment.mention_all`: @全体成员
 - `MessageSegment.room_link`: #房间跳转链接
 - `MessageSegment.link`: 超链接
   + 使用link的话链接能够点击进行跳转，使用text的话不能点击
   + 字段`show_text`是指链接显示的文字，但若指定了该字段，Web端大别野会无法正常跳转
   + 字段`requires_bot_access_token`为true时，跳转链接会带上含有用户信息的token
 - `MessageSegment.quote`: 引用(回复)消息
@@ -187,13 +199,14 @@
 使用命令`@bot /test 纯文本`时，bot会回复`这是一段纯文本`
 
 
 ## 交流、建议和反馈
 
 大别野 Bot 和本适配器均为开发测试中，如遇问题请提出 [issue](https://github.com/CMHopeSunshine/nonebot-adapter-villa/issues) ，感谢支持！
 
-也欢迎来我的大别野[「尘世闲游」]((https://dby.miyoushe.com/chat/1047/21652))(ID: `wgiJNaU`)进行交流~ 
+也欢迎来我的大别野[「尘世闲游」]((https://dby.miyoushe.com/chat/1047/21652))(ID: `wgiJNaU`)进行交流~
 
 ## 相关项目
 
 - [NoneBot2](https://github.com/nonebot/nonebot2): 非常好用的Python跨平台机器人框架！
 - [villa-py](https://github.com/CMHopeSunshine/villa-py): 大别野 Bot Python SDK。
+
```

#### html2text {}

```diff
@@ -1,48 +1,53 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.5.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.6.0 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
-(>=2.0.0-beta.3,<3.0.0) Project-URL: Documentation, https://github.com/
-CMHopeSunshine/nonebot-adapter-villa Project-URL: Repository, https://
-github.com/CMHopeSunshine/nonebot-adapter-villa Description-Content-Type: text/
-markdown
+(>=2.0.0,<3.0.0) Requires-Dist: rsa (>=4.9,<5.0) Project-URL: Documentation,
+https://github.com/CMHopeSunshine/nonebot-adapter-villa Project-URL:
+Repository, https://github.com/CMHopeSunshine/nonebot-adapter-villa
+Description-Content-Type: text/markdown
                             [nonebot-adapter-villa]
  # NoneBot-Adapter-Villa _â¨ å¤§å«é åè®®éé â¨_ [license] [version]
-                      [python] [pypi_download] [wakatime]
+                  [python] [pypi_download] [wakatime] [ruff]
 ## å®è£ å¨`nb create`åå»ºé¡¹ç®æ¶éæ©`Villa`ééå¨
 æå¨ç°æ`NoneBot2`é¡¹ç®ç®å½ä¸ä½¿ç¨èææ¶å®è£ï¼ ``` nb adapter
 install nonebot-adapter-villa ``` ## éç½® ä¿®æ¹ NoneBot éç½®æä»¶ `.env`
 æè `.env.*`ã ### Driver
 æ¬ééå¨åæ¶éè¦`ReverseDriver`å`ForwardDriver`ï¼åè [driver]
 (https://v2.nonebot.dev/docs/next/advanced/
 driver#%E9%A9%B1%E5%8A%A8%E5%99%A8%E7%B1%BB%E5%9E%8B) éç½®é¡¹ã ä¾å¦ï¼
 ```dotenv DRIVER=~fastapi+~httpx ``` ### VILLA_BOTS éç½® Bot
-å¸å·åè¡¨ï¼æ¯ä¸ªbotæ3ä¸ªå¿å¡«éç½®ï¼å¯åå¾å¤§å«é
-[ãæºå¨äººå¼åèç¤¾åºã](https://dby.miyoushe.com/chat/463/20020)(ID:
+å¸å·åè¡¨ï¼æ¯ä¸ªbotæ4ä¸ªå¿å¡«éç½®ï¼å¯åå¾
+[ãå¤§å«éå¼æ¾å¹³å°ã](https://open.miyoushe.com/#/login)(ID:
 `OpenVilla`)ç³è¯·ï¼åå¾ä»¥ä¸éç½®ï¼ - `bot_id`:
-æºå¨äººidï¼ä»¥`bot_`å¼å¤´ - `bot_secret`: æºå¨äººå¯é¥ - `callback_url`:
-httpåè°å°å endpointï¼ä¾å¦ç³è¯·botæ¶ç»çåè°å°åæ¯`http://
-åå/your/callback/url`ï¼é£ä¹éç½®éç`callback_url`å¡«å`/your/
-callback/url` ä¾å¦ï¼ ```dotenv VILLA_BOTS=' [ { "bot_id": "bot_123456789",
-"bot_secret": "abc123def456", "callback_url": "/your/callback/url" } ] ' ``` >
-æ³¨æï¼å½åå¤§å«éåªè½æ¥æ¶å°æ@Bot
+æºå¨äººidï¼ä»¥`bot_`å¼å¤´ - `bot_secret`: æºå¨äººå¯é¥ - `pub_key`:
+å å¯åéªè¯æéçpub_key - `callback_url`: httpåè°å°å
+endpointï¼ä¾å¦ç³è¯·botæ¶ç»çåè°å°åæ¯`http://åå/your/callback/
+url`ï¼é£ä¹éç½®éç`callback_url`å¡«å`/your/callback/url`
+æ­¤å¤è¿æä»¥ä¸éå¡«éç½®ï¼ -
+`verify_event`ï¼æ¯å¦å¯¹åè°äºä»¶ç­¾åè¿è¡éªè¯ ä¾å¦ï¼ ```dotenv
+VILLA_BOTS=' [ { "bot_id": "bot_123456789", "bot_secret": "abc123def456",
+"pub_key": "-----BEGIN PUBLIC KEY-----\nyour_pub_key\n-----END PUBLIC KEY-----
+\n", "callback_url": "/your/callback/url", "verify_event": true } ] ' ``` ##
+å·²æ¯ææ¶æ¯æ®µ > æ³¨æï¼å½åå¤§å«éåªè½æ¥æ¶å°æ@Bot
 (å¨åªä¸ªä½ç½®çå¯)çæ¶æ¯äºä»¶ï¼ä¸ä¸è½æå¤ä¸ª@
-(å³ä½¿æ¯@ä¸¤æ¬¡Boté½ä¸è¡) ## å·²æ¯ææ¶æ¯æ®µ - `MessageSegment.text`:
-çº¯ææ¬ + ç±³æ¸¸ç¤¾èªå¸¦è¡¨æä¹æ¯ç¨textæ¥åéï¼ä»¥
+(å³ä½¿æ¯@ä¸¤æ¬¡Boté½ä¸è¡) - `MessageSegment.text`: çº¯ææ¬ +
+ç±³æ¸¸ç¤¾èªå¸¦è¡¨æä¹æ¯ç¨textæ¥åéï¼ä»¥
 [è¡¨æå]æ ¼å¼ï¼ä¾å¦MessageSegment.text("[ç±å¿]") -
 `MessageSegment.mention_robot`: @æºå¨äºº - `MessageSegment.mention_user`:
-@ç¨æ· - `MessageSegment.mention_all`: @å¨ä½æå -
-`MessageSegment.room_link`: #æ¿é´è·³è½¬é¾æ¥ - `MessageSegment.link`:
-è¶é¾æ¥ +
+@ç¨æ· +
+`user_name`å`villa_id`å¿é¡»ç»åºå¶ä¸­ä¹ä¸ï¼ç»`villa_id`æ¶ï¼è°ç¨apiæ¥è·åç¨æ·å
+- `MessageSegment.mention_all`: @å¨ä½æå - `MessageSegment.room_link`:
+#æ¿é´è·³è½¬é¾æ¥ - `MessageSegment.link`: è¶é¾æ¥ +
 ä½¿ç¨linkçè¯é¾æ¥è½å¤ç¹å»è¿è¡è·³è½¬ï¼ä½¿ç¨textçè¯ä¸è½ç¹å» +
 å­æ®µ`show_text`æ¯æé¾æ¥æ¾ç¤ºçæå­ï¼ä½è¥æå®äºè¯¥å­æ®µï¼Webç«¯å¤§å«éä¼æ æ³æ­£å¸¸è·³è½¬
 +
 å­æ®µ`requires_bot_access_token`ä¸ºtrueæ¶ï¼è·³è½¬é¾æ¥ä¼å¸¦ä¸å«æç¨æ·ä¿¡æ¯çtoken
 - `MessageSegment.quote`: å¼ç¨(åå¤)æ¶æ¯ +
 ä¸è½**åç¬**ä½¿ç¨ï¼è¦ä¸å¶ä»æ¶æ¯æ®µä¸èµ·ä½¿ç¨ -
 `MessageSegment.image`: URLå¾ç + ææ¶åªæ¯æurlå¾ç +
```

