# Comparing `tmp/nonebot_plugin_learning_chat-0.2.3.tar.gz` & `tmp/nonebot_plugin_learning_chat-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_learning_chat-0.2.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_learning_chat-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_learning_chat-0.2.3.tar` & `nonebot_plugin_learning_chat-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    34523 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/LICENSE
--rw-r--r--   0        0        0     7613 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/README.md
--rw-r--r--   0        0        0     3594 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/__init__.py
--rw-r--r--   0        0        0     4484 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/config.py
--rw-r--r--   0        0        0     6587 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/genshin_word.txt
--rw-r--r--   0        0        0    30556 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/handler.py
--rw-r--r--   0        0        0     4831 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/models.py
--rw-r--r--   0        0        0    14892 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/web_api.py
--rw-r--r--   0        0        0    26485 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/web_page.py
--rw-r--r--   0        0        0      734 2023-06-10 09:10:36.972475 nonebot_plugin_learning_chat-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     8660 1970-01-01 00:00:00.000000 nonebot_plugin_learning_chat-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-17 15:47:55.707008 nonebot_plugin_learning_chat-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7613 2023-07-17 15:47:55.711008 nonebot_plugin_learning_chat-0.3.0/README.md
+-rw-r--r--   0        0        0     3707 2023-07-17 15:47:55.711008 nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/__init__.py
+-rw-r--r--   0        0        0     4544 2023-07-17 15:47:55.711008 nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/config.py
+-rw-r--r--   0        0        0     6587 2023-07-17 15:47:55.711008 nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/genshin_word.txt
+-rw-r--r--   0        0        0    30675 2023-07-17 15:47:55.711008 nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/handler.py
+-rw-r--r--   0        0        0     4831 2023-07-17 15:47:55.711008 nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/models.py
+-rw-r--r--   0        0        0    15774 2023-07-17 15:47:55.711008 nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/web_api.py
+-rw-r--r--   0        0        0    26485 2023-07-17 15:47:55.711008 nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/web_page.py
+-rw-r--r--   0        0        0      734 2023-07-17 15:47:55.711008 nonebot_plugin_learning_chat-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8660 1970-01-01 00:00:00.000000 nonebot_plugin_learning_chat-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_learning_chat-0.2.3/LICENSE` & `nonebot_plugin_learning_chat-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_learning_chat-0.2.3/README.md` & `nonebot_plugin_learning_chat-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/__init__.py` & `nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import random
 import time
 
-from nonebot import on_message, get_bot, require, logger
-from nonebot.adapters.onebot.v11 import GroupMessageEvent, GROUP, Message, ActionFailed
+from nonebot import on_message, require, logger, get_adapter
+from nonebot.adapters.onebot.v11 import GroupMessageEvent, GROUP, Message, ActionFailed, Adapter
 from nonebot.params import Arg
 from nonebot.plugin import PluginMetadata
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 from .handler import LearningChat
 from .models import ChatMessage
 from .config import config_manager, NICKNAME
@@ -76,15 +76,18 @@
 
 
 @scheduler.scheduled_job("interval", minutes=3, misfire_grace_time=5)
 async def speak_up():
     if not config_manager.config.total_enable:
         return
     try:
-        bot = get_bot()
+        bots = get_adapter(Adapter).bots
+        if len(bots) == 0:
+            return
+        bot = list(bots.values())[0]
     except ValueError:
         return
     if not (speak := await LearningChat.speak(int(bot.self_id))):
         return
     group_id, messages = speak
     for msg in messages:
         try:
```

### Comparing `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/config.py` & `nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Dict
 from pathlib import Path
-
 from pydantic import BaseModel, Field
 
 from nonebot import get_driver, logger
+from nonebot.utils import escape_tag
 from ruamel import yaml
 
 CONFIG_PATH = Path() / "data" / "learning_chat" / "learning_chat.yml"
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
 driver = get_driver()
 try:
@@ -104,12 +104,12 @@
             )
 
 
 config_manager = ChatConfigManager()
 
 
 def log_debug(command: str, info: str):
-    logger.opt(colors=True).debug(f"<u><y>[{command}]</y></u>{info}")
+    logger.opt(colors=True).debug(f"<u><y>[{command}]</y></u>{escape_tag(info)}")
 
 
 def log_info(command: str, info: str):
-    logger.opt(colors=True).info(f"<u><y>[{command}]</y></u>{info}")
+    logger.opt(colors=True).info(f"<u><y>[{command}]</y></u>{escape_tag(info)}")
```

### Comparing `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/genshin_word.txt` & `nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/genshin_word.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/handler.py` & `nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 try:
     import jieba_fast.analyse as jieba_analyse
 except ImportError:
     import jieba.analyse as jieba_analyse
 from typing import List, Union, Optional, Tuple
 from enum import IntEnum, auto
-from nonebot import get_bot
-from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment, ActionFailed
+from nonebot import get_adapter
+from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment, ActionFailed, Adapter
 from tortoise.functions import Count
 from .models import ChatBlackList, ChatContext, ChatAnswer, ChatMessage
 from .config import (
     config_manager,
     SUPERUSERS,
     NICKNAME,
     COMMAND_START,
@@ -326,15 +326,18 @@
             result_message = random.choice(result.messages)
             log_debug("群聊学习", f"➤➤将回复<m>{result_message}</m>")
             await asyncio.sleep(random.random() + 0.5)
             return [result_message]
 
     async def _ban(self, message_id: Optional[int] = None) -> bool:
         """屏蔽消息"""
-        bot = get_bot()
+        bots = get_adapter(Adapter).bots
+        if len(bots) == 0:
+            return False
+        bot = list(bots.values())[0]
         if message_id:
             if (
                 not (message := await ChatMessage.filter(message_id=message_id).first())
                 or message.message in ALL_WORDS
             ):
                 return False
             keywords = message.keywords
```

### Comparing `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/models.py` & `nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/web_api.py` & `nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/web_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import datetime
 from typing import Optional, Union
 
 from fastapi import FastAPI
 from fastapi import Header, HTTPException, Depends
 from fastapi.responses import JSONResponse, HTMLResponse, RedirectResponse
 from jose import jwt
-from nonebot import get_bot, get_app
+from nonebot import get_app, get_adapter
+from nonebot.adapters.onebot.v11 import Adapter
 from pydantic import BaseModel
 
 try:
     import jieba_fast as jieba
 except ImportError:
     import jieba
 
@@ -86,15 +87,19 @@
     @app.get(
         "/learning_chat/api/get_group_list",
         response_class=JSONResponse,
         dependencies=[authentication()],
     )
     async def get_group_list_api():
         try:
-            group_list = await get_bot().get_group_list()
+            bots = get_adapter(Adapter).bots
+            if len(bots) == 0:
+                return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
+            bot = list(bots.values())[0]
+            group_list = await bot.get_group_list()
             group_list = [
                 {
                     "label": f'{group["group_name"]}({group["group_id"]})',
                     "value": group["group_id"],
                 }
                 for group in group_list
             ]
@@ -105,15 +110,18 @@
     @app.get(
         "/learning_chat/api/chat_global_config",
         response_class=JSONResponse,
         dependencies=[authentication()],
     )
     async def get_chat_global_config():
         try:
-            bot = get_bot()
+            bots = get_adapter(Adapter).bots
+            if len(bots) == 0:
+                return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
+            bot = list(bots.values())[0]
             groups = await bot.get_group_list()
             member_list = []
             for group in groups:
                 members = await bot.get_group_member_list(group_id=group["group_id"])
                 member_list.extend(
                     [
                         {
@@ -149,15 +157,19 @@
     @app.get(
         "/learning_chat/api/chat_group_config",
         response_class=JSONResponse,
         dependencies=[authentication()],
     )
     async def get_chat_group_config(group_id: int):
         try:
-            members = await get_bot().get_group_member_list(group_id=group_id)
+            bots = get_adapter(Adapter).bots
+            if len(bots) == 0:
+                return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
+            bot = list(bots.values())[0]
+            members = await bot.get_group_member_list(group_id=group_id)
             member_list = [
                 {
                     "label": f'{member["nickname"] or member["card"]}({member["user_id"]})',
                     "value": member["user_id"],
                 }
                 for member in members
             ]
@@ -181,18 +193,22 @@
         if not data["answer_threshold_weights"]:
             return {"status": 400, "msg": "回复阈值权重不能为空，必须至少有一个数值"}
         data["break_probability"] = data["break_probability"] / 100
         data["speak_continuously_probability"] = (
             data["speak_continuously_probability"] / 100
         )
         data["speak_poke_probability"] = data["speak_poke_probability"] / 100
+        bots = get_adapter(Adapter).bots
+        if len(bots) == 0:
+            return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
+        bot = list(bots.values())[0]
         groups = (
             [{"group_id": group_id}]
             if group_id != "all"
-            else await get_bot().get_group_list()
+            else await bot.get_group_list()
         )
         for group in groups:
             config = config_manager.get_group_config(int(group["group_id"]))
             config.update(**data)
             config_manager.config.group_config[int(group["group_id"])] = config
         config_manager.save()
         return {"status": 0, "msg": "保存成功"}
```

### Comparing `nonebot_plugin_learning_chat-0.2.3/nonebot_plugin_learning_chat/web_page.py` & `nonebot_plugin_learning_chat-0.3.0/nonebot_plugin_learning_chat/web_page.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_learning_chat-0.2.3/pyproject.toml` & `nonebot_plugin_learning_chat-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_learning_chat"
-version = "0.2.3"
+version = "0.3.0"
 description = "Nonebot2 plugin to learn what your group members say."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 keywords = ["nonebot2"]
 homepage = "https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat"
 readme = "README.md"
 license = "AGPL"
```

### Comparing `nonebot_plugin_learning_chat-0.2.3/PKG-INFO` & `nonebot_plugin_learning_chat-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-learning-chat
-Version: 0.2.3
+Version: 0.3.0
 Summary: Nonebot2 plugin to learn what your group members say.
 Home-page: https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat
 License: AGPL
 Keywords: nonebot2
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-learning-chat Version: 0.2.3
+Metadata-Version: 2.1 Name: nonebot-plugin-learning-chat Version: 0.3.0
 Summary: Nonebot2 plugin to learn what your group members say. Home-page:
 https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat License: AGPL
 Keywords: nonebot2 Author: CMHopeSunshine Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

