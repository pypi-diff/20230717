# Comparing `tmp/fast_depends-2.1.0.tar.gz` & `tmp/fast_depends-2.1.1.tar.gz`

## Comparing `fast_depends-2.1.0.tar` & `fast_depends-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.1.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.1.0/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.1.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/_compat.py
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/use.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/core/__init__.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/core/build.py
--rw-r--r--   0        0        0    10029 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/core/model.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/dependencies/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/dependencies/model.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/dependencies/provider.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.1.0/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.1.0/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.1.0/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.1.0/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.1.0/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.1.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.1.0/LICENSE
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fast_depends-2.1.0/README.md
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 fast_depends-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 fast_depends-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.1.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.1.1/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.1.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/__init__.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/_compat.py
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/use.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/core/build.py
+-rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/core/model.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.1.1/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.1.1/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.1.1/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.1.1/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.1.1/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.1.1/LICENSE
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fast_depends-2.1.1/README.md
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 fast_depends-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 fast_depends-2.1.1/PKG-INFO
```

### Comparing `fast_depends-2.1.0/CONTRIBUTING.md` & `fast_depends-2.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/.github/workflows/documentation.yml` & `fast_depends-2.1.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/.github/workflows/publish_coverage.yml` & `fast_depends-2.1.1/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/.github/workflows/publish_pypi.yml` & `fast_depends-2.1.1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/.github/workflows/tests.yml` & `fast_depends-2.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/fast_depends/_compat.py` & `fast_depends-2.1.1/fast_depends/_compat.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/fast_depends/use.py` & `fast_depends-2.1.1/fast_depends/use.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/fast_depends/utils.py` & `fast_depends-2.1.1/fast_depends/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -60,39 +60,14 @@
 def solve_generator_sync(
     *sub_args: Any, call: Callable[..., Any], stack: ExitStack, **sub_values: Any
 ) -> Any:
     cm = contextmanager(call)(*sub_args, **sub_values)
     return stack.enter_context(cm)
 
 
-def args_to_kwargs(
-    arguments: Iterable[str], *args: Any, **kwargs: Any
-) -> Dict[str, Any]:
-    arguments = tuple(filter(lambda i: i not in ("args", "kwargs"), arguments))
-
-    if not args:
-        return kwargs
-
-    merged = {"kwargs": kwargs.get("kwargs", {})}
-
-    for arg, v in kwargs.items():
-        if arg not in arguments:
-            merged["kwargs"][arg] = v
-        else:
-            merged[arg] = v
-
-    for arg in filter(lambda x: x not in merged, arguments):
-        if args:
-            merged[arg], args = args[0], args[1:]
-
-    merged["args"] = args
-
-    return merged
-
-
 def get_typed_signature(
     call: Callable[..., Any]
 ) -> Tuple[List[inspect.Parameter], Any]:
     signature = inspect.signature(call)
     globalns = getattr(call, "__globals__", {})
 
     return [
```

### Comparing `fast_depends-2.1.0/fast_depends/core/build.py` & `fast_depends-2.1.1/fast_depends/core/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,14 @@
 
     class_fields: Dict[str, Tuple[Any, Any]] = {}
     dependencies: Dict[str, CallModel[..., Any]] = {}
     custom_fields: Dict[str, CustomField] = {}
     positional_args: List[str] = []
     keyword_args: List[str] = []
     for param in typed_params:
-        if param.kind is param.KEYWORD_ONLY:
-            keyword_args.append(param.name)
-        elif param.name not in ("args", "kwargs"):
-            positional_args.append(param.name)
-
         dep: Optional[Depends] = None
         custom: Optional[CustomField] = None
 
         if param.annotation is inspect._empty:
             annotation = Any
 
         elif get_origin(param.annotation) is Annotated:
@@ -130,30 +125,38 @@
                 cast=dep.cast,
                 use_cache=dep.use_cache,
                 is_sync=is_sync,
             )
 
             if dep.cast is True:
                 class_fields[param.name] = (annotation, ...)
+            keyword_args.append(param.name)
 
-        if custom:
+        elif custom:
             assert not (
                 is_sync and is_coroutine_callable(custom.use)
             ), f"You cannot use async custom field `{type(custom).__name__}` at sync `{name}`"
 
             custom.set_param_name(param.name)
             custom_fields[param.name] = custom
 
             if custom.cast is False:
                 annotation = Any
 
             if custom.required:
                 class_fields[param.name] = (annotation, ...)
             else:
                 class_fields[param.name] = (Optional[annotation], None)
+            keyword_args.append(param.name)
+
+        else:
+            if param.kind is param.KEYWORD_ONLY:
+                keyword_args.append(param.name)
+            elif param.name not in ("args", "kwargs"):
+                positional_args.append(param.name)
 
     func_model = create_model(name, **class_fields)  # type: ignore
 
     if cast and return_annotation is not inspect._empty:
         response_model = create_model(
             "ResponseModel", response=(return_annotation, ...)
         )
```

### Comparing `fast_depends-2.1.0/fast_depends/core/model.py` & `fast_depends-2.1.1/fast_depends/core/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from contextlib import AsyncExitStack, ExitStack
+import inspect
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     Generator,
     Generic,
@@ -15,15 +16,14 @@
 )
 
 from typing_extensions import ParamSpec, TypeVar, assert_never
 
 from fast_depends._compat import PYDANTIC_V2, BaseModel, FieldInfo
 from fast_depends.library import CustomField
 from fast_depends.utils import (
-    args_to_kwargs,
     is_async_gen_callable,
     is_coroutine_callable,
     is_gen_callable,
     run_async,
     solve_generator_async,
     solve_generator_sync,
 )
@@ -165,33 +165,63 @@
             assert self.is_async or not is_coroutine_callable(
                 self.call
             ), f"You cannot use async dependency `{self.call_name}` at sync main"
 
         if self.use_cache and self.call in cache_dependencies:
             return cache_dependencies[self.call]
 
-        kw = args_to_kwargs(self.alias_arguments, *args, **kwargs)
+        kw = {}
+
+        for arg in self.keyword_args:
+            v = kwargs.pop(arg, inspect._empty)
+            if v is not inspect._empty:
+                kw[arg] = v
+
+        if "kwargs" in self.alias_arguments:
+            kw["kwargs"] = kwargs
+
+        else:
+            kw.update(kwargs)
+
+        has_args = "args" in self.alias_arguments
+
+        for arg in self.positional_args:
+            if args:
+                kw[arg], args = args[0], args[1:]
+
+        if has_args:
+            kw["args"] = args
+
+        else:
+            for arg in self.keyword_args:
+                if args:
+                    kw[arg], args = args[0], args[1:]
 
         solved_kw: Dict[str, Any]
         solved_kw = yield kw
 
         casted_model = self.model(**solved_kw)
 
-        args_ = [
-            getattr(casted_model, arg, solved_kw.get(arg))
-            for arg in self.positional_args
-        ]
-        args_.extend(getattr(casted_model, "args", ()))
-
         kwargs_ = {
             arg: getattr(casted_model, arg, solved_kw.get(arg))
-            for arg in self.keyword_args
+            for arg in (
+                self.keyword_args + self.positional_args if not has_args else self.keyword_args
+            )
         }
         kwargs_.update(getattr(casted_model, "kwargs", {}))
 
+        if has_args:
+            args_ = [
+                getattr(casted_model, arg, solved_kw.get(arg))
+                for arg in self.positional_args
+            ]
+            args_.extend(getattr(casted_model, "args", ()))
+        else:
+            args_ = ()
+
         response: T
         response = yield args_, kwargs_
 
         if self.cast is True and self.response_model is not None:
             casted_resp = self.response_model(response=response)
             response = casted_resp.response  # type: ignore
```

### Comparing `fast_depends-2.1.0/fast_depends/dependencies/model.py` & `fast_depends-2.1.1/fast_depends/dependencies/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/fast_depends/library/model.py` & `fast_depends-2.1.1/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/LICENSE` & `fast_depends-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/README.md` & `fast_depends-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/pyproject.toml` & `fast_depends-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.0/PKG-INFO` & `fast_depends-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 2.1.0
+Version: 2.1.1
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

