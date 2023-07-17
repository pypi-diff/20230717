# Comparing `tmp/magentic-0.1.0.tar.gz` & `tmp/magentic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magentic-0.1.0.tar", max compression
+gzip compressed data, was "magentic-0.1.1.tar", max compression
```

## Comparing `magentic-0.1.0.tar` & `magentic-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-06-18 04:31:45.568698 magentic-0.1.0/LICENSE
--rw-r--r--   0        0        0     4929 2023-07-15 06:44:51.832343 magentic-0.1.0/README.md
--rw-r--r--   0        0        0      870 2023-07-15 07:09:32.567309 magentic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-07-15 07:11:09.503451 magentic-0.1.0/src/magentic/__init__.py
--rw-r--r--   0        0        0     2100 2023-07-15 07:11:09.503748 magentic-0.1.0/src/magentic/chat.py
--rw-r--r--   0        0        0        0 2023-07-15 07:11:09.503836 magentic-0.1.0/src/magentic/chat_model/__init__.py
--rw-r--r--   0        0        0     1559 2023-07-15 07:11:09.506563 magentic-0.1.0/src/magentic/chat_model/base.py
--rw-r--r--   0        0        0     9060 2023-07-15 07:11:09.510614 magentic-0.1.0/src/magentic/chat_model/openai_chat_model.py
--rw-r--r--   0        0        0     1019 2023-07-15 07:11:09.512404 magentic-0.1.0/src/magentic/function_call.py
--rw-r--r--   0        0        0     1712 2023-07-15 07:11:09.513068 magentic-0.1.0/src/magentic/prompt_chain.py
--rw-r--r--   0        0        0     3289 2023-07-15 07:11:09.513678 magentic-0.1.0/src/magentic/prompt_function.py
--rw-r--r--   0        0        0       61 2023-07-15 07:11:09.514294 magentic-0.1.0/src/magentic/py.typed
--rw-r--r--   0        0        0      672 2023-07-15 07:11:09.514838 magentic-0.1.0/src/magentic/typing.py
--rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 magentic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-18 04:31:45.568698 magentic-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4936 2023-07-15 16:45:38.068501 magentic-0.1.1/README.md
+-rw-r--r--   0        0        0      922 2023-07-17 06:22:04.852150 magentic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-07-15 07:11:09.503451 magentic-0.1.1/src/magentic/__init__.py
+-rw-r--r--   0        0        0     2100 2023-07-15 07:11:09.503748 magentic-0.1.1/src/magentic/chat.py
+-rw-r--r--   0        0        0        0 2023-07-15 07:11:09.503836 magentic-0.1.1/src/magentic/chat_model/__init__.py
+-rw-r--r--   0        0        0     1517 2023-07-16 21:00:12.901908 magentic-0.1.1/src/magentic/chat_model/base.py
+-rw-r--r--   0        0        0     9687 2023-07-17 06:21:54.657860 magentic-0.1.1/src/magentic/chat_model/openai_chat_model.py
+-rw-r--r--   0        0        0     1019 2023-07-15 07:11:09.512404 magentic-0.1.1/src/magentic/function_call.py
+-rw-r--r--   0        0        0     1712 2023-07-15 07:11:09.513068 magentic-0.1.1/src/magentic/prompt_chain.py
+-rw-r--r--   0        0        0     3271 2023-07-16 20:42:38.366497 magentic-0.1.1/src/magentic/prompt_function.py
+-rw-r--r--   0        0        0       61 2023-07-15 07:11:09.514294 magentic-0.1.1/src/magentic/py.typed
+-rw-r--r--   0        0        0     1584 2023-07-17 05:50:31.713612 magentic-0.1.1/src/magentic/typing.py
+-rw-r--r--   0        0        0     5529 1970-01-01 00:00:00.000000 magentic-0.1.1/PKG-INFO
```

### Comparing `magentic-0.1.0/LICENSE` & `magentic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magentic-0.1.0/README.md` & `magentic-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,17 @@
 
 ```python
 from typing import Literal
 
 from magentic import prompt, FunctionCall
 
 
-def activate_oven(temperature: int, mode: Literal["broil", "bake", "roast"]):
+def activate_oven(temperature: int, mode: Literal["broil", "bake", "roast"]) -> str:
     """Turn the oven on with the provided settings."""
-    print(f"Preheating to {temperature} F with mode {mode}")
+    return f"Preheating to {temperature} F with mode {mode}"
 
 
 @prompt(
     template="Prepare the oven so I can make {food}",
     functions=[activate_oven],
 )
 def configure_oven(food: str) -> FunctionCall[str]:
```

### Comparing `magentic-0.1.0/pyproject.toml` & `magentic-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 check_untyped_defs = true
 disable_error_code = ["empty-body"]
 disallow_untyped_defs = false
 strict = true
 
 [tool.poetry]
 name = "magentic"
-version = "0.1.0"
+version = "0.1.1"
 description = "Seamlessly integrate LLMs as Python functions"
 license = "MIT"
 authors = ["Jack Collins"]
 readme = "README.md"
 repository = "https://github.com/jackmpcollins/magentic"
 
 [tool.poetry.dependencies]
@@ -39,9 +39,12 @@
 markers = [
     "openai: Tests that query the OpenAI API"
 ]
 
 [tool.ruff]
 line-length = 120
 
+[tool.ruff.isort]
+known-first-party = ["magentic"]
+
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `magentic-0.1.0/src/magentic/chat.py` & `magentic-0.1.1/src/magentic/chat.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.0/src/magentic/chat_model/base.py` & `magentic-0.1.1/src/magentic/chat_model/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Generic, TypeVar
+from typing import Generic, TypeVar
 
 from magentic.function_call import FunctionCall
 
 T = TypeVar("T")
 
 
 class Message(Generic[T]):
@@ -26,31 +26,30 @@
     ...
 
 
 class AssistantMessage(Message[T], Generic[T]):
     ...
 
 
-Self = TypeVar("Self", bound="FunctionResultMessage[Any]")
-
-
 class FunctionResultMessage(Message[T], Generic[T]):
     def __init__(self, content: T, function_call: FunctionCall[T]):
         super().__init__(content)
         self._function_call = function_call
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.content!r}, {self._function_call!r})"
 
     @property
     def function_call(self) -> FunctionCall[T]:
         return self._function_call
 
     @classmethod
-    def from_function_call(cls: type[Self], function_call: FunctionCall[T]) -> Self:
+    def from_function_call(
+        cls, function_call: FunctionCall[T]
+    ) -> "FunctionResultMessage[T]":
         return cls(
             content=function_call(),
             function_call=function_call,
         )
 
 
 class FunctionCallMessage(AssistantMessage[FunctionCall[T]], Generic[T]):
```

### Comparing `magentic-0.1.0/src/magentic/chat_model/openai_chat_model.py` & `magentic-0.1.1/src/magentic/chat_model/openai_chat_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 import inspect
 import json
 from abc import ABC, abstractmethod
-from copy import deepcopy
 from enum import Enum
 from typing import Any, Callable, Generic, Iterable, TypeVar
 
 import openai
-from pydantic import BaseModel, validate_arguments
+from pydantic import BaseModel, TypeAdapter, create_model
 
 from magentic.chat_model.base import (
     AssistantMessage,
     FunctionCallMessage,
     FunctionResultMessage,
     Message,
     UserMessage,
 )
 from magentic.function_call import FunctionCall
-from magentic.typing import is_origin_subclass
+from magentic.typing import is_origin_subclass, name_type
 
 T = TypeVar("T")
 
 
-class Output(BaseModel, Generic[T]):
-    value: T
-
-
 class BaseFunctionSchema(ABC, Generic[T]):
     @property
     @abstractmethod
     def name(self) -> str:
         ...
 
     @property
@@ -54,23 +49,27 @@
         return AssistantMessage(self.parse_args(arguments))
 
     @abstractmethod
     def serialize_args(self, value: T) -> str:
         ...
 
 
+class Output(BaseModel, Generic[T]):
+    value: T
+
+
 class AnyFunctionSchema(BaseFunctionSchema[T], Generic[T]):
     def __init__(self, output_type: type[T]):
         self._output_type = output_type
         # https://github.com/python/mypy/issues/14458
         self._model = Output[output_type]  # type: ignore[valid-type]
 
     @property
     def name(self) -> str:
-        return f"return_{self._output_type.__name__.lower()}"
+        return f"return_{name_type(self._output_type)}"
 
     @property
     def parameters(self) -> dict[str, Any]:
         model_schema = self._model.model_json_schema().copy()
         model_schema.pop("title", None)
         model_schema.pop("description", None)
         return model_schema
@@ -78,14 +77,36 @@
     def parse_args(self, arguments: str) -> T:
         return self._model.model_validate_json(arguments).value
 
     def serialize_args(self, value: T) -> str:
         return self._model(value=value).model_dump_json()
 
 
+class DictFunctionSchema(BaseFunctionSchema[T], Generic[T]):
+    def __init__(self, output_type: type[T]):
+        self._output_type = output_type
+        self._type_adapter: TypeAdapter[T] = TypeAdapter(output_type)
+
+    @property
+    def name(self) -> str:
+        return f"return_{name_type(self._output_type)}"
+
+    @property
+    def parameters(self) -> dict[str, Any]:
+        model_schema = self._type_adapter.json_schema().copy()
+        model_schema["properties"] = model_schema.get("properties", {})
+        return model_schema
+
+    def parse_args(self, arguments: str) -> T:
+        return self._type_adapter.validate_json(arguments)
+
+    def serialize_args(self, value: T) -> str:
+        return json.dumps(value)
+
+
 BaseModelT = TypeVar("BaseModelT", bound=BaseModel)
 
 
 class BaseModelFunctionSchema(BaseFunctionSchema[BaseModelT], Generic[BaseModelT]):
     def __init__(self, model: type[BaseModelT]):
         self._model = model
 
@@ -106,56 +127,57 @@
     def serialize_args(self, value: BaseModelT) -> str:
         return value.model_dump_json()
 
 
 class FunctionCallFunctionSchema(BaseFunctionSchema[FunctionCall[T]], Generic[T]):
     def __init__(self, func: Callable[..., T]):
         self._func = func
-        # https://github.com/python/mypy/issues/2087
-        self._model: BaseModel = validate_arguments(self._func).model  # type: ignore[operator]
-        self._func_parameters = inspect.signature(self._func).parameters.keys()
+        # https://github.com/pydantic/pydantic/issues/3585#issuecomment-1002745763
+        fields: dict[str, Any] = {
+            param.name: (
+                (param.annotation if param.annotation != inspect._empty else Any),
+                (param.default if param.default != inspect._empty else ...),
+            )
+            for param in inspect.signature(func).parameters.values()
+        }
+        self._model = create_model("FuncModel", **fields)
 
     @property
     def name(self) -> str:
         return self._func.__name__
 
     @property
     def description(self) -> str | None:
         return inspect.getdoc(self._func)
 
     @property
     def parameters(self) -> dict[str, Any]:
-        schema = deepcopy(self._model.model_json_schema())
-        schema.pop("additionalProperties", None)
+        schema: dict[str, Any] = self._model.model_json_schema().copy()
         schema.pop("title", None)
-        # Pydantic adds extra parameters to the schema for the function
-        # https://docs.pydantic.dev/latest/usage/validation_decorator/#model-fields-and-reserved-arguments
-        schema["properties"] = {
-            k: v for k, v in schema["properties"].items() if k in self._func_parameters
-        }
         return schema
 
     def parse_args(self, arguments: str) -> FunctionCall[T]:
-        args = self._model.model_validate_json(arguments).model_dump(
-            include=set(self._func_parameters)
-        )
+        args = self._model.model_validate_json(arguments).model_dump()
         return FunctionCall(self._func, **args)
 
     def parse_args_to_message(self, arguments: str) -> FunctionCallMessage[T]:
         return FunctionCallMessage(self.parse_args(arguments))
 
     def serialize_args(self, value: FunctionCall[T]) -> str:
         return json.dumps(value.arguments)
 
 
 def function_schema_for_type(type_: type[T]) -> BaseFunctionSchema[T]:
     """Create a FunctionSchema for the given type."""
     if is_origin_subclass(type_, BaseModel):
         return BaseModelFunctionSchema(type_)  # type: ignore[return-value]
 
+    if is_origin_subclass(type_, dict):
+        return DictFunctionSchema(type_)  # type: ignore[arg-type]
+
     return AnyFunctionSchema(type_)
 
 
 class OpenaiMessageRole(Enum):
     ASSISTANT = "assistant"
     FUNCTION = "function"
     SYSTEM = "system"
@@ -221,17 +243,16 @@
         function_schemas: list[
             FunctionCallFunctionSchema[FuncR] | BaseFunctionSchema[R]
         ] = []
         for function in functions or []:
             function_schemas.append(FunctionCallFunctionSchema(function))
         for output_type in output_types:
             if issubclass(output_type, str):
-                pass
-            else:
-                function_schemas.append(function_schema_for_type(output_type))
+                continue
+            function_schemas.append(function_schema_for_type(output_type))
 
         includes_str_output_type = any(issubclass(cls, str) for cls in output_types)
 
         # `openai.ChatCompletion.create` doesn't accept `None`
         # so only pass function args if there are functions
         function_args: dict[str, Any] = {}
         if function_schemas:
```

### Comparing `magentic-0.1.0/src/magentic/function_call.py` & `magentic-0.1.1/src/magentic/function_call.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.0/src/magentic/prompt_chain.py` & `magentic-0.1.1/src/magentic/prompt_chain.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.0/src/magentic/prompt_function.py` & `magentic-0.1.1/src/magentic/prompt_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,17 +29,17 @@
             return_annotation=return_type,
         )
         self._template = template
         self._functions = functions or []
         self._model = model or OpenaiChatModel()
 
         self._return_types = [
-            return_type
-            for return_type in split_union_type(return_type)
-            if not is_origin_subclass(return_type, FunctionCall)
+            type_
+            for type_ in split_union_type(return_type)
+            if not is_origin_subclass(type_, FunctionCall)
         ]
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
         bound_args = self._signature.bind(*args, **kwargs)
         bound_args.apply_defaults()
         message = self._model.complete(
             messages=[
```

### Comparing `magentic-0.1.0/PKG-INFO` & `magentic-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magentic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Seamlessly integrate LLMs as Python functions
 Home-page: https://github.com/jackmpcollins/magentic
 License: MIT
 Author: Jack Collins
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -75,17 +75,17 @@
 
 ```python
 from typing import Literal
 
 from magentic import prompt, FunctionCall
 
 
-def activate_oven(temperature: int, mode: Literal["broil", "bake", "roast"]):
+def activate_oven(temperature: int, mode: Literal["broil", "bake", "roast"]) -> str:
     """Turn the oven on with the provided settings."""
-    print(f"Preheating to {temperature} F with mode {mode}")
+    return f"Preheating to {temperature} F with mode {mode}"
 
 
 @prompt(
     template="Prepare the oven so I can make {food}",
     functions=[activate_oven],
 )
 def configure_oven(food: str) -> FunctionCall[str]:
```

