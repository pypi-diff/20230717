# Comparing `tmp/eggella-0.0.2.tar.gz` & `tmp/eggella-0.0.3.tar.gz`

## Comparing `eggella-0.0.2.tar` & `eggella-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/__init__.py
--rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/app.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/exceptions.py
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/manager.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/abc.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/command.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/completer.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/exception_handle.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/handler.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/events/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/events/abc.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/events/events.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/fsm/__init__.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/fsm/fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/shortcuts/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/shortcuts/cmd_shortcuts.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/shortcuts/help_pager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/tools/__init__.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/tools/type_caster.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.2/.gitignore
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 eggella-0.0.2/README.md
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 eggella-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/__init__.py
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/app.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/exceptions.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/manager.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/abc.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/arg_caster.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/completer.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/handler.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/objects.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/events/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/events/abc.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/events/events.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/fsm/__init__.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/fsm/fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/shortcuts/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/shortcuts/cmd_shortcuts.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/shortcuts/help_pager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/tools/__init__.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/tools/type_caster.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.3/.gitignore
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 eggella-0.0.3/README.md
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 eggella-0.0.3/PKG-INFO
```

### Comparing `eggella-0.0.2/eggella/app.py` & `eggella-0.0.3/eggella/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from prompt_toolkit import HTML, PromptSession
 from prompt_toolkit.completion.fuzzy_completer import FuzzyCompleter
 from prompt_toolkit.formatted_text import FormattedText
 
 from eggella.command.abc import ABCCommandHandler
 from eggella.exceptions import CommandNotFoundError, CommandParseError
-from eggella.fsm.fsm import FsmController, IntState
+from eggella.fsm.fsm import FsmController, IntStateGroup
 from eggella.manager import CommandManager, EventManager
 from eggella.shortcuts.cmd_shortcuts import CmdShortCuts
 
 PromptLikeMsg = Union[str, FormattedText, Callable[..., Union[FormattedText, List[Tuple[str, str]]]]]
 
 _DEFAULT_INTRO_MSG = HTML(
     "<ansired>Press |CTRL+C| or |CTRL+D| or type</ansired> exit <ansired>for close this app</ansired>\n"
@@ -93,18 +93,18 @@
         return self._command_manager.command(
             key,
             short_description=short_description,
             usage=usage,
             cmd_handler=cmd_handler,
         )
 
-    def on_state(self, state: IntState):
+    def on_state(self, state: IntStateGroup):
         return self.fsm.state(state)
 
-    def register_states(self, states: Type[IntState]):
+    def register_states(self, states: Type[IntStateGroup]):
         self.fsm.attach(states)
 
     def register_command(
         self,
         func: Callable,
         key: Optional[str] = None,
         short_description: Optional[str] = None,
```

### Comparing `eggella-0.0.2/eggella/manager.py` & `eggella-0.0.3/eggella/manager.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.2/eggella/command/command.py` & `eggella-0.0.3/eggella/command/arg_caster.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,16 @@
 import ast
 import inspect
-import shlex
 from contextlib import suppress
 from typing import Any, Callable, Dict, List, Tuple
 
-from eggella.command.abc import ABCCommandArgumentsCaster, ABCCommandParser
+from eggella.command.abc import ABCCommandArgumentsCaster
 from eggella.tools.type_caster import TypeCaster
 
-
-class CommandParser(ABCCommandParser):
-    def __call__(self, raw_command: str) -> List[str]:
-        return shlex.split(raw_command)
-
-
-class CommandParserRaw(ABCCommandParser):
-    def __call__(self, raw_command: str) -> List[str]:
-        return [raw_command]
+ARGS_AND_KWARGS = Tuple[Tuple[Any], Dict[str, Any]]
 
 
 class CommandArgumentsCaster(ABCCommandArgumentsCaster):
     @staticmethod
     def _literal_eval(token: str) -> Any:
         # simple convert variables like list, dict, int, float
         with suppress(ValueError, SyntaxError):
@@ -44,15 +35,15 @@
                 elif isinstance(values, dict) and param.kind is param.VAR_KEYWORD:
                     bound.arguments[arg_name] = {k: tc.cast(param.annotation, v) for k, v in values.items()}
                 # positional
                 else:
                     bound.arguments[arg_name] = tc.cast(param.annotation, values)
         return bound.args, bound.kwargs
 
-    def __call__(self, fn: Callable, tokens: List[str]) -> Tuple[Tuple[Any], Dict[str, Any]]:
+    def __call__(self, fn: Callable, tokens: List[str]) -> ARGS_AND_KWARGS:
         sig = inspect.signature(fn)
         param_names = list(sig.parameters.keys())
         args: List[Any] = []
         kwargs = {}
 
         for token in tokens:
             if "=" in token:
@@ -63,12 +54,7 @@
             else:
                 args.append(self._literal_eval(token))
         # bind parsed arguments, set defaults values
         bound = sig.bind(*args, **kwargs)
         # set defaults, if not set
         bound.apply_defaults()
         return self._cast_arguments(fn, *bound.args, **bound.kwargs)
-
-
-if __name__ == "__main__":
-    cp = CommandParser()
-    print(cp("a='12 123' 100"))
```

### Comparing `eggella-0.0.2/eggella/command/completer.py` & `eggella-0.0.3/eggella/command/completer.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.2/eggella/command/objects.py` & `eggella-0.0.3/eggella/command/objects.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.2/eggella/events/events.py` & `eggella-0.0.3/eggella/events/events.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.2/eggella/fsm/fsm.py` & `eggella-0.0.3/eggella/fsm/fsm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Type, Union
 
 if TYPE_CHECKING:
     from eggella.app import Eggella
 
 
-class IntState(int, Enum):
+class IntStateGroup(int, Enum):
     @classmethod
-    def last(cls) -> "IntState":
+    def last(cls) -> "IntStateGroup":
         return cls.list()[-1]
 
     @classmethod
-    def list(cls) -> List["IntState"]:
+    def list(cls) -> List["IntStateGroup"]:
         return list(cls.__iter__())
 
     @classmethod
-    def first(cls) -> "IntState":
+    def first(cls) -> "IntStateGroup":
         return cls.list()[0]
 
 
 class Fsm:
-    def __init__(self, state: Type["IntState"]):
+    def __init__(self, state: Type["IntStateGroup"]):
         self.ctx: Dict[str, Any] = {}
-        self.handlers: Dict[IntState, Callable] = {}
+        self.handlers: Dict[IntStateGroup, Callable] = {}
 
         self._all_states = state.list()
         self._start_state = state.first()
         self._end_state = state.last()
-        self._current_state: Optional[IntState] = None
+        self._current_state: Optional[IntStateGroup] = None
 
-    def add_handler(self, state: IntState, func: Callable):
+    def add_handler(self, state: IntStateGroup, func: Callable):
         self.handlers[state] = func
 
     def is_finish(self) -> bool:
         return self._current_state is None
 
-    def on_state(self, state: "IntState"):
+    def on_state(self, state: "IntStateGroup"):
         def decorator(func):
             self.handlers[state] = func
             return func
 
         return decorator
 
-    def set(self, state: "IntState"):
+    def _exec_state(self, state: "IntStateGroup"):
+        if not self.handlers.get(state, None):
+            raise KeyError(f"State {state} is not registered")
+        return self.handlers[state]()
+
+    def set(self, state: "IntStateGroup"):
         self._current_state = state
-        return self.handlers[self._current_state]()
+        return self._exec_state(self._current_state)
 
     def clear(self):
         self.ctx.clear()
 
-    def run(self, state: Optional["IntState"] = None):
+    def run(self, state: Optional["IntStateGroup"] = None):
         self._current_state = state or self._start_state
-        return self.handlers[self._current_state]()
+        return self._exec_state(self._current_state)
 
     def finish(self) -> None:
         self.ctx.clear()
         self._current_state = None
 
     def next(self):
         index = self._all_states.index(self._current_state)
         if index < len(self._all_states):
             self._current_state = self._all_states[index + 1]
-            return self.handlers[self._current_state]()
+            return self._exec_state(self._current_state)
+        elif index == len(self._all_states) - 1 and self._all_states[index] == self._end_state:
+            self.finish()
+            return
         else:
             raise IndexError("States out of range")
 
     def prev(self):
         index = self._all_states.index(self._current_state)
         if index < len(self._all_states) and index != 0:
             self._current_state = self._all_states[index - 1]
-            return self.handlers[self._current_state]()
+            return self._exec_state(self._current_state)
+        elif self._current_state == self._all_states[0]:
+            self.finish()
+            return
         else:
             raise IndexError("States out of range")
 
     def __getitem__(self, item):
         return self.ctx[item]
 
     def __setitem__(self, key, value):
@@ -101,23 +112,29 @@
 
     @property
     def ctx(self):
         if self._current_fsm:
             return self._current_fsm.ctx
         raise AttributeError("Need invoke FSM first")
 
-    def attach(self, states: Type[IntState]):
+    def attach(self, states: Type[IntStateGroup]):
         self.fsm_storage[states.__name__] = Fsm(states)
 
-    def state(self, state: IntState):
+    def state(self, state: IntStateGroup):
         """state decorator"""
+        if not self.fsm_storage.get(state.__class__.__name__):
+            raise RuntimeError(
+                f"State `{state.__class__.__name__}` is not registered in `{self.__app.app_name}`\n"
+                f"Register this state group in application "
+                f"by `register_states({state.__class__.__name__}) method`"
+            )
         return self.fsm_storage[state.__class__.__name__].on_state(state)
 
-    def run(self, state: Union[IntState, Type[IntState]]):
-        if isinstance(state, IntState):
+    def run(self, state: Union[IntStateGroup, Type[IntStateGroup]]):
+        if isinstance(state, IntStateGroup):
             self._current_fsm = self.fsm_storage[state.__class__.__name__]
             return self._current_fsm.run(state)
         else:
             self._current_fsm = self.fsm_storage[state.__name__]
             return self._current_fsm.run(state.first())
 
     def prev(self):
@@ -126,29 +143,29 @@
         self._current_fsm.prev()
 
     def next(self):
         if not self._current_fsm:
             raise AttributeError("Need activate FSM first")
         self._current_fsm.next()
 
-    def set(self, state: IntState):
+    def set(self, state: IntStateGroup):
         if not self._current_fsm:
             raise AttributeError("Need activate FSM first")
         self._current_fsm.set(state)
 
     def finish(self):
         if not self._current_fsm:
             raise AttributeError("Need activate FSM first")
         self._current_fsm.finish()
         self._current_fsm = None
 
 
 if __name__ == "__main__":
 
-    class MyStates(IntState):
+    class MyStates(IntStateGroup):
         a = 1
         b = 2
 
     print(type(MyStates))
     print(type(MyStates.a))
     # print(MyStates.__name__)
     # print(MyStates.first().__class__.__name__)
```

### Comparing `eggella-0.0.2/eggella/shortcuts/cmd_shortcuts.py` & `eggella-0.0.3/eggella/shortcuts/cmd_shortcuts.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.2/eggella/shortcuts/help_pager.py` & `eggella-0.0.3/eggella/shortcuts/help_pager.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.2/eggella/tools/type_caster.py` & `eggella-0.0.3/eggella/tools/type_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.2/.gitignore` & `eggella-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `eggella-0.0.2/README.md` & `eggella-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -61,18 +61,18 @@
 
 ```python
 from typing import Optional
 
 from prompt_toolkit.validation import Validator
 
 from eggella import Eggella
-from eggella.fsm import IntState
+from eggella.fsm import IntStateGroup
 
 
-class LoginForm(IntState):
+class LoginForm(IntStateGroup):
     EMAIL = 0
     PASSWORD = 1
     ACCEPT = 2
 
 
 # prompt validators
```

### Comparing `eggella-0.0.2/pyproject.toml` & `eggella-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eggella-0.0.2/PKG-INFO` & `eggella-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eggella
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create awesome command line applications with less effort
 Project-URL: Documentation, https://github.com/unknown/eggella#readme
 Project-URL: Issues, https://github.com/unknown/eggella/issues
 Project-URL: Source, https://github.com/unknown/eggella
 Author: georgiy
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -87,18 +87,18 @@
 
 ```python
 from typing import Optional
 
 from prompt_toolkit.validation import Validator
 
 from eggella import Eggella
-from eggella.fsm import IntState
+from eggella.fsm import IntStateGroup
 
 
-class LoginForm(IntState):
+class LoginForm(IntStateGroup):
     EMAIL = 0
     PASSWORD = 1
     ACCEPT = 2
 
 
 # prompt validators
```

