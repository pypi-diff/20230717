# Comparing `tmp/nonebot_plugin_translator-2.0.0b4.post0.tar.gz` & `tmp/nonebot_plugin_translator-2.0.0b4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_translator-2.0.0b4.post0.tar", max compression
+gzip compressed data, was "nonebot_plugin_translator-2.0.0b4.post1.tar", max compression
```

## Comparing `nonebot_plugin_translator-2.0.0b4.post0.tar` & `nonebot_plugin_translator-2.0.0b4.post1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    35823 2022-12-25 18:39:12.996734 nonebot_plugin_translator-2.0.0b4.post0/LICENSE
--rw-r--r--   0        0        0      226 2022-12-25 18:39:12.996734 nonebot_plugin_translator-2.0.0b4.post0/nonebot_plugin_translator/__init__.py
--rw-r--r--   0        0        0    15987 2023-01-23 04:34:13.314725 nonebot_plugin_translator-2.0.0b4.post0/nonebot_plugin_translator/translator.py
--rw-r--r--   0        0        0      668 2023-01-23 04:49:18.658481 nonebot_plugin_translator-2.0.0b4.post0/pyproject.toml
--rw-r--r--   0        0        0     3795 2023-01-23 04:52:26.786650 nonebot_plugin_translator-2.0.0b4.post0/README.rst
--rw-r--r--   0        0        0     4624 1970-01-01 00:00:00.000000 nonebot_plugin_translator-2.0.0b4.post0/setup.py
--rw-r--r--   0        0        0     4614 1970-01-01 00:00:00.000000 nonebot_plugin_translator-2.0.0b4.post0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-12-25 18:39:12.996734 nonebot_plugin_translator-2.0.0b4.post1/LICENSE
+-rw-r--r--   0        0        0       26 2023-07-17 12:59:32.105124 nonebot_plugin_translator-2.0.0b4.post1/nonebot_plugin_translator/__init__.py
+-rw-r--r--   0        0        0    17871 2023-07-17 12:59:31.916261 nonebot_plugin_translator-2.0.0b4.post1/nonebot_plugin_translator/translator.py
+-rw-r--r--   0        0        0      667 2023-07-17 12:59:38.355808 nonebot_plugin_translator-2.0.0b4.post1/pyproject.toml
+-rw-r--r--   0        0        0     3795 2023-01-23 04:52:26.786650 nonebot_plugin_translator-2.0.0b4.post1/README.rst
+-rw-r--r--   0        0        0     4614 1970-01-01 00:00:00.000000 nonebot_plugin_translator-2.0.0b4.post1/PKG-INFO
```

### Comparing `nonebot_plugin_translator-2.0.0b4.post0/LICENSE` & `nonebot_plugin_translator-2.0.0b4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_translator-2.0.0b4.post0/nonebot_plugin_translator/translator.py` & `nonebot_plugin_translator-2.0.0b4.post1/nonebot_plugin_translator/translator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-"""
-Author       : Lancercmd
-Date         : 2020-12-14 13:29:38
-LastEditors  : Lancercmd
-LastEditTime : 2022-12-26 18:15:46
-Description  : None
-GitHub       : https://github.com/Lancercmd
-"""
 from binascii import b2a_base64
 from dataclasses import dataclass
 from hashlib import sha1
 from hmac import new
 from pathlib import Path
 from random import randint
 from sys import maxsize, version_info
 from time import time
 
 from aiohttp import request
 from nonebot import get_driver
 from nonebot.adapters import Event, Message, MessageTemplate
+from nonebot.adapters.onebot.v11 import Bot as OneBot_V11_Bot
 from nonebot.adapters.onebot.v11 import MessageEvent as OneBot_V11_MessageEvent
 from nonebot.exception import ActionFailed
 from nonebot.params import CommandArg
 from nonebot.plugin import MatcherGroup, PluginMetadata
 from nonebot.typing import T_State
 from nonebot.utils import logger_wrapper
 from ujson import dumps as dumpJsonS
@@ -156,51 +149,92 @@
 
 workers = MatcherGroup(type="message", block=True)
 worker1 = workers.on_command("翻译", aliases={"机翻"})
 worker2 = workers.on_command("翻译+", aliases={"机翻+", "翻译锁定", "机翻锁定"})
 
 
 @worker1.handle()
-async def _(event: OneBot_V11_MessageEvent, state: T_State, args: Message = CommandArg()):
+async def _(
+    bot: OneBot_V11_Bot,
+    event: OneBot_V11_MessageEvent,
+    state: T_State,
+    args: Message = CommandArg(),
+):
     avl = await iterAvaiLang(targets=False)
     state["avl"] = " | ".join(avl)
     state["valid"] = loadJsonS(dumpJsonS(avl))
-    _plain_text = args.extract_plain_text()
-    if _plain_text:
-        for language in avl:
-            if _plain_text.startswith(language):
-                state["Source"] = language
-                break
-            elif _plain_text.startswith("jp"):
-                state["Source"] = "ja"
-                break
-        if "Source" in state:
-            input = _plain_text.split(" ", 2)
-            avl = await iterAvaiLang(state["Source"])
-            if len(avl) == 1:
-                state["Target"] = avl[0]
-                if len(input) == 3:
-                    state["SourceText"] = input[2]
+    try:
+        if event.reply is not None:
+            reply_ev = event.reply
+            _source_text = reply_ev.message.extract_plain_text()
+            state["SourceText"] = _source_text
+            message = "正在检测语言..."
+            await bot.send(
+                event, message, reply_message=True, message_id=reply_ev.message_id
+            )
+            resp = await requestLanguageDetect(_source_text)
+            if resp[0]:
+                message = resp[1]
+                if "header" in state:
+                    message = "".join([state["header"], f"{message}"])
+                await worker1.finish(message)
+            else:
+                data = resp[1]
+                if "Error" in data:
+                    message = "\n".join(
+                        [
+                            f"<{data['Error']['Code']}> {data['Error']['Message']}",
+                            f"RequestId: {data['RequestId']}",
+                        ]
+                    )
+                    if "header" in state:
+                        message = "".join([state["header"], f"{message}"])
+                    await worker1.finish(message)
                 else:
-                    state["SourceText"] = input[1]
-            elif len(input) == 3:
-                state["Target"] = input[1]
-                state["SourceText"] = input[2]
-            elif len(input) == 2:
+                    _source = data["Lang"]
+                    state["Source"] = _source
+        else:
+            _plain_text = args.extract_plain_text()
+            if _plain_text:
                 for language in avl:
-                    if input[0] in avl:
+                    if _plain_text.startswith(language):
+                        state["Source"] = language
+                        break
+                    elif _plain_text.startswith("jp"):
+                        state["Source"] = "ja"
+                        break
+                if "Source" in state:
+                    input = _plain_text.split(" ", 2)
+                    avl = await iterAvaiLang(state["Source"])
+                    if len(avl) == 1:
+                        state["Target"] = avl[0]
+                        if len(input) == 3:
+                            state["SourceText"] = input[2]
+                        else:
+                            state["SourceText"] = input[1]
+                    elif len(input) == 3:
                         state["Target"] = input[1]
-                    else:
-                        state["SourceText"] = input[1]
-        else:
-            state["SourceText"] = _plain_text
-    message = f"请选择输入语种，可选值如下~\n{state['avl']}"
-    if "header" in state:
-        message = "".join([state["header"], f"{message}"])
-    state["prompt"] = message
+                        state["SourceText"] = input[2]
+                    elif len(input) == 2:
+                        for language in avl:
+                            if input[0] in avl:
+                                state["Target"] = input[1]
+                            else:
+                                state["SourceText"] = input[1]
+                else:
+                    state["SourceText"] = _plain_text
+            message = f"请选择输入语种，可选值如下~\n{state['avl']}"
+            if "header" in state:
+                message = "".join([state["header"], f"{message}"])
+            state["prompt"] = message
+    except ActionFailed as e:
+        log(
+            "WARNING",
+            f"ActionFailed {e.info['retcode']} {e.info['msg'].lower()} {e.info['wording']}",
+        )
 
 
 @worker1.got("Source", prompt=MessageTemplate("{prompt}"))
 async def _(event: OneBot_V11_MessageEvent, state: T_State):
     _source = str(state["Source"])
     try:
         avl: list = loadJsonS(dumpJsonS(state["valid"]))
@@ -277,15 +311,17 @@
         log(
             "WARNING",
             f"ActionFailed {e.info['retcode']} {e.info['msg'].lower()} {e.info['wording']}",
         )
 
 
 @worker2.handle()
-async def _(event: OneBot_V11_MessageEvent, state: T_State, args: Message = CommandArg()):
+async def _(
+    event: OneBot_V11_MessageEvent, state: T_State, args: Message = CommandArg()
+):
     user_id = event.get_user_id()
     try:
         if not session_pool.find(user_id):
             avl = await iterAvaiLang()
             lang = "en"
             _plain_text = args.extract_plain_text()
             if _plain_text:
@@ -317,19 +353,21 @@
                         " | ".join(avl),
                     ]
                 )
                 if "header" in state:
                     message = "".join([state["header"], f"{message}"])
                 await worker2.finish(message)
         else:
-            message = "\n".join([
-                "已恢复到翻译锁定模式的会话~",
-                "",
-                "超时会自动切出会话，请注意~",
-            ])
+            message = "\n".join(
+                [
+                    "已恢复到翻译锁定模式的会话~",
+                    "",
+                    "超时会自动切出会话，请注意~",
+                ]
+            )
             if "header" in state:
                 message = "".join([state["header"], f"{message}"])
             await worker2.send(message)
     except ActionFailed as e:
         log(
             "WARNING",
             f"ActionFailed {e.info['retcode']} {e.info['msg'].lower()} {e.info['wording']}",
@@ -349,15 +387,17 @@
                     message = "".join([state["header"], f"{message}"])
                 await worker2.finish(message)
             elif _source_text.startswith("+"):
                 _source_text = _source_text[1:]
                 avl = await iterAvaiLang()
                 if _source_text in avl:
                     session_pool.add(user_id, _source_text)
-                    message = "\n".join([f"已切换为目标语种 {_source_text}", "取决于输入语种，目标语种可能变化"])
+                    message = "\n".join(
+                        [f"已切换为目标语种 {_source_text}", "取决于输入语种，目标语种可能变化"]
+                    )
                 else:
                     message = "\n".join(
                         [
                             f"不支持的目标语种 {_source_text}",
                             "",
                             "可用的目标语种有：",
                             " | ".join(avl),
@@ -423,16 +463,19 @@
 @worker2.handle()
 async def _(event: Event) -> None:
     # fmt: off
     supported = \
         isinstance(event, OneBot_V11_MessageEvent)
     # fmt: on
     if not supported:
-        log("WARNING", "Not supported: translator")
+        log("WARNING", "Not supported")
 
 
 __plugin_meta__ = PluginMetadata(
     name="多语种翻译插件",
     description="接口来自 腾讯机器翻译 TMT",
     usage="翻译 <ilang> <olang> <text>",
+    homepage="https://github.com/Lancercmd/nonebot_plugin_translator",
+    type="application",
+    supported_adapters={"~onebot.v11"},
     extra={"author": "Lancercmd"},
 )
```

### Comparing `nonebot_plugin_translator-2.0.0b4.post0/pyproject.toml` & `nonebot_plugin_translator-2.0.0b4.post1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "nonebot_plugin_translator"
-version = "2.0.0b4.post0"
+version = "2.0.0b4.post1"
 description = "Multi language tanslator worked with nonebot2"
 authors = ["Lancercmd <lancercmd@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 repository = "https://github.com/Lancercmd/nonebot_plugin_translator"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = {version = "^2.0.0b4", extras = ["fastapi"]}
 nonebot-adapter-onebot = "^2.0.0b1"
 aiohttp = "^3.8.1"
 ujson = ">=4.3.0,<6.0.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.1"
-black = "^22.12.0"
+pytest = "^7.4.0"
+black = "^23.7.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_translator-2.0.0b4.post0/README.rst` & `nonebot_plugin_translator-2.0.0b4.post1/README.rst`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_translator-2.0.0b4.post0/setup.py` & `nonebot_plugin_translator-2.0.0b4.post1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,100 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-translator
+Version: 2.0.0b4.post1
+Summary: Multi language tanslator worked with nonebot2
+Home-page: https://github.com/Lancercmd/nonebot_plugin_translator
+License: GPL-3.0-or-later
+Author: Lancercmd
+Author-email: lancercmd@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.0.0b1,<3.0.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0b4,<3.0.0)
+Requires-Dist: ujson (>=4.3.0,<6.0.0)
+Project-URL: Repository, https://github.com/Lancercmd/nonebot_plugin_translator
+Description-Content-Type: text/x-rst
+
+##############################################################################
+多语种翻译插件
+##############################################################################
+| 基于 `NoneBot2 <https://github.com/nonebot/nonebot2>`_。
+
+******************************************************************************
+前言
+******************************************************************************
+| 接口来自 `腾讯机器翻译 TMT <https://cloud.tencent.com/product/tmt>`_ 目前使用 `签名方法 v1 <https://cloud.tencent.com/document/api/213/15692#.E4.BD.BF.E7.94.A8.E7.AD.BE.E5.90.8D.E6.96.B9.E6.B3.95-v1-.E7.9A.84.E5.85.AC.E5.85.B1.E5.8F.82.E6.95.B0>`_
+
+******************************************************************************
+准备工作
+******************************************************************************
+* 在 `云API密钥 <https://console.cloud.tencent.com/capi>`_ 新建密钥
+   取得 ``SecretId`` 和 ``SecretKey``
+* 打开 `机器翻译控制台 <https://console.cloud.tencent.com/tmt>`_ 确认是否能正常看到概览页面
+   若提示没有完成实名认证，则需要完成才能继续和正常使用
+
+******************************************************************************
+开始使用
+******************************************************************************
+| 建议使用 poetry
+|
+
+* 通过 poetry 添加到 NoneBot2 项目的 pyproject.toml
+
+.. code:: cmd
+
+ poetry add nonebot-plugin-translator
+
+* 也可以通过 pip 从 `PyPI <https://pypi.org/project/nonebot-plugin-translator/>`_ 安装
+
+.. code:: cmd
+
+ pip install nonebot-plugin-translator
+
+* 参照下文在 NoneBot2 项目的环境文件 ``.env.*`` 中添加配置项
+
+******************************************************************************
+配置项
+******************************************************************************
+| 腾讯云 API 请求的公共参数（必须）
+
+* tencentcloud_common_region ``str``
+   | `地域参数 <https://cloud.tencent.com/document/api/551/15615#.E5.9C.B0.E5.9F.9F.E5.88.97.E8.A1.A8>`_ ，用来标识希望操作哪个地域的数据
+* tencentcloud_common_secretid ``str``
+   | 在 `云API密钥 <https://console.cloud.tencent.com/capi>`_ 上申请的标识身份的 ``SecretId``，一个 ``SecretId`` 对应唯一的 ``SecretKey``
+* tencentcloud_common_secretkey ``str``
+   | 你的 ``SecretKey`` 用来生成请求签名 Signature
+
+.. code:: python
+
+ # .env.prod
+ tencentcloud_common_region = "ap-shanghai"
+ tencentcloud_common_secretid = ""
+ tencentcloud_common_secretkey = ""
+
+| 这样，就能够在 bot 所在群聊或私聊发送 ``翻译`` 或 ``翻译+`` 使用了
+|
+
+  | ``翻译+`` 是一个用于进行连续翻译的翻译锁定模式，``翻译锁定`` 是它的别名，请根据提示操作
+
+******************************************************************************
+常见问题
+******************************************************************************
+* 我确认我的安装和配置过程正确，但我发送 ``翻译`` 或 ``机翻`` 没有反应
+   | 如果在 ``.env.*`` 的 ``command_start`` 内仅设置了非空前缀，就必须在命令前加上前缀，比如 ``/翻译`` ``/翻译+``
+
+******************************************************************************
+特别感谢
+******************************************************************************
+* `Mrs4s / go-cqhttp <https://github.com/Mrs4s/go-cqhttp>`_
+* `nonebot / nonebot2 <https://github.com/nonebot/nonebot2>`_
+
+******************************************************************************
+优化建议
+******************************************************************************
+| 请积极提交 Issues 或 Pull requests
 
-packages = \
-['nonebot_plugin_translator']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.8.1,<4.0.0',
- 'nonebot-adapter-onebot>=2.0.0b1,<3.0.0',
- 'nonebot2[fastapi]>=2.0.0b4,<3.0.0',
- 'ujson>=4.3.0,<6.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-translator',
-    'version': '2.0.0b4.post0',
-    'description': 'Multi language tanslator worked with nonebot2',
-    'long_description': '##############################################################################\n多语种翻译插件\n##############################################################################\n| 基于 `NoneBot2 <https://github.com/nonebot/nonebot2>`_。\n\n******************************************************************************\n前言\n******************************************************************************\n| 接口来自 `腾讯机器翻译 TMT <https://cloud.tencent.com/product/tmt>`_ 目前使用 `签名方法 v1 <https://cloud.tencent.com/document/api/213/15692#.E4.BD.BF.E7.94.A8.E7.AD.BE.E5.90.8D.E6.96.B9.E6.B3.95-v1-.E7.9A.84.E5.85.AC.E5.85.B1.E5.8F.82.E6.95.B0>`_\n\n******************************************************************************\n准备工作\n******************************************************************************\n* 在 `云API密钥 <https://console.cloud.tencent.com/capi>`_ 新建密钥\n   取得 ``SecretId`` 和 ``SecretKey``\n* 打开 `机器翻译控制台 <https://console.cloud.tencent.com/tmt>`_ 确认是否能正常看到概览页面\n   若提示没有完成实名认证，则需要完成才能继续和正常使用\n\n******************************************************************************\n开始使用\n******************************************************************************\n| 建议使用 poetry\n|\n\n* 通过 poetry 添加到 NoneBot2 项目的 pyproject.toml\n\n.. code:: cmd\n\n poetry add nonebot-plugin-translator\n\n* 也可以通过 pip 从 `PyPI <https://pypi.org/project/nonebot-plugin-translator/>`_ 安装\n\n.. code:: cmd\n\n pip install nonebot-plugin-translator\n\n* 参照下文在 NoneBot2 项目的环境文件 ``.env.*`` 中添加配置项\n\n******************************************************************************\n配置项\n******************************************************************************\n| 腾讯云 API 请求的公共参数（必须）\n\n* tencentcloud_common_region ``str``\n   | `地域参数 <https://cloud.tencent.com/document/api/551/15615#.E5.9C.B0.E5.9F.9F.E5.88.97.E8.A1.A8>`_ ，用来标识希望操作哪个地域的数据\n* tencentcloud_common_secretid ``str``\n   | 在 `云API密钥 <https://console.cloud.tencent.com/capi>`_ 上申请的标识身份的 ``SecretId``，一个 ``SecretId`` 对应唯一的 ``SecretKey``\n* tencentcloud_common_secretkey ``str``\n   | 你的 ``SecretKey`` 用来生成请求签名 Signature\n\n.. code:: python\n\n # .env.prod\n tencentcloud_common_region = "ap-shanghai"\n tencentcloud_common_secretid = ""\n tencentcloud_common_secretkey = ""\n\n| 这样，就能够在 bot 所在群聊或私聊发送 ``翻译`` 或 ``翻译+`` 使用了\n|\n\n  | ``翻译+`` 是一个用于进行连续翻译的翻译锁定模式，``翻译锁定`` 是它的别名，请根据提示操作\n\n******************************************************************************\n常见问题\n******************************************************************************\n* 我确认我的安装和配置过程正确，但我发送 ``翻译`` 或 ``机翻`` 没有反应\n   | 如果在 ``.env.*`` 的 ``command_start`` 内仅设置了非空前缀，就必须在命令前加上前缀，比如 ``/翻译`` ``/翻译+``\n\n******************************************************************************\n特别感谢\n******************************************************************************\n* `Mrs4s / go-cqhttp <https://github.com/Mrs4s/go-cqhttp>`_\n* `nonebot / nonebot2 <https://github.com/nonebot/nonebot2>`_\n\n******************************************************************************\n优化建议\n******************************************************************************\n| 请积极提交 Issues 或 Pull requests\n',
-    'author': 'Lancercmd',
-    'author_email': 'lancercmd@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Lancercmd/nonebot_plugin_translator',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

