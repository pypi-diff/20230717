# Comparing `tmp/nonebot_plugin_rauthman-2.0.0rc1.post1.tar.gz` & `tmp/nonebot_plugin_rauthman-2.0.0rc1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rauthman-2.0.0rc1.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_rauthman-2.0.0rc1.post2.tar", max compression
```

## Comparing `nonebot_plugin_rauthman-2.0.0rc1.post1.tar` & `nonebot_plugin_rauthman-2.0.0rc1.post2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    35823 2022-07-25 20:59:00.187265 nonebot_plugin_rauthman-2.0.0rc1.post1/LICENSE
--rw-r--r--   0        0        0      249 2022-07-25 20:59:00.191254 nonebot_plugin_rauthman-2.0.0rc1.post1/nonebot_plugin_rauthman/__init__.py
--rw-r--r--   0        0        0    33986 2022-10-04 17:31:09.513487 nonebot_plugin_rauthman-2.0.0rc1.post1/nonebot_plugin_rauthman/_FileStation.py
--rw-r--r--   0        0        0    21359 2022-10-04 17:31:09.512480 nonebot_plugin_rauthman-2.0.0rc1.post1/nonebot_plugin_rauthman/RAM.py
--rw-r--r--   0        0        0      691 2023-01-23 04:29:29.308916 nonebot_plugin_rauthman-2.0.0rc1.post1/pyproject.toml
--rw-r--r--   0        0        0     8032 2022-10-04 17:31:09.512480 nonebot_plugin_rauthman-2.0.0rc1.post1/README.rst
--rw-r--r--   0        0        0     8882 1970-01-01 00:00:00.000000 nonebot_plugin_rauthman-2.0.0rc1.post1/setup.py
--rw-r--r--   0        0        0     8747 1970-01-01 00:00:00.000000 nonebot_plugin_rauthman-2.0.0rc1.post1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-07-25 20:59:00.187265 nonebot_plugin_rauthman-2.0.0rc1.post2/LICENSE
+-rw-r--r--   0        0        0       49 2023-07-17 12:50:48.313328 nonebot_plugin_rauthman-2.0.0rc1.post2/nonebot_plugin_rauthman/__init__.py
+-rw-r--r--   0        0        0    33786 2023-07-17 12:50:48.129589 nonebot_plugin_rauthman-2.0.0rc1.post2/nonebot_plugin_rauthman/_FileStation.py
+-rw-r--r--   0        0        0    21239 2023-07-17 12:50:47.898088 nonebot_plugin_rauthman-2.0.0rc1.post2/nonebot_plugin_rauthman/RAM.py
+-rw-r--r--   0        0        0      694 2023-07-17 12:52:32.208830 nonebot_plugin_rauthman-2.0.0rc1.post2/pyproject.toml
+-rw-r--r--   0        0        0     8032 2022-10-04 17:31:09.512480 nonebot_plugin_rauthman-2.0.0rc1.post2/README.rst
+-rw-r--r--   0        0        0     8743 1970-01-01 00:00:00.000000 nonebot_plugin_rauthman-2.0.0rc1.post2/PKG-INFO
```

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post1/LICENSE` & `nonebot_plugin_rauthman-2.0.0rc1.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post1/nonebot_plugin_rauthman/_FileStation.py` & `nonebot_plugin_rauthman-2.0.0rc1.post2/nonebot_plugin_rauthman/_FileStation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-"""
-Author       : Lancercmd
-Date         : 2021-12-07 15:34:10
-LastEditors  : Lancercmd
-LastEditTime : 2022-08-29 16:11:57
-Description  : None
-GitHub       : https://github.com/Lancercmd
-"""
 from __future__ import annotations
 
 from datetime import datetime
 from os import makedirs, remove, rename
 from pathlib import Path
 from re import sub
 from sys import getsizeof
```

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post1/nonebot_plugin_rauthman/RAM.py` & `nonebot_plugin_rauthman-2.0.0rc1.post2/nonebot_plugin_rauthman/RAM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-"""
-Author       : Lancercmd
-Date         : 2021-12-17 09:45:45
-LastEditors  : Lancercmd
-LastEditTime : 2022-10-05 01:21:22
-Description  : None
-GitHub       : https://github.com/Lancercmd
-"""
 from __future__ import annotations
 
 from dataclasses import dataclass, field, fields
 from functools import wraps
 from pathlib import Path
 from typing import Optional, Union
 
@@ -372,17 +364,15 @@
                 if int(_services[0]) > 99999999999999999999:
                     await worker.finish(f"Level too large: {_services[0]}")
                 segments = []
                 for group_id in state["group_ids"]:
                     prev = _amc.check_universal(bot, group_id)
                     _amc.set_universal(bot, group_id, level=int(_services[0]))
                     if len(state["group_ids"]) == 1:
-                        segments.append(
-                            f"群 Level {prev} => " + str(state["services"])
-                        )
+                        segments.append(f"群 Level {prev} => " + str(state["services"]))
                     else:
                         segments.append(
                             f"群 {group_id} Level {prev} => " + str(state["services"])
                         )
                 await worker.finish("\n".join(segments))
             elif _services[0] == _opt.show:
                 queue = []
@@ -551,9 +541,12 @@
     return Rule(_isInService)
 
 
 __plugin_meta__ = PluginMetadata(
     name="RAM - 基于规则的授权管理",
     description="为 Matcher 配置一条或多条 Rule 来实现功能的授权管理",
     usage=f"{config.ram_cmd} [{config.ram_add} <service>] [{config.ram_rm} <service>] [{config.ram_show}] [{config.ram_available}] [\d+]",
+    homepage="https://github.com/Lancercmd/nonebot_plugin_rauthman",
+    type="application",
+    supported_adapters={"~onebot.v11"},
     extra={"author": "Lancercmd"},
 )
```

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post1/pyproject.toml` & `nonebot_plugin_rauthman-2.0.0rc1.post2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "nonebot_plugin_rauthman"
-version = "2.0.0rc1.post1"
+version = "2.0.0rc1.post2"
 description = "Rule-based authorization manager worked with nonebot2"
 authors = ["Lancercmd <lancercmd@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 repository = "https://github.com/Lancercmd/nonebot_plugin_rauthman"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = {version = "^2.0.0rc1", extras = ["fastapi"]}
 nonebot-adapter-onebot = "^2.1.3"
 ujson = ">=4.0.2,<6.0.0"
-nonebot-plugin-apscheduler = "^0.2.0"
+nonebot-plugin-apscheduler = ">=0.2,<0.4"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.1"
-black = "^22.12.0"
+pytest = "^7.4.0"
+black = "^23.7.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post1/README.rst` & `nonebot_plugin_rauthman-2.0.0rc1.post2/README.rst`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post1/setup.py` & `nonebot_plugin_rauthman-2.0.0rc1.post2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,225 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-rauthman
+Version: 2.0.0rc1.post2
+Summary: Rule-based authorization manager worked with nonebot2
+Home-page: https://github.com/Lancercmd/nonebot_plugin_rauthman
+License: GPL-3.0-or-later
+Author: Lancercmd
+Author-email: lancercmd@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.2,<0.4)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0rc1,<3.0.0)
+Requires-Dist: ujson (>=4.0.2,<6.0.0)
+Project-URL: Repository, https://github.com/Lancercmd/nonebot_plugin_rauthman
+Description-Content-Type: text/x-rst
 
-packages = \
-['nonebot_plugin_rauthman']
+##############################################################################
+RAM - 基于规则的授权管理器
+##############################################################################
+.. image:: https://www.oscs1024.com/platform/badge/Lancercmd/nonebot_plugin_rauthman.svg?size=small
+ :target: https://www.oscs1024.com/project/Lancercmd/nonebot_plugin_rauthman?ref=badge_small
 
-package_data = \
-{'': ['*']}
+******************************************************************************
+前言
+******************************************************************************
+| 本项目将对 PyPI 上的发行版 `nonebot-plugin-rauthman <https://pypi.org/project/nonebot-plugin-rauthman/>`_ 来源进行 deprecate 的处理。
+|
 
-install_requires = \
-['nonebot-adapter-onebot>=2.1.3,<3.0.0',
- 'nonebot-plugin-apscheduler>=0.2.0,<0.3.0',
- 'nonebot2[fastapi]>=2.0.0rc1,<3.0.0',
- 'ujson>=4.0.2,<6.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-rauthman',
-    'version': '2.0.0rc1.post1',
-    'description': 'Rule-based authorization manager worked with nonebot2',
-    'long_description': '##############################################################################\nRAM - 基于规则的授权管理器\n##############################################################################\n.. image:: https://www.oscs1024.com/platform/badge/Lancercmd/nonebot_plugin_rauthman.svg?size=small\n :target: https://www.oscs1024.com/project/Lancercmd/nonebot_plugin_rauthman?ref=badge_small\n\n******************************************************************************\n前言\n******************************************************************************\n| 本项目将对 PyPI 上的发行版 `nonebot-plugin-rauthman <https://pypi.org/project/nonebot-plugin-rauthman/>`_ 来源进行 deprecate 的处理。\n|\n\n 由于本模块的性质，未来即使提交更新也仅对本仓库进行。\n\n 正在使用的 PyPI 发行版来源也应择日改为使用本 Git 来源。\n\n| 基于 `NoneBot2 <https://github.com/nonebot/nonebot2>`_。\n\n******************************************************************************\nHighlights\n******************************************************************************\n* 为 Matcher 或 MatcherGroup 配置一条或多条 Rule 来实现功能的授权管理\n\n.. code:: python\n\n # MatcherGroup\n\n from nonebot.plugin import MatcherGroup\n\n from nonebot_plugin_rauthman import isInService\n\n workers = MatcherGroup(\n     type="message", rule=isInService("module_name", 10)\n )  # Rule 自动套用到 MatcherGroup 下所有 Matcher\n worker_1 = workers.on_regex(...)\n worker_2 = workers.on_regex(...)\n worker_3 = workers.on_regex(...)\n worker_4 = workers.on_regex(...)\n worker_5 = workers.on_regex(...)\n worker_6 = workers.on_regex(...)\n\n ...\n.. code:: python\n\n # Matcher\n\n from nonebot.plugin import on_command\n\n from nonebot_plugin_rauthman import isInService\n\n worker = on_command(\n     "test", rule=isInService("module_name_A", 10) & isInService("module_name_B", 10)\n )  # 同时满足多个 Rule 才可触发\n\n ...\n.. code:: python\n\n # Matcher\n\n from nonebot_plugin_rauthman import isInService\n from nonebot_plugin_translator import translator\n\n translator.rule.checkers.add(\n     isInService("translator", 10)\n )  # 为具名的 Matcher 附加 RuleChecker\n\n ...\n\n* 授权策略可选 ``根据可用功能`` 或 ``根据服务级别``\n* 参数可完全自定义\n\n.. code:: python\n\n class Config:\n     savedata: str = getattr(_config, "savedata", "") or ""\n     ram_policy: int = getattr(_config, "ram_policy", 0) or 0\n     ram_cmd: str = getattr(_config, "ram_cmd", "ram") or "ram"\n     ram_add: str = getattr(_config, "ram_add", "-a") or "-a"\n     ram_rm: str = getattr(_config, "ram_rm", "-r") or "-r"\n     ram_show: str = getattr(_config, "ram_show", "-s") or "-s"\n     ram_available: str = getattr(_config, "ram_available", "-v") or "-v"\n\n******************************************************************************\n开始使用\n******************************************************************************\n==============================================================================\n对于 PyPI 发行版来源\n==============================================================================\n| 建议使用 poetry\n|\n\n* 通过 poetry 添加到 NoneBot2 项目的 ``pyproject.toml``\n\n.. code:: cmd\n\n poetry add nonebot-plugin-rauthman\n\n* 也可以通过 pip 从 `PyPI <https://pypi.org/project/nonebot-plugin-rauthman/>`_ 安装\n\n.. code:: cmd\n\n pip install nonebot-plugin-rauthman\n\n* 参照下文在 NoneBot2 项目的环境文件 ``.env.*`` 中添加配置项\n\n==============================================================================\n对于 Git 来源\n==============================================================================\n| 自己看着办吧。\n\n******************************************************************************\n配置项\n******************************************************************************\n| 以下配置项皆为可选，即使不添加也可以直接使用默认值\n|\n\n.. code-block:: python\n\n # .env.prod\n savedata = Yuni/savedata  # 保存路径，相对路径，此处为保存至运行目录下的 "Yuni/savedata/" 下，默认为 ""\n ram_policy = 0  # 授权策略 0 为根据可用功能 1 为根据服务级别，默认为 0\n ram_cmd = ram  # 指令名，或者叫触发词，默认为 ram\n ram_add = -a  # 启用功能（根据可用功能），默认为 -a\n ram_rm = -r  # 禁用功能（根据可用功能），默认为 -r\n ram_show = -s  # 展示群功能状态（根据可用功能），默认为 -s\n ram_available = -v  # 展示全局可用功能（根据可用功能），默认为 -v\n\n| 为需要管理的 ``on_*`` 事件设置规则授权，示例意为将一个 ``on_command`` 事件划入一个名为 ``module_name`` 的功能，同时设置功能级别 ``1``\n|\n\n.. code:: python\n\n  from nonebot.plugin import on_command\n  from nonebot_plugin_rauthman import isInService\n\n  command = on_command("cmd", rule=isInService("module_name", 1))\n\n| 这样，群聊必须被启用了该功能，或功能级别高于 ``1`` 才会进入事件处理（取决于当前应用的授权管理应用策略）\n\n******************************************************************************\n小白案例\n******************************************************************************\n| 以 PyPI 发行版来源为例，基于以下配置文件和事件响应器\n|\n\n.. code:: python\n\n # .env.prod\n ram_cmd = 功能  # 指令名，默认为 ram\n ram_add = 开启  # 启用功能（根据可用功能），默认为 -a\n ram_rm = 关闭  # 禁用功能（根据可用功能），默认为 -r\n ram_show = 查询  # 展示群功能状态（根据可用功能），默认为 -s\n ram_available = 全局查询  # 展示全局可用功能（根据可用功能），默认为 -v\n\n.. code:: python\n\n from nonebot.plugin import on_notice\n from nonebot_plugin_rauthman import isInService\n\n notice = on_notice(rule=to_me() & isInService("戳一戳", 1))\n\n.. image:: BotTest1.jpg\n\n******************************************************************************\n常见问题\n******************************************************************************\n* 这个插件可以做到什么？\n   | RAM 可以实现对不同群，不同功能的控制\n\n* 提示群聊未注册是怎么回事？\n   | 本地 JSON 文件中不存在该群群号，则会提示为群聊未注册\n   | 进行一次授权变更操作即可生成，如 ``ram 0``\n\n* 谁可以开启/关闭功能？\n   | ``SUPERUSERS`` 在 ``.env.*`` 中定义，参考 `配置 <https://v2.nonebot.dev/docs/tutorial/configuration#env-%E6%96%87%E4%BB%B6-1>`_\n\n* 批量对群进行授权修改？\n   | 私聊 Bot 直接发送 ``ram`` 并根据提示操作\n\n* 我设置了 ``ram_policy = 1``，怎么设置群 Level？\n   | 例如在 Bot 所在群聊中发送 ``ram 10``\n   | 这样这个群的 Level 就被设定成 ``10`` 默认的 Level 为 ``0``\n\n     授权修改操作与当前授权策略无关\n\n* 如果我希望在一个群中，管理员和群主可以修改开关/设置群 Level 我该怎么办？\n   | 对源代码第 ``101`` 行进行修改\n\n.. code:: python\n\n permission: Permission = SUPERUSER  # 参考 NoneBot2 文档 - 进阶 - 权限控制\n\n******************************************************************************\n特别感谢\n******************************************************************************\n* `Mrs4s / go-cqhttp <https://github.com/Mrs4s/go-cqhttp>`_\n* `nonebot / nonebot2 <https://github.com/nonebot/nonebot2>`_\n* `Sichongzou <https://github.com/Sichongzou>`_ 对 `README.md <README.md>`_ ``小白案例`` 和 ``常见问题`` 的贡献\n\n******************************************************************************\n优化建议\n******************************************************************************\n| 如有优化建议请积极提交 Issues 或 Pull requests\n',
-    'author': 'Lancercmd',
-    'author_email': 'lancercmd@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Lancercmd/nonebot_plugin_rauthman',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+ 由于本模块的性质，未来即使提交更新也仅对本仓库进行。
 
+ 正在使用的 PyPI 发行版来源也应择日改为使用本 Git 来源。
+
+| 基于 `NoneBot2 <https://github.com/nonebot/nonebot2>`_。
+
+******************************************************************************
+Highlights
+******************************************************************************
+* 为 Matcher 或 MatcherGroup 配置一条或多条 Rule 来实现功能的授权管理
+
+.. code:: python
+
+ # MatcherGroup
+
+ from nonebot.plugin import MatcherGroup
+
+ from nonebot_plugin_rauthman import isInService
+
+ workers = MatcherGroup(
+     type="message", rule=isInService("module_name", 10)
+ )  # Rule 自动套用到 MatcherGroup 下所有 Matcher
+ worker_1 = workers.on_regex(...)
+ worker_2 = workers.on_regex(...)
+ worker_3 = workers.on_regex(...)
+ worker_4 = workers.on_regex(...)
+ worker_5 = workers.on_regex(...)
+ worker_6 = workers.on_regex(...)
+
+ ...
+.. code:: python
+
+ # Matcher
+
+ from nonebot.plugin import on_command
+
+ from nonebot_plugin_rauthman import isInService
+
+ worker = on_command(
+     "test", rule=isInService("module_name_A", 10) & isInService("module_name_B", 10)
+ )  # 同时满足多个 Rule 才可触发
+
+ ...
+.. code:: python
+
+ # Matcher
+
+ from nonebot_plugin_rauthman import isInService
+ from nonebot_plugin_translator import translator
+
+ translator.rule.checkers.add(
+     isInService("translator", 10)
+ )  # 为具名的 Matcher 附加 RuleChecker
+
+ ...
+
+* 授权策略可选 ``根据可用功能`` 或 ``根据服务级别``
+* 参数可完全自定义
+
+.. code:: python
+
+ class Config:
+     savedata: str = getattr(_config, "savedata", "") or ""
+     ram_policy: int = getattr(_config, "ram_policy", 0) or 0
+     ram_cmd: str = getattr(_config, "ram_cmd", "ram") or "ram"
+     ram_add: str = getattr(_config, "ram_add", "-a") or "-a"
+     ram_rm: str = getattr(_config, "ram_rm", "-r") or "-r"
+     ram_show: str = getattr(_config, "ram_show", "-s") or "-s"
+     ram_available: str = getattr(_config, "ram_available", "-v") or "-v"
+
+******************************************************************************
+开始使用
+******************************************************************************
+==============================================================================
+对于 PyPI 发行版来源
+==============================================================================
+| 建议使用 poetry
+|
+
+* 通过 poetry 添加到 NoneBot2 项目的 ``pyproject.toml``
+
+.. code:: cmd
+
+ poetry add nonebot-plugin-rauthman
+
+* 也可以通过 pip 从 `PyPI <https://pypi.org/project/nonebot-plugin-rauthman/>`_ 安装
+
+.. code:: cmd
+
+ pip install nonebot-plugin-rauthman
+
+* 参照下文在 NoneBot2 项目的环境文件 ``.env.*`` 中添加配置项
+
+==============================================================================
+对于 Git 来源
+==============================================================================
+| 自己看着办吧。
+
+******************************************************************************
+配置项
+******************************************************************************
+| 以下配置项皆为可选，即使不添加也可以直接使用默认值
+|
+
+.. code-block:: python
+
+ # .env.prod
+ savedata = Yuni/savedata  # 保存路径，相对路径，此处为保存至运行目录下的 "Yuni/savedata/" 下，默认为 ""
+ ram_policy = 0  # 授权策略 0 为根据可用功能 1 为根据服务级别，默认为 0
+ ram_cmd = ram  # 指令名，或者叫触发词，默认为 ram
+ ram_add = -a  # 启用功能（根据可用功能），默认为 -a
+ ram_rm = -r  # 禁用功能（根据可用功能），默认为 -r
+ ram_show = -s  # 展示群功能状态（根据可用功能），默认为 -s
+ ram_available = -v  # 展示全局可用功能（根据可用功能），默认为 -v
+
+| 为需要管理的 ``on_*`` 事件设置规则授权，示例意为将一个 ``on_command`` 事件划入一个名为 ``module_name`` 的功能，同时设置功能级别 ``1``
+|
+
+.. code:: python
+
+  from nonebot.plugin import on_command
+  from nonebot_plugin_rauthman import isInService
+
+  command = on_command("cmd", rule=isInService("module_name", 1))
+
+| 这样，群聊必须被启用了该功能，或功能级别高于 ``1`` 才会进入事件处理（取决于当前应用的授权管理应用策略）
+
+******************************************************************************
+小白案例
+******************************************************************************
+| 以 PyPI 发行版来源为例，基于以下配置文件和事件响应器
+|
+
+.. code:: python
+
+ # .env.prod
+ ram_cmd = 功能  # 指令名，默认为 ram
+ ram_add = 开启  # 启用功能（根据可用功能），默认为 -a
+ ram_rm = 关闭  # 禁用功能（根据可用功能），默认为 -r
+ ram_show = 查询  # 展示群功能状态（根据可用功能），默认为 -s
+ ram_available = 全局查询  # 展示全局可用功能（根据可用功能），默认为 -v
+
+.. code:: python
+
+ from nonebot.plugin import on_notice
+ from nonebot_plugin_rauthman import isInService
+
+ notice = on_notice(rule=to_me() & isInService("戳一戳", 1))
+
+.. image:: BotTest1.jpg
+
+******************************************************************************
+常见问题
+******************************************************************************
+* 这个插件可以做到什么？
+   | RAM 可以实现对不同群，不同功能的控制
+
+* 提示群聊未注册是怎么回事？
+   | 本地 JSON 文件中不存在该群群号，则会提示为群聊未注册
+   | 进行一次授权变更操作即可生成，如 ``ram 0``
+
+* 谁可以开启/关闭功能？
+   | ``SUPERUSERS`` 在 ``.env.*`` 中定义，参考 `配置 <https://v2.nonebot.dev/docs/tutorial/configuration#env-%E6%96%87%E4%BB%B6-1>`_
+
+* 批量对群进行授权修改？
+   | 私聊 Bot 直接发送 ``ram`` 并根据提示操作
+
+* 我设置了 ``ram_policy = 1``，怎么设置群 Level？
+   | 例如在 Bot 所在群聊中发送 ``ram 10``
+   | 这样这个群的 Level 就被设定成 ``10`` 默认的 Level 为 ``0``
+
+     授权修改操作与当前授权策略无关
+
+* 如果我希望在一个群中，管理员和群主可以修改开关/设置群 Level 我该怎么办？
+   | 对源代码第 ``101`` 行进行修改
+
+.. code:: python
+
+ permission: Permission = SUPERUSER  # 参考 NoneBot2 文档 - 进阶 - 权限控制
+
+******************************************************************************
+特别感谢
+******************************************************************************
+* `Mrs4s / go-cqhttp <https://github.com/Mrs4s/go-cqhttp>`_
+* `nonebot / nonebot2 <https://github.com/nonebot/nonebot2>`_
+* `Sichongzou <https://github.com/Sichongzou>`_ 对 `README.md <README.md>`_ ``小白案例`` 和 ``常见问题`` 的贡献
+
+******************************************************************************
+优化建议
+******************************************************************************
+| 如有优化建议请积极提交 Issues 或 Pull requests
 
-setup(**setup_kwargs)
```

