# Comparing `tmp/fast_depends-2.0.5.tar.gz` & `tmp/fast_depends-2.1.0.tar.gz`

## Comparing `fast_depends-2.0.5.tar` & `fast_depends-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.5/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.5/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.5/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.0.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/_compat.py
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/use.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/core/__init__.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/core/build.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/core/model.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/dependencies/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/dependencies/model.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/dependencies/provider.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.5/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.5/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.5/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.5/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.5/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.5/LICENSE
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 fast_depends-2.0.5/README.md
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 fast_depends-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 fast_depends-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.1.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.1.0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.1.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/__init__.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/_compat.py
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/use.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/core/build.py
+-rw-r--r--   0        0        0    10029 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/core/model.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.1.0/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.1.0/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.1.0/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.1.0/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.1.0/LICENSE
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fast_depends-2.1.0/README.md
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 fast_depends-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 fast_depends-2.1.0/PKG-INFO
```

### Comparing `fast_depends-2.0.5/CONTRIBUTING.md` & `fast_depends-2.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/.github/workflows/documentation.yml` & `fast_depends-2.1.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/.github/workflows/publish_coverage.yml` & `fast_depends-2.1.0/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/.github/workflows/publish_pypi.yml` & `fast_depends-2.1.0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/.github/workflows/tests.yml` & `fast_depends-2.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/fast_depends/_compat.py` & `fast_depends-2.1.0/fast_depends/_compat.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/fast_depends/use.py` & `fast_depends-2.1.0/fast_depends/use.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/fast_depends/utils.py` & `fast_depends-2.1.0/fast_depends/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,46 +44,61 @@
 ) -> T:
     if kwargs:  # pragma: no cover
         func = functools.partial(func, **kwargs)
     return await anyio.to_thread.run_sync(func, *args)
 
 
 async def solve_generator_async(
-    *, call: Callable[..., Any], stack: AsyncExitStack, **sub_values: Any
+    *sub_args: Any, call: Callable[..., Any], stack: AsyncExitStack, **sub_values: Any
 ) -> Any:
     if is_gen_callable(call):
         cm = contextmanager_in_threadpool(contextmanager(call)(**sub_values))
     elif is_async_gen_callable(call):  # pragma: no branch
-        cm = asynccontextmanager(call)(**sub_values)
+        cm = asynccontextmanager(call)(*sub_args, **sub_values)
     return await stack.enter_async_context(cm)
 
 
 def solve_generator_sync(
-    *, call: Callable[..., Any], stack: ExitStack, **sub_values: Any
+    *sub_args: Any, call: Callable[..., Any], stack: ExitStack, **sub_values: Any
 ) -> Any:
-    cm = contextmanager(call)(**sub_values)
+    cm = contextmanager(call)(*sub_args, **sub_values)
     return stack.enter_context(cm)
 
 
 def args_to_kwargs(
     arguments: Iterable[str], *args: Any, **kwargs: Any
 ) -> Dict[str, Any]:
+    arguments = tuple(filter(lambda i: i not in ("args", "kwargs"), arguments))
+
     if not args:
         return kwargs
 
-    unused = filter(lambda x: x not in kwargs, arguments)
+    merged = {"kwargs": kwargs.get("kwargs", {})}
+
+    for arg, v in kwargs.items():
+        if arg not in arguments:
+            merged["kwargs"][arg] = v
+        else:
+            merged[arg] = v
+
+    for arg in filter(lambda x: x not in merged, arguments):
+        if args:
+            merged[arg], args = args[0], args[1:]
 
-    return dict((*zip(unused, args), *kwargs.items()))
+    merged["args"] = args
+
+    return merged
 
 
 def get_typed_signature(
     call: Callable[..., Any]
 ) -> Tuple[List[inspect.Parameter], Any]:
     signature = inspect.signature(call)
     globalns = getattr(call, "__globals__", {})
+
     return [
         inspect.Parameter(
             name=param.name,
             kind=param.kind,
             default=param.default,
             annotation=get_typed_annotation(param.annotation, globalns),
         )
```

### Comparing `fast_depends-2.0.5/fast_depends/core/build.py` & `fast_depends-2.1.0/fast_depends/core/build.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 import inspect
-from typing import Any, Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 from typing_extensions import (
     Annotated,
     ParamSpec,
     TypeVar,
     assert_never,
     get_args,
@@ -45,15 +55,22 @@
         ), f"You cannot use async dependency `{name}` at sync main"
 
     typed_params, return_annotation = get_typed_signature(call)
 
     class_fields: Dict[str, Tuple[Any, Any]] = {}
     dependencies: Dict[str, CallModel[..., Any]] = {}
     custom_fields: Dict[str, CustomField] = {}
+    positional_args: List[str] = []
+    keyword_args: List[str] = []
     for param in typed_params:
+        if param.kind is param.KEYWORD_ONLY:
+            keyword_args.append(param.name)
+        elif param.name not in ("args", "kwargs"):
+            positional_args.append(param.name)
+
         dep: Optional[Depends] = None
         custom: Optional[CustomField] = None
 
         if param.annotation is inspect._empty:
             annotation = Any
 
         elif get_origin(param.annotation) is Annotated:
@@ -78,15 +95,21 @@
 
                 annotation = type_annotation
             else:
                 annotation = param.annotation
         else:
             annotation = param.annotation
 
-        default = param.default
+        if param.name == "args":
+            default = ()
+        elif param.name == "kwargs":
+            default = {}
+        else:
+            default = param.default
+
         if isinstance(default, Depends):
             assert (
                 not dep
             ), "You can not use `Depends` with `Annotated` and default both"
             dep = default
 
         elif isinstance(default, CustomField):
@@ -142,14 +165,16 @@
         model=func_model,
         response_model=response_model,
         cast=cast,
         use_cache=use_cache,
         is_async=is_call_async,
         dependencies=dependencies,
         custom_fields=custom_fields,
+        positional_args=positional_args,
+        keyword_args=keyword_args,
         extra_dependencies=[
             build_call_model(
                 d.dependency,
                 cast=d.cast,
                 use_cache=d.use_cache,
                 is_sync=is_sync,
             )
```

### Comparing `fast_depends-2.0.5/fast_depends/core/model.py` & `fast_depends-2.1.0/fast_depends/core/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Callable,
     Dict,
     Generator,
     Generic,
     Iterable,
     List,
     Optional,
+    Tuple,
     Type,
     Union,
 )
 
 from typing_extensions import ParamSpec, TypeVar, assert_never
 
 from fast_depends._compat import PYDANTIC_V2, BaseModel, FieldInfo
@@ -43,19 +44,38 @@
 
     params: Dict[str, FieldInfo]
     alias_arguments: List[str]
 
     dependencies: Dict[str, "CallModel[..., Any]"]
     extra_dependencies: Iterable["CallModel[..., Any]"]
     custom_fields: Dict[str, CustomField]
+    keyword_args: Tuple[str]
+    positional_args: Tuple[str]
 
     # Dependencies and custom fields
     use_cache: bool
     cast: bool
 
+    __slots__ = (
+        "call",
+        "is_async",
+        "is_generator",
+        "model",
+        "response_model",
+        "params",
+        "alias_arguments",
+        "keyword_args",
+        "positional_args",
+        "dependencies",
+        "extra_dependencies",
+        "custom_fields",
+        "use_cache",
+        "cast",
+    )
+
     @property
     def call_name(self) -> str:
         return getattr(self.call, "__name__", type(self.call).__name__)
 
     @property
     def real_params(self) -> Dict[str, FieldInfo]:
         params = self.params.copy()
@@ -79,14 +99,16 @@
         model: Type[BaseModel],
         response_model: Optional[Type[BaseModel]] = None,
         use_cache: bool = True,
         cast: bool = True,
         is_async: bool = False,
         dependencies: Optional[Dict[str, "CallModel[..., Any]"]] = None,
         extra_dependencies: Optional[Iterable["CallModel[..., Any]"]] = None,
+        keyword_args: Optional[List[str]] = None,
+        positional_args: Optional[List[str]] = None,
         custom_fields: Optional[Dict[str, CustomField]] = None,
     ):
         self.call = call
         self.model = model
         self.response_model = response_model
 
         fields: Dict[str, FieldInfo]
@@ -96,14 +118,16 @@
             fields = self.model.__fields__  # type: ignore
 
         self.dependencies = dependencies or {}
         self.extra_dependencies = extra_dependencies or []
         self.custom_fields = custom_fields or {}
 
         self.alias_arguments = [f.alias or name for name, f in fields.items()]
+        self.keyword_args = tuple(keyword_args or [])
+        self.positional_args = tuple(positional_args or [])
 
         self.params = fields.copy()
         for name in self.dependencies.keys():
             self.params.pop(name, None)
 
         self.use_cache = use_cache
         self.cast = cast
@@ -148,21 +172,28 @@
         kw = args_to_kwargs(self.alias_arguments, *args, **kwargs)
 
         solved_kw: Dict[str, Any]
         solved_kw = yield kw
 
         casted_model = self.model(**solved_kw)
 
-        casted_kw = {
+        args_ = [
+            getattr(casted_model, arg, solved_kw.get(arg))
+            for arg in self.positional_args
+        ]
+        args_.extend(getattr(casted_model, "args", ()))
+
+        kwargs_ = {
             arg: getattr(casted_model, arg, solved_kw.get(arg))
-            for arg in (*self.params.keys(), *self.dependencies.keys())
+            for arg in self.keyword_args
         }
+        kwargs_.update(getattr(casted_model, "kwargs", {}))
 
         response: T
-        response = yield casted_kw
+        response = yield args_, kwargs_
 
         if self.cast is True and self.response_model is not None:
             casted_resp = self.response_model(response=response)
             response = casted_resp.response  # type: ignore
 
         if self.use_cache:  # pragma: no branch
             cache_dependencies[self.call] = response
@@ -221,24 +252,25 @@
                 dependency_overrides=dependency_overrides,
                 **kwargs,
             )
 
         for custom in self.custom_fields.values():
             kwargs = custom.use(**kwargs)
 
-        final_kw = cast_gen.send(kwargs)
+        final_args, final_kwargs = cast_gen.send(kwargs)
 
         if self.is_generator:
             response = solve_generator_sync(
+                *final_args,
                 call=self.call,
                 stack=stack,
-                **final_kw,
+                **final_kwargs,
             )
         else:
-            response = self.call(**final_kw)
+            response = self.call(*final_args, **final_kwargs)
 
         try:
             cast_gen.send(response)
         except StopIteration as e:
             value: T = e.value
             return value
 
@@ -296,24 +328,25 @@
                 dependency_overrides=dependency_overrides,
                 **kwargs,
             )
 
         for custom in self.custom_fields.values():
             kwargs = await run_async(custom.use, **kwargs)
 
-        final_kw = cast_gen.send(kwargs)
+        final_args, final_kwargs = cast_gen.send(kwargs)
 
         if self.is_generator:
             response = await solve_generator_async(
+                *final_args,
                 call=self.call,
                 stack=stack,
-                **final_kw,
+                **final_kwargs,
             )
         else:
-            response = await run_async(self.call, **final_kw)
+            response = await run_async(self.call, *final_args, **final_kwargs)
 
         try:
             cast_gen.send(response)
         except StopIteration as e:
             value: T = e.value
             return value
```

### Comparing `fast_depends-2.0.5/fast_depends/dependencies/model.py` & `fast_depends-2.1.0/fast_depends/dependencies/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/fast_depends/library/model.py` & `fast_depends-2.1.0/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/LICENSE` & `fast_depends-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/README.md` & `fast_depends-2.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -25,35 +25,42 @@
 ---
 
 Documentation: https://lancetnik.github.io/FastDepends/
 
 ---
 
 FastDepends - FastAPI Dependency Injection system extracted from FastAPI and cleared of all HTTP logic.
-This is a small library which provides you with the ability to use lovely Fastapi interfaces in your own
+This is a small library which provides you with the ability to use lovely FastAPI interfaces in your own
 projects or tools.
 
 Thanks to [*fastapi*](https://fastapi.tiangolo.com/) and [*pydantic*](https://docs.pydantic.dev/) projects for this
-greate functionality. This package is just a small change of the original Fastapi sources to provide DI functionality in a pyre-Python way.
+greate functionality. This package is just a small change of the original FastAPI sources to provide DI functionality in a pyre-Python way.
 
 Async and sync modes are both supported.
 
+# For why?
+
+This project should be extreamly helpfull to boost your not-**FastAPI** applications (even **Flask**, I know that u like some legacy).
+
+Also the project can be a core of your own framework for anything. Actually, it was build for my another project - :rocket:[**Propan**](https://github.com/Lancetnik/Propan):rocket:, check it to see full-featured **FastDepends** usage example.
+
 ## Installation
 
 ```bash
 pip install fast-depends
 ```
 
 ## Usage
 
 There is no way to make Dependency Injection easier
 
 You can use this library without any frameworks in both **sync** and **async** code.
 
 ### Async code
+
 ```python
 import asyncio
 
 from fast_depends import inject, Depends
 
 async def dependency(a: int) -> int:
     return a
@@ -66,14 +73,15 @@
 ) -> float:
     return a + b + c
 
 assert asyncio.run(main("1", 2)) == 4.0
 ```
 
 ### Sync code
+
 ```python
 from fast_depends import inject, Depends
 
 def dependency(a: int) -> int:
     return a
 
 @inject
@@ -97,15 +105,15 @@
 
 ### Features
 
 Synchronous code is fully supported in this package: without any `async_to_sync`, `run_sync`, `syncify` or any other tricks.
 
 Also, *FastDepends* casts functions' return values the same way, it can be very helpful in building your own tools.
 
-These are two main defferences from native Fastapi DI System.
+These are two main defferences from native FastAPI DI System.
 
 ---
 
 ### Custom Fields
 
 If you wish to write your own FastAPI or another closely by architecture tool, you should define your own custom fields to specify application behavior.
```

### Comparing `fast_depends-2.0.5/pyproject.toml` & `fast_depends-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.5/PKG-INFO` & `fast_depends-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 2.0.5
+Version: 2.1.0
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -78,35 +78,42 @@
 ---
 
 Documentation: https://lancetnik.github.io/FastDepends/
 
 ---
 
 FastDepends - FastAPI Dependency Injection system extracted from FastAPI and cleared of all HTTP logic.
-This is a small library which provides you with the ability to use lovely Fastapi interfaces in your own
+This is a small library which provides you with the ability to use lovely FastAPI interfaces in your own
 projects or tools.
 
 Thanks to [*fastapi*](https://fastapi.tiangolo.com/) and [*pydantic*](https://docs.pydantic.dev/) projects for this
-greate functionality. This package is just a small change of the original Fastapi sources to provide DI functionality in a pyre-Python way.
+greate functionality. This package is just a small change of the original FastAPI sources to provide DI functionality in a pyre-Python way.
 
 Async and sync modes are both supported.
 
+# For why?
+
+This project should be extreamly helpfull to boost your not-**FastAPI** applications (even **Flask**, I know that u like some legacy).
+
+Also the project can be a core of your own framework for anything. Actually, it was build for my another project - :rocket:[**Propan**](https://github.com/Lancetnik/Propan):rocket:, check it to see full-featured **FastDepends** usage example.
+
 ## Installation
 
 ```bash
 pip install fast-depends
 ```
 
 ## Usage
 
 There is no way to make Dependency Injection easier
 
 You can use this library without any frameworks in both **sync** and **async** code.
 
 ### Async code
+
 ```python
 import asyncio
 
 from fast_depends import inject, Depends
 
 async def dependency(a: int) -> int:
     return a
@@ -119,14 +126,15 @@
 ) -> float:
     return a + b + c
 
 assert asyncio.run(main("1", 2)) == 4.0
 ```
 
 ### Sync code
+
 ```python
 from fast_depends import inject, Depends
 
 def dependency(a: int) -> int:
     return a
 
 @inject
@@ -150,15 +158,15 @@
 
 ### Features
 
 Synchronous code is fully supported in this package: without any `async_to_sync`, `run_sync`, `syncify` or any other tricks.
 
 Also, *FastDepends* casts functions' return values the same way, it can be very helpful in building your own tools.
 
-These are two main defferences from native Fastapi DI System.
+These are two main defferences from native FastAPI DI System.
 
 ---
 
 ### Custom Fields
 
 If you wish to write your own FastAPI or another closely by architecture tool, you should define your own custom fields to specify application behavior.
```

