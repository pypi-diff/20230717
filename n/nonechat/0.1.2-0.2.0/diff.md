# Comparing `tmp/nonechat-0.1.2.tar.gz` & `tmp/nonechat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonechat-0.1.2.tar", last modified: Sat Jul 15 10:16:27 2023, max compression
+gzip compressed data, was "nonechat-0.2.0.tar", last modified: Mon Jul 17 01:21:04 2023, max compression
```

## Comparing `nonechat-0.1.2.tar` & `nonechat-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      984 2023-07-15 10:15:48.014680 nonechat-0.1.2/README.md
--rw-r--r--   0        0        0      359 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/__init__.py
--rw-r--r--   0        0        0     3528 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/app.py
--rw-r--r--   0        0        0      745 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/backend.py
--rw-r--r--   0        0        0      912 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/chatroom/__init__.py
--rw-r--r--   0        0        0     2013 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/chatroom/history.py
--rw-r--r--   0        0        0     1418 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/chatroom/input.py
--rw-r--r--   0        0        0     4053 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/chatroom/message.py
--rw-r--r--   0        0        0     2234 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/chatroom/toolbar.py
--rw-r--r--   0        0        0       45 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/footer.py
--rw-r--r--   0        0        0      950 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/general/action.py
--rw-r--r--   0        0        0     1184 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/header.py
--rw-r--r--   0        0        0     1508 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/components/log/__init__.py
--rw-r--r--   0        0        0     1499 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/components/log/toolbar.py
--rw-r--r--   0        0        0      582 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/info.py
--rw-r--r--   0        0        0     1143 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/log_redirect.py
--rw-r--r--   0        0        0     4132 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/message.py
--rw-r--r--   0        0        0       92 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/router/__init__.py
--rw-r--r--   0        0        0     1222 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/router/router.py
--rw-r--r--   0        0        0      416 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/setting.py
--rw-r--r--   0        0        0     2131 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/storage/__init__.py
--rw-r--r--   0        0        0      285 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/utils.py
--rw-r--r--   0        0        0     1905 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/views/horizontal.py
--rw-r--r--   0        0        0      700 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/views/log_view.py
--rw-r--r--   0        0        0     1224 2023-07-15 10:16:27.093310 nonechat-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 nonechat-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      523 2023-07-17 01:20:32.519825 nonechat-0.2.0/README.md
+-rw-r--r--   0        0        0      359 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/__init__.py
+-rw-r--r--   0        0        0     3756 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/app.py
+-rw-r--r--   0        0        0      674 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/backend.py
+-rw-r--r--   0        0        0        0 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/__init__.py
+-rw-r--r--   0        0        0      950 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/action.py
+-rw-r--r--   0        0        0      913 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/chatroom/__init__.py
+-rw-r--r--   0        0        0     2013 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/chatroom/history.py
+-rw-r--r--   0        0        0     1418 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/chatroom/input.py
+-rw-r--r--   0        0        0     4053 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/chatroom/message.py
+-rw-r--r--   0        0        0     2396 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/chatroom/toolbar.py
+-rw-r--r--   0        0        0       45 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/footer.py
+-rw-r--r--   0        0        0     1184 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/header.py
+-rw-r--r--   0        0        0     1508 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/log/__init__.py
+-rw-r--r--   0        0        0     1561 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/log/toolbar.py
+-rw-r--r--   0        0        0      582 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/info.py
+-rw-r--r--   0        0        0     1143 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/log_redirect.py
+-rw-r--r--   0        0        0     4132 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/message.py
+-rw-r--r--   0        0        0       92 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/router/__init__.py
+-rw-r--r--   0        0        0     1222 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/router/router.py
+-rw-r--r--   0        0        0      690 2023-07-17 01:20:32.523825 nonechat-0.2.0/nonechat/setting.py
+-rw-r--r--   0        0        0     2079 2023-07-17 01:20:32.523825 nonechat-0.2.0/nonechat/storage/__init__.py
+-rw-r--r--   0        0        0      285 2023-07-17 01:20:32.523825 nonechat-0.2.0/nonechat/utils.py
+-rw-r--r--   0        0        0     1905 2023-07-17 01:20:32.523825 nonechat-0.2.0/nonechat/views/horizontal.py
+-rw-r--r--   0        0        0      700 2023-07-17 01:20:32.523825 nonechat-0.2.0/nonechat/views/log_view.py
+-rw-r--r--   0        0        0     1303 2023-07-17 01:21:04.676749 nonechat-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 nonechat-0.2.0/PKG-INFO
```

### Comparing `nonechat-0.1.2/README.md` & `nonechat-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,30 @@
 # Nonechat
 
 通用控制台聊天界面
 
 ## 使用
 
 ```python
+from nonechat.info import Event
 from nonechat.app import Frontend
 from nonechat.backend import Backend
-from nonechat.info import User, MessageEvent, Event
-from nonechat.message import ConsoleMessage, Text
-from datetime import datetime
 
 
 class ExampleBackend(Backend):
 
-    def on_console_init(self):
-        print("on_console_init")
-
     def on_console_load(self):
         print("on_console_load")
 
     def on_console_mount(self):
         print("on_console_mount")
 
     def on_console_unmount(self):
         print("on_console_unmount")
 
-    async def build_message_event(self, message: str, user: User) -> MessageEvent:
-        return MessageEvent(
-            time=datetime.now(),
-            self_id="robot",
-            type="console.message",
-            user=user,
-            message=ConsoleMessage([Text(message)])
-        )
-
     async def post_event(self, event: Event):
         print("post_event")
 
 
 app = Frontend(ExampleBackend)
 app.run()
 ```
```

### Comparing `nonechat-0.1.2/nonechat/app.py` & `nonechat-0.2.0/nonechat/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from .storage import Storage
 from .router import RouterView
 from .log_redirect import FakeIO
 from .setting import ConsoleSetting
 from .views.log_view import LogView
 from .components.footer import Footer
 from .components.header import Header
-from .info import Event, MessageEvent
+from .message import Text, ConsoleMessage
+from .info import User, Event, MessageEvent
 from .views.horizontal import HorizontalView
 
 TB = TypeVar("TB", bound=Backend)
 
 
 class Frontend(App, Generic[TB]):
     BINDINGS = [
@@ -28,23 +29,22 @@
         Binding("ctrl+underscore", "focus_input", "Focus input", key_display="ctrl+/"),
     ]
 
     ROUTES = {"main": lambda: HorizontalView(), "log": lambda: LogView()}
 
     def __init__(self, backend: Type[TB], setting: ConsoleSetting = ConsoleSetting()):
         super().__init__()
-        self.backend: TB = backend(self)
         self.setting = setting
         self.title = setting.title  # type: ignore
         self.sub_title = setting.sub_title  # type: ignore
-        self.storage = Storage()
-        self.backend.on_console_init()
+        self.storage = Storage(User("console", setting.user_avatar, setting.user_name))
         self._fake_output = cast(TextIO, FakeIO(self.storage))
         self._redirect_stdout: Optional[contextlib.redirect_stdout[TextIO]] = None
         self._redirect_stderr: Optional[contextlib.redirect_stderr[TextIO]] = None
+        self.backend: TB = backend(self)
 
     def compose(self):
         yield Header()
         yield RouterView(self.ROUTES, "main")
         yield Footer()
 
     def on_load(self):
@@ -74,26 +74,32 @@
 
     async def call(self, api: str, data: Dict[str, Any]):
         if api == "send_msg":
             self.storage.write_chat(
                 MessageEvent(
                     type="console.message",
                     time=datetime.now(),
-                    self_id=data["info"].id,
+                    self_id=self.backend.bot.id,
                     message=data["message"],
-                    user=data["info"],
+                    user=self.backend.bot,
                 )
             )
         elif api == "bell":
             await self.run_action("bell")
 
     def action_focus_input(self):
         with contextlib.suppress(Exception):
             self.query_one(Input).focus()
 
     async def action_post_message(self, message: str):
-        msg = await self.backend.build_message_event(message, self.storage.current_user)
+        msg = MessageEvent(
+            time=datetime.now(),
+            self_id=self.backend.bot.id,
+            type="console.message",
+            user=self.storage.current_user,
+            message=ConsoleMessage([Text(message)]),
+        )
         self.storage.write_chat(msg)
         await self.backend.post_event(msg)
 
     async def action_post_event(self, event: Event):
         await self.backend.post_event(event)
```

### Comparing `nonechat-0.1.2/nonechat/components/chatroom/__init__.py` & `nonechat-0.2.0/nonechat/components/chatroom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from textual.binding import Binding
 
 from .input import InputBox
 from .toolbar import Toolbar
 from .history import ChatHistory
 
 if TYPE_CHECKING:
-    from ..app import Frontend
+    from ...app import Frontend
 
 
 class ChatRoom(Widget):
     DEFAULT_CSS = """
     ChatRoom {
         layout: vertical;
     }
```

### Comparing `nonechat-0.1.2/nonechat/components/chatroom/history.py` & `nonechat-0.2.0/nonechat/components/chatroom/history.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/components/chatroom/input.py` & `nonechat-0.2.0/nonechat/components/chatroom/input.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/components/chatroom/message.py` & `nonechat-0.2.0/nonechat/components/chatroom/message.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/components/chatroom/toolbar.py` & `nonechat-0.2.0/nonechat/components/chatroom/toolbar.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING, cast
 
 from textual.widget import Widget
 from textual.widgets import Static
 
+from ..action import Action
 from ...router import RouteChange
-from ..general.action import Action
 
 if TYPE_CHECKING:
     from .history import ChatHistory
     from ...setting import ConsoleSetting
     from ...views.horizontal import HorizontalView
 
 
@@ -40,19 +40,21 @@
     Toolbar Action.mr {
         margin-right: 4;
     }
     """
 
     def __init__(self, setting: "ConsoleSetting"):
         super().__init__()
-        self.exit_button = Action("⛔", id="exit", classes="left")
-        self.clear_button = Action("🗑️", id="clear", classes="left ml")
+        self.exit_button = Action(setting.toolbar_exit, id="exit", classes="left")
+        self.clear_button = Action(setting.toolbar_clear, id="clear", classes="left ml")
         self.center_title = Static(setting.room_title, classes="center")
-        self.settings_button = Action("⚙️", id="settings", classes="right mr")
-        self.log_button = Action("📝", id="log", classes="right")
+        self.settings_button = Action(
+            setting.toolbar_setting, id="settings", classes="right mr"
+        )
+        self.log_button = Action(setting.toolbar_log, id="log", classes="right")
 
     def compose(self):
         yield self.exit_button
         yield self.clear_button
 
         yield self.center_title
 
@@ -60,17 +62,21 @@
         yield self.log_button
 
     async def on_action_pressed(self, event: Action.Pressed):
         event.stop()
         if event.action == self.exit_button:
             self.app.exit()
         elif event.action == self.clear_button:
-            history = cast("ChatHistory", self.app.query_one("ChatHistory"))
+            history: "ChatHistory" = cast(
+                "ChatHistory", self.app.query_one("ChatHistory")
+            )
             history.action_clear_history()
         elif event.action == self.settings_button:
             ...
         elif event.action == self.log_button:
-            view = cast("HorizontalView", self.app.query_one("HorizontalView"))
+            view: "HorizontalView" = cast(
+                "HorizontalView", self.app.query_one("HorizontalView")
+            )
             if view.can_show_log:
                 view.action_toggle_log_panel()
             else:
                 self.post_message(RouteChange("log"))  # noqa
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nonechat-0.1.2/nonechat/components/general/action.py` & `nonechat-0.2.0/nonechat/components/action.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/components/header.py` & `nonechat-0.2.0/nonechat/components/header.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/components/log/__init__.py` & `nonechat-0.2.0/nonechat/components/log/__init__.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/info.py` & `nonechat-0.2.0/nonechat/info.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/log_redirect.py` & `nonechat-0.2.0/nonechat/log_redirect.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/message.py` & `nonechat-0.2.0/nonechat/message.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/router/router.py` & `nonechat-0.2.0/nonechat/router/router.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/storage/__init__.py` & `nonechat-0.2.0/nonechat/storage/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(self, data: T) -> None:
         super().__init__()
         self.data = data
 
 
 @dataclass
 class Storage:
-    current_user: User = field(default_factory=lambda: User(id="console"))
+    current_user: User
 
     log_history: List[RenderableType] = field(default_factory=list)
     log_watchers: List[Widget] = field(default_factory=list)
 
     chat_history: List[MessageEvent] = field(default_factory=list)
     chat_watchers: List[Widget] = field(default_factory=list)
```

### Comparing `nonechat-0.1.2/nonechat/views/horizontal.py` & `nonechat-0.2.0/nonechat/views/horizontal.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/nonechat/views/log_view.py` & `nonechat-0.2.0/nonechat/views/log_view.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.2/pyproject.toml` & `nonechat-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "nonechat"
-version = "0.1.2"
 description = "Awesome chat console using Textual"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "textual ~=0.29.0",
 ]
 requires-python = ">=3.8, <4.0"
 readme = "README.md"
+dynamic = []
+version = "0.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/nonebot/nonechat"
 repository = "https://github.com/nonebot/nonechat"
@@ -29,14 +30,18 @@
 ]
 
 [tool.pdm.build]
 includes = [
     "nonechat",
 ]
 
+[tool.pdm.version]
+source = "file"
+path = "nonechat/__init__.py"
+
 [tool.black]
 line-length = 88
 target-version = [
     "py38",
     "py39",
     "py310",
     "py311",
```

### Comparing `nonechat-0.1.2/PKG-INFO` & `nonechat-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonechat
-Version: 0.1.2
+Version: 0.2.0
 Summary: Awesome chat console using Textual
 Home-page: https://github.com/nonebot/nonechat
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonebot/nonechat
 Project-URL: Repository, https://github.com/nonebot/nonechat
 Requires-Python: <4.0,>=3.8
@@ -14,44 +14,30 @@
 # Nonechat
 
 通用控制台聊天界面
 
 ## 使用
 
 ```python
+from nonechat.info import Event
 from nonechat.app import Frontend
 from nonechat.backend import Backend
-from nonechat.info import User, MessageEvent, Event
-from nonechat.message import ConsoleMessage, Text
-from datetime import datetime
 
 
 class ExampleBackend(Backend):
 
-    def on_console_init(self):
-        print("on_console_init")
-
     def on_console_load(self):
         print("on_console_load")
 
     def on_console_mount(self):
         print("on_console_mount")
 
     def on_console_unmount(self):
         print("on_console_unmount")
 
-    async def build_message_event(self, message: str, user: User) -> MessageEvent:
-        return MessageEvent(
-            time=datetime.now(),
-            self_id="robot",
-            type="console.message",
-            user=user,
-            message=ConsoleMessage([Text(message)])
-        )
-
     async def post_event(self, event: Event):
         print("post_event")
 
 
 app = Frontend(ExampleBackend)
 app.run()
 ```
```

