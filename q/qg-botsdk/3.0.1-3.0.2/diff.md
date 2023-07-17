# Comparing `tmp/qg-botsdk-3.0.1.tar.gz` & `tmp/qg-botsdk-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg-botsdk-3.0.1.tar", last modified: Tue May 23 14:40:01 2023, max compression
+gzip compressed data, was "qg-botsdk-3.0.2.tar", last modified: Mon Jul 17 06:54:03 2023, max compression
```

## Comparing `qg-botsdk-3.0.1.tar` & `qg-botsdk-3.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 14:40:01.639948 qg-botsdk-3.0.1/
--rw-rw-rw-   0        0        0     1083 2022-05-05 08:39:02.000000 qg-botsdk-3.0.1/LICENSE
--rw-rw-rw-   0        0        0     7349 2023-05-23 14:40:01.640460 qg-botsdk-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6959 2023-05-14 14:33:12.000000 qg-botsdk-3.0.1/README.md
--rw-rw-rw-   0        0        0     6763 2023-05-14 14:33:12.000000 qg-botsdk-3.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-23 14:40:01.581620 qg-botsdk-3.0.1/qg_botsdk/
--rw-rw-rw-   0        0        0     1369 2023-05-21 14:48:31.000000 qg-botsdk-3.0.1/qg_botsdk/__init__.py
--rw-rw-rw-   0        0        0    23274 2023-05-23 14:38:53.000000 qg-botsdk-3.0.1/qg_botsdk/_api_model.py
--rw-rw-rw-   0        0        0      379 2023-05-21 14:48:29.000000 qg-botsdk-3.0.1/qg_botsdk/_exception.py
--rw-rw-rw-   0        0        0      616 2023-02-05 14:08:40.000000 qg-botsdk-3.0.1/qg_botsdk/_queue.py
--rw-rw-rw-   0        0        0    24671 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/_session.py
--rw-rw-rw-   0        0        0     1465 2023-05-19 10:22:38.000000 qg-botsdk-3.0.1/qg_botsdk/_statics.py
--rw-rw-rw-   0        0        0    15501 2023-05-21 15:23:06.000000 qg-botsdk-3.0.1/qg_botsdk/_utils.py
--rw-rw-rw-   0        0        0    51004 2023-05-23 14:32:30.000000 qg-botsdk-3.0.1/qg_botsdk/api.py
--rw-rw-rw-   0        0        0    77566 2023-05-23 14:32:42.000000 qg-botsdk-3.0.1/qg_botsdk/async_api.py
--rw-rw-rw-   0        0        0     6023 2023-05-19 10:22:38.000000 qg-botsdk-3.0.1/qg_botsdk/http.py
--rw-rw-rw-   0        0        0     6926 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/logger.py
--rw-rw-rw-   0        0        0    25549 2023-05-23 14:38:53.000000 qg-botsdk-3.0.1/qg_botsdk/model.py
--rw-rw-rw-   0        0        0     5282 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/plugins.py
--rw-rw-rw-   0        0        0    29389 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/qg_bot.py
--rw-rw-rw-   0        0        0    20262 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/qg_bot_ws.py
--rw-rw-rw-   0        0        0     8524 2023-05-21 15:19:52.000000 qg-botsdk-3.0.1/qg_botsdk/session.py
--rw-rw-rw-   0        0        0     2210 2023-05-19 10:22:41.000000 qg-botsdk-3.0.1/qg_botsdk/utils.py
--rw-rw-rw-   0        0        0       23 2023-05-23 08:17:09.000000 qg-botsdk-3.0.1/qg_botsdk/version.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:40:01.617966 qg-botsdk-3.0.1/qg_botsdk.egg-info/
--rw-rw-rw-   0        0        0     7349 2023-05-23 14:40:01.000000 qg-botsdk-3.0.1/qg_botsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      740 2023-05-23 14:40:01.000000 qg-botsdk-3.0.1/qg_botsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 14:40:01.000000 qg-botsdk-3.0.1/qg_botsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-23 14:40:01.000000 qg-botsdk-3.0.1/qg_botsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-23 14:40:01.000000 qg-botsdk-3.0.1/qg_botsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      489 2023-05-23 14:40:01.643880 qg-botsdk-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      538 2023-05-13 10:50:24.000000 qg-botsdk-3.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:40:01.637808 qg-botsdk-3.0.1/test/
--rw-rw-rw-   0        0        0        0 2023-05-14 02:41:18.000000 qg-botsdk-3.0.1/test/__init__.py
--rw-rw-rw-   0        0        0     1705 2023-05-21 15:18:34.000000 qg-botsdk-3.0.1/test/_base_context.py
--rw-rw-rw-   0        0        0      368 2023-05-19 10:22:38.000000 qg-botsdk-3.0.1/test/_testing_plugin.py
--rw-rw-rw-   0        0        0      122 2023-05-19 10:22:38.000000 qg-botsdk-3.0.1/test/conftest.py
--rw-rw-rw-   0        0        0     8167 2023-05-23 14:34:02.000000 qg-botsdk-3.0.1/test/test_api.py
--rw-rw-rw-   0        0        0    16702 2023-05-21 15:22:40.000000 qg-botsdk-3.0.1/test/test_base.py
--rw-rw-rw-   0        0        0    16088 2023-05-23 14:38:53.000000 qg-botsdk-3.0.1/test/test_run.py
--rw-rw-rw-   0        0        0     8254 2023-05-21 15:38:46.000000 qg-botsdk-3.0.1/test/test_session.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:54:03.391544 qg-botsdk-3.0.2/
+-rw-rw-rw-   0        0        0     1083 2022-05-05 08:39:02.000000 qg-botsdk-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0     7310 2023-07-17 06:54:03.391544 qg-botsdk-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6959 2023-05-14 14:33:12.000000 qg-botsdk-3.0.2/README.md
+-rw-rw-rw-   0        0        0     6763 2023-05-14 14:33:12.000000 qg-botsdk-3.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-17 06:54:03.369546 qg-botsdk-3.0.2/qg_botsdk/
+-rw-rw-rw-   0        0        0     1369 2023-05-21 14:48:31.000000 qg-botsdk-3.0.2/qg_botsdk/__init__.py
+-rw-rw-rw-   0        0        0    23311 2023-07-17 06:52:26.000000 qg-botsdk-3.0.2/qg_botsdk/_api_model.py
+-rw-rw-rw-   0        0        0      379 2023-05-21 14:48:29.000000 qg-botsdk-3.0.2/qg_botsdk/_exception.py
+-rw-rw-rw-   0        0        0      616 2023-02-05 14:08:40.000000 qg-botsdk-3.0.2/qg_botsdk/_queue.py
+-rw-rw-rw-   0        0        0    25091 2023-07-17 06:52:26.000000 qg-botsdk-3.0.2/qg_botsdk/_session.py
+-rw-rw-rw-   0        0        0     1465 2023-05-19 10:22:38.000000 qg-botsdk-3.0.2/qg_botsdk/_statics.py
+-rw-rw-rw-   0        0        0    12221 2023-07-17 06:52:28.000000 qg-botsdk-3.0.2/qg_botsdk/_utils.py
+-rw-rw-rw-   0        0        0    51046 2023-07-17 06:52:26.000000 qg-botsdk-3.0.2/qg_botsdk/api.py
+-rw-rw-rw-   0        0        0    77566 2023-05-23 14:32:42.000000 qg-botsdk-3.0.2/qg_botsdk/async_api.py
+-rw-rw-rw-   0        0        0     6023 2023-05-19 10:22:38.000000 qg-botsdk-3.0.2/qg_botsdk/http.py
+-rw-rw-rw-   0        0        0     6926 2023-05-21 15:19:52.000000 qg-botsdk-3.0.2/qg_botsdk/logger.py
+-rw-rw-rw-   0        0        0    27362 2023-07-17 06:52:26.000000 qg-botsdk-3.0.2/qg_botsdk/model.py
+-rw-rw-rw-   0        0        0     5282 2023-05-21 15:19:52.000000 qg-botsdk-3.0.2/qg_botsdk/plugins.py
+-rw-rw-rw-   0        0        0    29389 2023-05-21 15:19:52.000000 qg-botsdk-3.0.2/qg_botsdk/qg_bot.py
+-rw-rw-rw-   0        0        0    20262 2023-05-21 15:19:52.000000 qg-botsdk-3.0.2/qg_botsdk/qg_bot_ws.py
+-rw-rw-rw-   0        0        0     8679 2023-05-25 10:57:52.000000 qg-botsdk-3.0.2/qg_botsdk/session.py
+-rw-rw-rw-   0        0        0     2210 2023-05-19 10:22:41.000000 qg-botsdk-3.0.2/qg_botsdk/utils.py
+-rw-rw-rw-   0        0        0       23 2023-05-23 14:42:51.000000 qg-botsdk-3.0.2/qg_botsdk/version.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:54:03.377544 qg-botsdk-3.0.2/qg_botsdk.egg-info/
+-rw-rw-rw-   0        0        0     7310 2023-07-17 06:54:03.000000 qg-botsdk-3.0.2/qg_botsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2023-07-17 06:54:03.000000 qg-botsdk-3.0.2/qg_botsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:54:03.000000 qg-botsdk-3.0.2/qg_botsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-17 06:54:03.000000 qg-botsdk-3.0.2/qg_botsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-17 06:54:03.000000 qg-botsdk-3.0.2/qg_botsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      489 2023-07-17 06:54:03.392543 qg-botsdk-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      538 2023-05-13 10:50:24.000000 qg-botsdk-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:54:03.390544 qg-botsdk-3.0.2/test/
+-rw-rw-rw-   0        0        0        0 2023-05-14 02:41:18.000000 qg-botsdk-3.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0     1705 2023-05-21 15:18:34.000000 qg-botsdk-3.0.2/test/_base_context.py
+-rw-rw-rw-   0        0        0      368 2023-05-19 10:22:38.000000 qg-botsdk-3.0.2/test/_testing_plugin.py
+-rw-rw-rw-   0        0        0      122 2023-05-19 10:22:38.000000 qg-botsdk-3.0.2/test/conftest.py
+-rw-rw-rw-   0        0        0     8167 2023-05-23 14:34:02.000000 qg-botsdk-3.0.2/test/test_api.py
+-rw-rw-rw-   0        0        0    16702 2023-05-21 15:22:40.000000 qg-botsdk-3.0.2/test/test_base.py
+-rw-rw-rw-   0        0        0    16088 2023-05-23 14:38:53.000000 qg-botsdk-3.0.2/test/test_run.py
+-rw-rw-rw-   0        0        0     8254 2023-05-21 15:38:46.000000 qg-botsdk-3.0.2/test/test_session.py
```

### Comparing `qg-botsdk-3.0.1/LICENSE` & `qg-botsdk-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/PKG-INFO` & `qg-botsdk-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: qg-botsdk
-Version: 3.0.1
+Version: 3.0.2
 Summary: easy-to-use SDK for Tencent QQ guild robot
 Home-page: https://github.com/GLGDLY/qg_botsdk
 Author: GDLY
 Author-email: tzlgdly@gmail.com
-License: UNKNOWN
 Keywords: sample,example,setuptools
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: <4,>=3.7
 License-File: LICENSE
@@ -197,8 +195,7 @@
 ========
 
 -   文档：
      * `readthedocs <https://qg-botsdk.readthedocs.io/zh_CN/latest/>`_
 -   官方注册机器人：https://q.qq.com/#/
 -   官方API文档：https://bot.q.qq.com/wiki/develop/api/
 -   SDK QQ交流群：https://jq.qq.com/?_wv=1027&k=3NnWvGpz
-
```

### Comparing `qg-botsdk-3.0.1/README.md` & `qg-botsdk-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/README.rst` & `qg-botsdk-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk/__init__.py` & `qg-botsdk-3.0.2/qg_botsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk/_api_model.py` & `qg-botsdk-3.0.2/qg_botsdk/_api_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from typing import Any, Callable, Dict, List, Optional
+from typing import Dict, List, Optional
 
-from ._utils import object_class
-from .model import BotCommandObject, Model
 
+class object_class:
+    def __init__(self, _static_copy, _data):
+        self.__dict__.update(_data)
+        self._static_copy = _static_copy
 
-class WaifForCommandCallback:
-    def __init__(
-        self, command: BotCommandObject, callback: Callable[[Model.MESSAGE], Any]
-    ):
-        self.command = command
-        self.callback = callback
+    def __doc__(self):
+        return self._static_copy
+
+    def __repr__(self):
+        return self._static_copy
+
+    @property
+    def dict(self):
+        return self._static_copy
 
 
 apis = {
     ("获取用户ID", "get_bot_id"): [False, "此API不需要请求权限"],
     ("获取用户信息", "get_bot_info"): ["GET", "/users/@me"],
     ("获取用户频道列表", "get_bot_guilds"): ["GET", "/users/@me/guilds"],
     ("获取频道详情", "get_guild_info"): ["GET", "/guilds/{guild_id}"],
```

### Comparing `qg-botsdk-3.0.1/qg_botsdk/_queue.py` & `qg-botsdk-3.0.2/qg_botsdk/_queue.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk/_session.py` & `qg-botsdk-3.0.2/qg_botsdk/_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,27 @@
 from collections import namedtuple
 from copy import deepcopy
 from threading import Thread
 from time import time
 from typing import Dict, Hashable, Iterable, List, Optional, Union
 from weakref import finalize
 
-from ._api_model import WaifForCommandCallback
 from ._statics import EVENTS
 from ._utils import exception_handler
 from .api import API
 from .async_api import AsyncAPI
 from .logger import Logger
-from .model import BotCommandObject, Model, Scope, SessionObject, SessionStatus
+from .model import (
+    BotCommandObject,
+    Model,
+    Scope,
+    SessionObject,
+    SessionStatus,
+    WaifForCommandCallback,
+)
 
 _AllScopeStr = ("USER", "GUILD", "CHANNEL", "GLOBAL")
 ScopeRegisterKey = namedtuple("ScopeRegisterKey", _AllScopeStr)
 
 
 class _SessionObject:
     def __init__(
@@ -70,14 +76,15 @@
     def __init__(
         self,
         logger: Logger,
         commit_path: Optional[str] = None,
         is_auto_commit: bool = True,
     ):
         self.__sessions: Dict = {x: {} for x in _AllScopeStr}
+        self.__sessions_pk_cache = None
         self.__wait_for_registers: Dict = {}
         self.__logger: Logger = logger
         self.__bot_identify: str = logger.bot_app_id
         self.__commit_path: str = commit_path or os.path.join(
             os.getcwd(), "session_data"
         )
         self.__check_path(self.__commit_path)
@@ -189,16 +196,22 @@
                                 gc_identifies.append(identify)
                         for identify in gc_identifies:
                             del sessions[identify]
                             change = True
             except Exception as e:
                 self.__logger.error(e.__repr__())
                 self.__logger.error(exception_handler(e))
-            if change and self.__is_auto_commit:
-                self.commit_data(is_info=False)
+            if self.__is_auto_commit:
+                if change:
+                    self.commit_data(is_info=False)
+                else:
+                    _new_pk_data = pickle.dumps(self.__sessions)
+                    if self.__sessions_pk_cache != _new_pk_data:
+                        self.__sessions_pk_cache = _new_pk_data
+                        self.commit_data(is_info=False, pk_data=_new_pk_data)
 
     @staticmethod
     def __valid_scope(scope):
         if isinstance(scope, Scope):
             scope = scope.value
         elif scope in _AllScopeStr:
             pass
@@ -503,20 +516,21 @@
                                         f"Session Manager 读取 Scope::{scope}::{_id}::{k} 数据时出现错误，将跳过：{repr(e)}"
                                     )
             if is_info:
                 self.__logger.info(f"Session Manager 读取了 {self.__commit_path} 的数据")
         except Exception as e:
             self.__logger.error(f"Session Manager 读取 {_path} 时出现错误，将跳过：{repr(e)}")
 
-    def commit_data(self, is_info: bool = True):
+    def commit_data(self, is_info: bool = True, pk_data: Optional[bytes] = None):
         _path = os.path.join(self.__commit_path, f"session_{self.__bot_identify}.db")
         try:
-            # print(dill.dumps(self.__sessions["USER"]))
             with open(_path, "wb") as f_db:
-                f_db.write(pickle.dumps(self.__sessions))
+                if not pk_data:
+                    pk_data = pickle.dumps(self.__sessions)
+                f_db.write(pk_data)
             if is_info:
                 self.__logger.info(f"Session Manager 写入了 {_path} 的数据")
         except Exception as e:
             self.__logger.error(f"Session Manager 写入 {_path} 时出现错误，将跳过：{repr(e)}")
 
     def set_auto_commit(self, is_auto_commit: bool):
         self.__is_auto_commit = is_auto_commit
```

### Comparing `qg-botsdk-3.0.1/qg_botsdk/_statics.py` & `qg-botsdk-3.0.2/qg_botsdk/_statics.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk/_utils.py` & `qg-botsdk-3.0.2/qg_botsdk/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from asyncio import iscoroutinefunction
-from copy import deepcopy
 from functools import wraps
 from inspect import Signature, signature, stack
 from json import dumps, loads
 from json.decoder import JSONDecodeError
 from sys import exc_info
 from time import localtime, strftime
 from traceback import extract_tb
 from typing import BinaryIO, Callable, Dict, Iterable, Optional, Union
 
 from aiohttp import ContentTypeError
 
+from ._api_model import object_class, send_msg
 from .version import __version__
 
 general_header = {"User-Agent": f"qg-botsdk v{__version__}"}
 security_header = {
     "Content-Type": "application/json",
     "charset": "UTF-8",
     "User-Agent": f"qg-botsdk v{__version__}",
@@ -54,136 +54,14 @@
     "FORUM_POST_CREATE",
     "FORUM_POST_DELETE",
     "FORUM_REPLY_CREATE",
     "FORUM_REPLY_DELETE",
     "INTERACTION_CREATE",
 )
 
-
-def template_wrapper(func):
-    @wraps(func)
-    async def wrap(*args):
-        try:
-            result = await func(*args)
-            return result
-        except (JSONDecodeError, ContentTypeError, AttributeError, KeyError):
-            return_ = args[0]
-            code = (
-                return_.status_code
-                if hasattr(return_, "status_code")
-                else getattr(return_, "status", None)
-            )
-            trace_id = getattr(return_, "headers", {}).get("X-Tps-Trace-Id")
-            return objectize(
-                {"data": None, "trace_id": trace_id, "http_code": code, "result": False}
-            )
-
-    return wrap
-
-
-def security_wrapper(func):
-    @wraps(func)
-    def wrap(*args, **kwargs):
-        try:
-            return func(*args, **kwargs)
-        except (JSONDecodeError, KeyError, AttributeError) as e:
-            name = func.__name__
-            logger = getattr(args[0], "logger", None)
-            if name == "__security_check_code":
-                if logger:
-                    logger.error("无法调用内容安全检测接口（备注：请检查机器人密钥是否正确）")
-            else:
-                if logger:
-                    logger.error(f"调用内容安全检测接口失败，详情：{exception_handler(e)}")
-                return False
-
-    return wrap
-
-
-def stack_exception_handler(error, stack_no: int = 1):
-    target_frame = stack()[stack_no]
-    return '[error:{}] File "{}", line {}, in {}'.format(
-        error.__repr__(),
-        target_frame.filename,
-        target_frame.lineno,
-        target_frame.function,
-    )
-
-
-def exception_handler(error):
-    error_info = extract_tb(exc_info()[-1])[-1]
-    return '[error:{}] File "{}", line {}, in {}'.format(
-        error.__repr__(), *error_info[:3]
-    )
-
-
-def exception_processor(func):
-    @wraps(func)
-    def wrap(*args, **kwargs):
-        try:
-            return func(*args, **kwargs)
-        except Exception as e:
-            logger = getattr(args[0], "logger", None)
-            if logger:
-                logger.error(e.__repr__())
-                logger.error(exception_handler(e))
-            else:
-                t = strftime("%m-%d %H:%M:%S", localtime())
-                print(f"\033[1;31m[{t}] [ERROR]\033[0m {e.__repr__()}")
-                print(f"[{t}] [ERROR] {exception_handler(e)}")
-
-    return wrap
-
-
-class object_class:
-    def __init__(self, **kwargs):
-        for k, v in kwargs.items():
-            self.__setattr__(k, v)
-
-    def __getattribute__(self, item):
-        if item == "__doc__":
-            return object.__getattribute__(self, "__repr__")()
-        return object.__getattribute__(self, item)
-
-    def __repr__(self):
-        try:
-            return dumps(self._data)
-        except (TypeError, ValueError):
-            return str(self._data)
-
-    @property
-    def dict(self):
-        return self._data
-
-
-def _send_msg():  # Cannot direct import from _api_model.py since circular import
-    class SendMsg(object_class):
-        class data:
-            id: str
-            channel_id: str
-            guild_id: str
-            content: str
-            timestamp: str
-            tts: bool
-            mention_everyone: bool
-            author: Dict
-            pinned: bool
-            type: int
-            flags: int
-            seq_in_channel: str
-            code: int
-            message: str
-
-        http_code: int
-        trace_id: str
-        result: bool
-
-    return SendMsg
-
-
 _reply_args = (
     "content",
     "image",
     "file_image",
     "message_reference_id",
     "ignore_message_reference_error",
 )
@@ -193,31 +71,15 @@
     def reply(
         self,
         content: Optional[str] = None,
         image: Optional[str] = None,
         file_image: Optional[Union[bytes, BinaryIO, str]] = None,
         message_reference_id: Optional[str] = None,
         ignore_message_reference_error: Optional[bool] = None,
-    ) -> _send_msg():
-        """
-        目前支持reply()发送被动消息的事件类型有:
-
-        GUILD_MEMBER_ADD GUILD_MEMBER_UPDATE GUILD_MEMBER_REMOVE MESSAGE_REACTION_ADD MESSAGE_REACTION_REMOVE
-        FORUM_THREAD_CREATE FORUM_THREAD_UPDATE FORUM_THREAD_DELETE FORUM_POST_CREATE FORUM_POST_DELETE
-        FORUM_REPLY_CREATE FORUM_REPLY_DELETE INTERACTION_CREATE
-
-        剩余事件的reply()将会转为发送主动消息
-
-        :param content: 消息文本（选填，此项与image至少需要有一个字段，否则无法下发消息）
-        :param image: 图片url，不可发送本地图片（选填，此项与msg至少需要有一个字段，否则无法下发消息）
-        :param file_image: 本地图片，可选三种方式传参，具体可参阅github中的example_10或帮助文档
-        :param message_reference_id: 引用消息的id（选填）
-        :param ignore_message_reference_error: 是否忽略获取引用消息详情错误，默认否（选填）
-        :return: 返回的.data中为解析后的json数据
-        """
+    ) -> send_msg():
         raw_args = locals()
         kwargs = {arg: raw_args[arg] for arg in _reply_args}
         t = getattr(self, "t", None)
         if t in msg_t:
             kwargs["message_id"] = getattr(self, "id", None)
         elif t in event_t:
             kwargs["message_id"] = getattr(self, "event_id", None)
@@ -237,31 +99,15 @@
     async def reply(
         self,
         content: Optional[str] = None,
         image: Optional[str] = None,
         file_image: Optional[Union[bytes, BinaryIO, str]] = None,
         message_reference_id: Optional[str] = None,
         ignore_message_reference_error: Optional[bool] = None,
-    ) -> _send_msg():
-        """
-        目前支持reply()发送被动消息的事件类型有:
-
-        GUILD_MEMBER_ADD GUILD_MEMBER_UPDATE GUILD_MEMBER_REMOVE MESSAGE_REACTION_ADD MESSAGE_REACTION_REMOVE
-        FORUM_THREAD_CREATE FORUM_THREAD_UPDATE FORUM_THREAD_DELETE FORUM_POST_CREATE FORUM_POST_DELETE
-        FORUM_REPLY_CREATE FORUM_REPLY_DELETE INTERACTION_CREATE
-
-        剩余事件的reply()将会转为发送主动消息
-
-        :param content: 消息文本（选填，此项与image至少需要有一个字段，否则无法下发消息）
-        :param image: 图片url，不可发送本地图片（选填，此项与msg至少需要有一个字段，否则无法下发消息）
-        :param file_image: 本地图片，可选三种方式传参，具体可参阅github中的example_10或帮助文档
-        :param message_reference_id: 引用消息的id（选填）
-        :param ignore_message_reference_error: 是否忽略获取引用消息详情错误，默认否（选填）
-        :return: 返回的.data中为解析后的json数据
-        """
+    ) -> send_msg():
         raw_args = locals()
         kwargs = {arg: raw_args[arg] for arg in _reply_args}
         t = getattr(self, "t", None)
         if t in msg_t:
             kwargs["message_id"] = getattr(self, "id", None)
         elif t in event_t:
             kwargs["message_id"] = getattr(self, "event_id", None)
@@ -274,42 +120,120 @@
                 if hasattr(self, "channel_id")
                 else getattr(self, "id", None)
             )
             return await getattr(self, "api").send_msg(**kwargs)
 
 
 def objectize(
-    data, api=None, is_async=False, is_recursion=False
+    data, api=None, is_async=False
 ):  # if api is not None, the event is a resp class
     if isinstance(data, dict):
-        _data = data
-        if not is_recursion:
-            # create a copy that doesn't reference to the original data
-            data = deepcopy(data)
+        try:
+            _static_copy = dumps(data)
+        except (TypeError, JSONDecodeError):
+            _static_copy = str(data)
         # main func to process data
         for keys, values in data.items():
             if keys.isnumeric():
                 return data
             if isinstance(values, dict):
-                data[keys] = objectize(values, is_recursion=True)
+                data[keys] = objectize(values)
             elif isinstance(values, list):
                 for i, items in enumerate(values):
                     if isinstance(items, dict):
-                        data[keys][i] = objectize(items, is_recursion=True)
-        data["_data"] = _data
+                        data[keys][i] = objectize(items)
         if api:
             data["api"] = api
-            object_data = async_event_class(**data) if is_async else event_class(**data)
+            object_data = (
+                async_event_class(_static_copy, data)
+                if is_async
+                else event_class(_static_copy, data)
+            )
         else:
-            object_data = object_class(**data)
+            object_data = object_class(_static_copy, data)
         return object_data
     else:
         return data
 
 
+def template_wrapper(func):
+    @wraps(func)
+    async def wrap(*args):
+        try:
+            result = await func(*args)
+            return result
+        except (JSONDecodeError, ContentTypeError, AttributeError, KeyError):
+            return_ = args[0]
+            code = (
+                return_.status_code
+                if hasattr(return_, "status_code")
+                else getattr(return_, "status", None)
+            )
+            trace_id = getattr(return_, "headers", {}).get("X-Tps-Trace-Id")
+            return objectize(
+                {"data": None, "trace_id": trace_id, "http_code": code, "result": False}
+            )
+
+    return wrap
+
+
+def security_wrapper(func):
+    @wraps(func)
+    def wrap(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except (JSONDecodeError, KeyError, AttributeError) as e:
+            name = func.__name__
+            logger = getattr(args[0], "logger", None)
+            if name == "__security_check_code":
+                if logger:
+                    logger.error("无法调用内容安全检测接口（备注：请检查机器人密钥是否正确）")
+            else:
+                if logger:
+                    logger.error(f"调用内容安全检测接口失败，详情：{exception_handler(e)}")
+                return False
+
+    return wrap
+
+
+def stack_exception_handler(error, stack_no: int = 1):
+    target_frame = stack()[stack_no]
+    return '[error:{}] File "{}", line {}, in {}'.format(
+        error.__repr__(),
+        target_frame.filename,
+        target_frame.lineno,
+        target_frame.function,
+    )
+
+
+def exception_handler(error):
+    error_info = extract_tb(exc_info()[-1])[-1]
+    return '[error:{}] File "{}", line {}, in {}'.format(
+        error.__repr__(), *error_info[:3]
+    )
+
+
+def exception_processor(func):
+    @wraps(func)
+    def wrap(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except Exception as e:
+            logger = getattr(args[0], "logger", None)
+            if logger:
+                logger.error(e.__repr__())
+                logger.error(exception_handler(e))
+            else:
+                t = strftime("%m-%d %H:%M:%S", localtime())
+                print(f"\033[1;31m[{t}] [ERROR]\033[0m {e.__repr__()}")
+                print(f"[{t}] [ERROR] {exception_handler(e)}")
+
+    return wrap
+
+
 def treat_msg(raw_msg: str, at: str):
     raw_msg = raw_msg if raw_msg.find(at) else raw_msg.replace(at, "", 1).strip()
     if not raw_msg:
         return ""
     if raw_msg[0] == "/":
         raw_msg = raw_msg[1:]
     return (
```

### Comparing `qg-botsdk-3.0.1/qg_botsdk/api.py` & `qg-botsdk-3.0.2/qg_botsdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -823,16 +823,16 @@
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.delete_dm_msg(**_args), self._loop)
         return future_.result(timeout=self._timeout)
 
     def mute_all_member(
         self,
         guild_id: str,
-        mute_end_timestamp: Optional[str],
-        mute_seconds: Optional[str],
+        mute_end_timestamp: Optional[str] = None,
+        mute_seconds: Optional[str] = None,
     ) -> _api_model.mute_member():
         """
         用于将频道的全体成员（非管理员）禁言
 
         :param guild_id: 频道id
         :param mute_end_timestamp: 禁言到期时间戳，绝对时间戳，单位：秒（与 mute_seconds 字段同时赋值的话，以该字段为准）
         :param mute_seconds: 禁言多少秒（两个字段二选一，默认以 mute_end_timestamp 为准）
@@ -846,16 +846,16 @@
         )
         return future_.result(timeout=self._timeout)
 
     def mute_member(
         self,
         guild_id: str,
         user_id: str,
-        mute_end_timestamp: Optional[str],
-        mute_seconds: Optional[str],
+        mute_end_timestamp: Optional[str] = None,
+        mute_seconds: Optional[str] = None,
     ) -> _api_model.mute_member():
         """
         用于禁言频道 guild_id 下的成员 user_id
 
         :param guild_id: 频道id
         :param user_id: 目标成员的用户ID
         :param mute_end_timestamp: 禁言到期时间戳，绝对时间戳，单位：秒（与 mute_seconds 字段同时赋值的话，以该字段为准）
@@ -868,16 +868,16 @@
         future_ = run_coroutine_threadsafe(self._api.mute_member(**_args), self._loop)
         return future_.result(timeout=self._timeout)
 
     def mute_members(
         self,
         guild_id: str,
         user_id: List[str],
-        mute_end_timestamp: Optional[str],
-        mute_seconds: Optional[str],
+        mute_end_timestamp: Optional[str] = None,
+        mute_seconds: Optional[str] = None,
     ) -> _api_model.mute_members():
         """
         用于将频道的指定批量成员（非管理员）禁言
 
         :param guild_id: 频道id
         :param user_id: 目标成员的用户ID列表
         :param mute_end_timestamp: 禁言到期时间戳，绝对时间戳，单位：秒（与 mute_seconds 字段同时赋值的话，以该字段为准）
```

### Comparing `qg-botsdk-3.0.1/qg_botsdk/async_api.py` & `qg-botsdk-3.0.2/qg_botsdk/async_api.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk/http.py` & `qg-botsdk-3.0.2/qg_botsdk/http.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk/logger.py` & `qg-botsdk-3.0.2/qg_botsdk/logger.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk/model.py` & `qg-botsdk-3.0.2/qg_botsdk/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,65 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from enum import Enum
 from re import Pattern
 from re import compile as re_compile
-from typing import Any, Callable, Dict, Hashable, Iterable, List, Optional, Tuple, Union
+from typing import (
+    Any,
+    BinaryIO,
+    Callable,
+    Dict,
+    Hashable,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
 
-from ._utils import event_class
+from ._api_model import send_msg
+
+
+class _AbstractEventClass:
+    def reply(
+        self,
+        content: Optional[str] = None,
+        image: Optional[str] = None,
+        file_image: Optional[Union[bytes, BinaryIO, str]] = None,
+        message_reference_id: Optional[str] = None,
+        ignore_message_reference_error: Optional[bool] = None,
+    ) -> send_msg():
+        """
+        目前支持reply()发送被动消息的事件类型有:
+
+        GUILD_MEMBER_ADD GUILD_MEMBER_UPDATE GUILD_MEMBER_REMOVE MESSAGE_REACTION_ADD MESSAGE_REACTION_REMOVE
+        FORUM_THREAD_CREATE FORUM_THREAD_UPDATE FORUM_THREAD_DELETE FORUM_POST_CREATE FORUM_POST_DELETE
+        FORUM_REPLY_CREATE FORUM_REPLY_DELETE INTERACTION_CREATE
+
+        剩余事件的reply()将会转为发送主动消息
+
+        :param content: 消息文本（选填，此项与image至少需要有一个字段，否则无法下发消息）
+        :param image: 图片url，不可发送本地图片（选填，此项与msg至少需要有一个字段，否则无法下发消息）
+        :param file_image: 本地图片，可选三种方式传参，具体可参阅github中的example_10或帮助文档
+        :param message_reference_id: 引用消息的id（选填）
+        :param ignore_message_reference_error: 是否忽略获取引用消息详情错误，默认否（选填）
+        :return: 返回的.data中为解析后的json数据
+        """
+        ...
 
 
 class Model:
     """
     使用此Model库可用作验证事件数据的准确性，目前可用的模型如下：
 
     GUILDS - 频道事件
     GUILD_MEMBERS -
     """
 
-    class GUILDS(event_class):
+    class GUILDS(_AbstractEventClass):
         """
         频道事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - GUILD_CREATE - 当机器人加入新guild时
         - GUILD_UPDATE - 当guild资料发生变更时
         - GUILD_DELETE - 当机器人退出guild时
 
@@ -37,15 +76,15 @@
         member_count: int
         name: str
         op_user_id: str
         owner_id: str
         t: str
         event_id: str
 
-    class CHANNELS(event_class):
+    class CHANNELS(_AbstractEventClass):
         """
         子频道事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - CHANNEL_CREATE - 当channel被创建时
         - CHANNEL_UPDATE - 当channel被更新时
         - CHANNEL_DELETE - 当channel被删除时
 
@@ -66,15 +105,15 @@
         private_type: int
         speak_permission: int
         sub_type: int
         type: int
         t: str
         event_id: str
 
-    class GUILD_MEMBERS(event_class):
+    class GUILD_MEMBERS(_AbstractEventClass):
         """
         频道成员事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - GUILD_MEMBER_ADD - 当成员加入时
         - GUILD_MEMBER_UPDATE - 当成员资料变更时
         - GUILD_MEMBER_REMOVE - 当成员被移除时
 
@@ -93,15 +132,15 @@
         joined_at: str
         nick: str
         op_user_id: str
         roles: List[str]
         t: str
         event_id: str
 
-    class MESSAGE(event_class):
+    class MESSAGE(_AbstractEventClass):
         """
         消息事件的数据模，可从t字段判断具体事件，其中包含：
 
         - MESSAGE_CREATE - 发送消息事件，代表频道内的全部消息，而不只是 at 机器人的消息
         - AT_MESSAGE_CREATE - 当收到@机器人的消息时
 
         .. note::
@@ -154,15 +193,15 @@
         pinned: bool
         type: int
         flags: int
         treated_msg: Union[str, Tuple]
         t: str
         event_id: str
 
-    class MESSAGE_DELETE(event_class):
+    class MESSAGE_DELETE(_AbstractEventClass):
         """
         消息撤回事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - MESSAGE_DELETE - 删除（撤回）消息事件
         - PUBLIC_MESSAGE_DELETE - 当频道的消息被删除时
         - DIRECT_MESSAGE_DELETE - 删除（撤回）私信消息事件
 
@@ -186,15 +225,15 @@
 
         class op_user:
             id: str
 
         t: str
         event_id: str
 
-    class DIRECT_MESSAGE(event_class):
+    class DIRECT_MESSAGE(_AbstractEventClass):
         """
         私信消息事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - DIRECT_MESSAGE_CREATE - 当收到用户发给机器人的私信消息时
 
         .. seealso::
              其子字段数据可参阅：
@@ -231,15 +270,15 @@
         seq_in_channel: str
         src_guild_id: str
         timestamp: str
         treated_msg: str
         t: str
         event_id: str
 
-    class MESSAGE_AUDIT(event_class):
+    class MESSAGE_AUDIT(_AbstractEventClass):
         """
         主动消息审核事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - MESSAGE_AUDIT_PASS - 消息审核通过
         - MESSAGE_AUDIT_REJECT - 消息审核不通过
 
         .. note::
@@ -255,15 +294,15 @@
         create_time: str
         channel_id: str
         guild_id: str
         message_id: str
         t: str
         event_id: str
 
-    class FORUMS_EVENT(event_class):
+    class FORUMS_EVENT(_AbstractEventClass):
         """
         论坛事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - FORUM_THREAD_CREATE - 当用户创建主题（帖子）时
         - FORUM_THREAD_UPDATE - 当用户更新主题（帖子）时
         - FORUM_THREAD_DELETE - 当用户删除主题（帖子）时
 
@@ -343,15 +382,15 @@
 
         guild_id: str
         channel_id: str
         author_id: str
         t: str
         event_id: str
 
-    class OPEN_FORUMS(event_class):
+    class OPEN_FORUMS(_AbstractEventClass):
         """
         公域论坛事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - OPEN_FORUM_THREAD_CREATE - 当用户创建主题（帖子）时
         - OPEN_FORUM_THREAD_UPDATE - 当用户更新主题（帖子）时
         - OPEN_FORUM_THREAD_DELETE - 当用户删除主题（帖子）时
 
@@ -364,15 +403,15 @@
 
         guild_id: str
         channel_id: str
         author_id: str
         t: str
         event_id: str
 
-    class AUDIO_ACTION(event_class):
+    class AUDIO_ACTION(_AbstractEventClass):
         """
         音频事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - AUDIO_START - 音频开始播放时
         - AUDIO_FINISH - 音频播放结束时
         - AUDIO_ON_MIC - 上麦时
         - AUDIO_OFF_MIC - 下麦时
@@ -388,15 +427,15 @@
         channel_id: str
         guild_id: str
         audio_url: str
         text: str
         t: str
         event_id: str
 
-    class REACTION(event_class):
+    class REACTION(_AbstractEventClass):
         """
         表情表态事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - MESSAGE_REACTION_ADD - 为消息添加表情表态
         - MESSAGE_REACTION_REMOVE - 为消息删除表情表态
 
         .. seealso::
@@ -414,15 +453,15 @@
 
         user_id: str
         channel_id: str
         guild_id: str
         t: str
         event_id: str
 
-    class INTERACTION(event_class):
+    class INTERACTION(_AbstractEventClass):
         """
         互动事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - INTERACTION_CREATE - 互动事件创建时
 
         .. seealso::
              其子字段数据可参阅：
@@ -443,15 +482,15 @@
         guild_id: str
         id: str
         type: int
         version: int
         t: str
         event_id: str
 
-    class LIVE_CHANNEL_MEMBER(event_class):
+    class LIVE_CHANNEL_MEMBER(_AbstractEventClass):
         """
         音视频/直播子频道成员进出事件的数据模型，可从t字段判断具体事件，其中包含：
 
         - AUDIO_OR_LIVE_CHANNEL_MEMBER_ENTER - 当用户进入音视频/直播子频道
         - AUDIO_OR_LIVE_CHANNEL_MEMBER_EXIT - 当用户离开音视频/直播子频道
 
         .. seealso::
@@ -841,7 +880,15 @@
     加油 = "<emoji:315>"
     崇拜 = "<emoji:318>"
     比心 = "<emoji:319>"
     庆祝 = "<emoji:320>"
     拒绝 = "<emoji:322>"
     吃糖 = "<emoji:324>"
     生气 = "<emoji:326>"
+
+
+class WaifForCommandCallback:
+    def __init__(
+        self, command: BotCommandObject, callback: Callable[[Model.MESSAGE], Any]
+    ):
+        self.command = command
+        self.callback = callback
```

### Comparing `qg-botsdk-3.0.1/qg_botsdk/plugins.py` & `qg-botsdk-3.0.2/qg_botsdk/plugins.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk/qg_bot.py` & `qg-botsdk-3.0.2/qg_botsdk/qg_bot.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk/qg_bot_ws.py` & `qg-botsdk-3.0.2/qg_botsdk/qg_bot_ws.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk/session.py` & `qg-botsdk-3.0.2/qg_botsdk/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from ._statics import TraceNames
 from ._utils import TraceCallerData, stack_exception_handler
 from .model import Scope, SessionObject, SessionStatus
 
 
 class AbstractSessionManager:
     """
-    Session Manager用于管理在不同作用域（scope）下的 sessions，具有
+    Session Manager用于管理在不同作用域（scope）下的 sessions，主要用处为存储运行时的临时数据。
+
+    注意：为允许session可以保存class实例等py数据类型，session的数据以pickle方式保存
     """
 
     # -*- session manage methods -*-
     def new(
         self,
         scope: Scope,
         key: Hashable,
```

### Comparing `qg-botsdk-3.0.1/qg_botsdk/utils.py` & `qg-botsdk-3.0.2/qg_botsdk/utils.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/qg_botsdk.egg-info/PKG-INFO` & `qg-botsdk-3.0.2/qg_botsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: qg-botsdk
-Version: 3.0.1
+Version: 3.0.2
 Summary: easy-to-use SDK for Tencent QQ guild robot
 Home-page: https://github.com/GLGDLY/qg_botsdk
 Author: GDLY
 Author-email: tzlgdly@gmail.com
-License: UNKNOWN
 Keywords: sample,example,setuptools
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: <4,>=3.7
 License-File: LICENSE
@@ -197,8 +195,7 @@
 ========
 
 -   文档：
      * `readthedocs <https://qg-botsdk.readthedocs.io/zh_CN/latest/>`_
 -   官方注册机器人：https://q.qq.com/#/
 -   官方API文档：https://bot.q.qq.com/wiki/develop/api/
 -   SDK QQ交流群：https://jq.qq.com/?_wv=1027&k=3NnWvGpz
-
```

### Comparing `qg-botsdk-3.0.1/qg_botsdk.egg-info/SOURCES.txt` & `qg-botsdk-3.0.2/qg_botsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/setup.py` & `qg-botsdk-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/test/_base_context.py` & `qg-botsdk-3.0.2/test/_base_context.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/test/test_api.py` & `qg-botsdk-3.0.2/test/test_api.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/test/test_base.py` & `qg-botsdk-3.0.2/test/test_base.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/test/test_run.py` & `qg-botsdk-3.0.2/test/test_run.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-3.0.1/test/test_session.py` & `qg-botsdk-3.0.2/test/test_session.py`

 * *Files identical despite different names*

