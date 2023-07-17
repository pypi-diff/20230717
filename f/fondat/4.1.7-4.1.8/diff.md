# Comparing `tmp/fondat-4.1.7.tar.gz` & `tmp/fondat-4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat-4.1.7.tar", max compression
+gzip compressed data, was "fondat-4.1.8.tar", max compression
```

## Comparing `fondat-4.1.7.tar` & `fondat-4.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.7/LICENSE
--rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.7/README.md
--rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.7/fondat/annotation.py
--rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.7/fondat/asgi.py
--rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.7/fondat/cache.py
--rw-r--r--   0        0        0    47781 2023-05-27 21:00:56.141881 fondat-4.1.7/fondat/codec.py
--rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.7/fondat/context.py
--rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.7/fondat/csv.py
--rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.7/fondat/data.py
--rw-r--r--   0        0        0     2444 2023-07-11 20:44:25.310120 fondat-4.1.7/fondat/error.py
--rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.7/fondat/file.py
--rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.7/fondat/http.py
--rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.7/fondat/lazy.py
--rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.7/fondat/memory.py
--rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.7/fondat/monitor.py
--rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.7/fondat/oauth.py
--rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.7/fondat/openapi.py
--rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.7/fondat/pagination.py
--rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.7/fondat/patch.py
--rw-r--r--   0        0        0    11552 2023-07-11 21:43:50.415822 fondat-4.1.7/fondat/resource.py
--rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.7/fondat/security.py
--rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.7/fondat/sql.py
--rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.7/fondat/sqlite.py
--rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.7/fondat/stream.py
--rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.7/fondat/string.py
--rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.7/fondat/types.py
--rw-r--r--   0        0        0    12793 2023-07-11 23:21:08.121362 fondat-4.1.7/fondat/validation.py
--rw-r--r--   0        0        0     1171 2023-07-11 23:21:44.151545 fondat-4.1.7/pyproject.toml
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 fondat-4.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.8/LICENSE
+-rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.8/README.md
+-rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.8/fondat/annotation.py
+-rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.8/fondat/asgi.py
+-rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.8/fondat/cache.py
+-rw-r--r--   0        0        0    47875 2023-07-16 23:51:26.184751 fondat-4.1.8/fondat/codec.py
+-rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.8/fondat/context.py
+-rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.8/fondat/csv.py
+-rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.8/fondat/data.py
+-rw-r--r--   0        0        0     2444 2023-07-11 20:44:25.310120 fondat-4.1.8/fondat/error.py
+-rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.8/fondat/file.py
+-rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.8/fondat/http.py
+-rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.8/fondat/lazy.py
+-rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.8/fondat/memory.py
+-rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.8/fondat/monitor.py
+-rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.8/fondat/oauth.py
+-rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.8/fondat/openapi.py
+-rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.8/fondat/pagination.py
+-rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.8/fondat/patch.py
+-rw-r--r--   0        0        0    11552 2023-07-11 21:43:50.415822 fondat-4.1.8/fondat/resource.py
+-rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.8/fondat/security.py
+-rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.8/fondat/sql.py
+-rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.8/fondat/sqlite.py
+-rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.8/fondat/stream.py
+-rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.8/fondat/string.py
+-rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.8/fondat/types.py
+-rw-r--r--   0        0        0    13873 2023-07-17 00:04:51.967963 fondat-4.1.8/fondat/validation.py
+-rw-r--r--   0        0        0     1171 2023-07-17 00:05:42.774849 fondat-4.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 fondat-4.1.8/PKG-INFO
```

### Comparing `fondat-4.1.7/LICENSE` & `fondat-4.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/README.md` & `fondat-4.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/annotation.py` & `fondat-4.1.8/fondat/annotation.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/asgi.py` & `fondat-4.1.8/fondat/asgi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/cache.py` & `fondat-4.1.8/fondat/cache.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/codec.py` & `fondat-4.1.8/fondat/codec.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,28 +90,33 @@
 class CodecError(ValueError):
     """
     Error raised in the event that a value cannot be decoded.
     """
 
     __slots__ = {"message", "path"}
 
-    def __init__(self, message: str | None = None, path: list[str | int] | None = None):
+    Path = list[str | int]
+
+    def __init__(self, message: str | None = None, path: Path | None = None):
         self.message = message
         self.path = path
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.message!r}, {self.path!r})"
 
     def __str__(self):
         return " ".join(str(s) for s in (self.message, self.path) if s is not None)
 
     @staticmethod
     @contextmanager
-    def path_on_error(path: list[str | int] | str | int) -> None:
-        """Context manager to add to error path in the event that a DecodeError is raised."""
+    def path_on_error(path: Path | str | int) -> None:
+        """
+        Execute within context that inserts a base error path if a CodecError is raised.
+        Base error path can be a full path or a single path segment.
+        """
         try:
             yield
         except CodecError as ce:
             if ce.path is None:
                 ce.path = []
             match path:
                 case str() | int():
```

### Comparing `fondat-4.1.7/fondat/context.py` & `fondat-4.1.8/fondat/context.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/csv.py` & `fondat-4.1.8/fondat/csv.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/data.py` & `fondat-4.1.8/fondat/data.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/error.py` & `fondat-4.1.8/fondat/error.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/file.py` & `fondat-4.1.8/fondat/file.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/http.py` & `fondat-4.1.8/fondat/http.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/lazy.py` & `fondat-4.1.8/fondat/lazy.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/memory.py` & `fondat-4.1.8/fondat/memory.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/monitor.py` & `fondat-4.1.8/fondat/monitor.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/oauth.py` & `fondat-4.1.8/fondat/oauth.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/openapi.py` & `fondat-4.1.8/fondat/openapi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/pagination.py` & `fondat-4.1.8/fondat/pagination.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/patch.py` & `fondat-4.1.8/fondat/patch.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/resource.py` & `fondat-4.1.8/fondat/resource.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/security.py` & `fondat-4.1.8/fondat/security.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/sql.py` & `fondat-4.1.8/fondat/sql.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/sqlite.py` & `fondat-4.1.8/fondat/sqlite.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/stream.py` & `fondat-4.1.8/fondat/stream.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/string.py` & `fondat-4.1.8/fondat/string.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/types.py` & `fondat-4.1.8/fondat/types.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.7/fondat/validation.py` & `fondat-4.1.8/fondat/validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,34 +24,39 @@
     • message: human-readable error message
     • path: path to the attribute that is the subject of the validation error
     • code: machine-readable error code
     """
 
     __slots__ = {"message", "path", "code"}
 
+    Path = list[str | int]
+
     def __init__(
         self,
         message: str | None = None,
-        path: list[str | int] | None = None,
+        path: Path | None = None,
         code: str | None = None,
     ):
         self.message = message
         self.path = path
         self.code = code
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.message!r}, {self.path!r}, {self.code!r})"
 
     def __str__(self):
         return self.message or self.code
 
     @staticmethod
     @contextmanager
-    def path_on_error(path: list[str | int] | str | int):
-        """Context manager to specify error path in the event that a DecodeError is raised."""
+    def path_on_error(path: Path | str | int):
+        """
+        Execute within context that inserts a base error path if a ValidationError is raised.
+        Base error path can be a full path or a single path segment.
+        """
         try:
             yield
         except ValidationError as ve:
             if ve.path is None:
                 ve.path = []
             match path:
                 case str() | int():
@@ -226,15 +231,15 @@
     for arg in args:
         if arg == value and type(arg) is type(value):
             return
     raise ValidationError(f"expecting one of: {args}; received: {value}")
 
 
 @contextmanager
-def validation_error_path(segment: Any):
+def validation_error_path(segment: str | int):
     try:
         yield
     except ValidationError as ve:
         ve.path = (ve.path or []).insert(0, segment)
         raise
 
 
@@ -291,15 +296,15 @@
     dc_type = python_type if not origin else origin
     with fondat.types.capture_typevars(python_type):
         for attr_name, attr_type in typing.get_type_hints(dc_type, include_extras=True).items():
             with validation_error_path(attr_name):
                 validate(getattr(value, attr_name), attr_type)
 
 
-def validate(value: Any, type_hint: Any) -> NoneType:
+def validate_value(value: Any, type_hint: Any) -> None:
     """Validate a value."""
 
     python_type, annotations = split_annotations(type_hint)
     origin = typing.get_origin(python_type)
     args = typing.get_args(python_type)
 
     # validate using specified validator annotations
@@ -341,14 +346,19 @@
         return _validate_tuple(value, python_type, args)
     elif is_subclass(origin, Iterable):
         return _validate_iterable(value, python_type, args)
     elif dataclasses.is_dataclass(python_type) or dataclasses.is_dataclass(origin):
         return _validate_dataclass(value, python_type, origin)
 
 
+def validate(value: Any, type_hint: Any) -> None:
+    """Deprecated. Use validate_value."""
+    validate_value(value, type_hint)
+
+
 def validate_arguments(callable: Callable):
     """Decorate a function or coroutine to validate its arguments using type annotations."""
 
     sig = inspect.signature(callable)
 
     positional_params = [
         p.name
@@ -419,7 +429,34 @@
     """Return if a value is valid for specified type."""
 
     try:
         validate(value, type_hint)
     except ValidationError:
         return False
     return True
+
+
+def validate_condition(
+    condition: bool,
+    *,
+    errors: ValidationErrors | None = None,
+    message: str | None = None,
+    path: ValidationError.Path | None = None,
+    code: str | None = None,
+) -> None:
+    """
+    Validate a condition. If the condition is false then a ValidationError is created. If an
+    errors object is specified, then the error is added to it; otherwise the ValidationError
+    is raised.
+
+    Parameters:
+    • errors: object to add error to
+    • message: human-readable error message
+    • path: path to the attribute that is the subject of the validation error
+    • code: machine-readable error code
+    """
+    if condition:  # validation passed
+        return
+    error = ValidationError(message=message, path=path, code=code)
+    if errors is None:
+        raise error
+    errors.add(error)
```

### Comparing `fondat-4.1.7/pyproject.toml` & `fondat-4.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat"
-version = "4.1.7"
+version = "4.1.8"
 description = "A foundation for resource-oriented backend applications."
 readme = "README.md"
 authors = ["fondat authors"]
 homepage = "https://github.com/fondat/fondat/"
 documentation = "https://github.com/fondat/fondat/tree/main/docs"
 license = "MIT"
 keywords = ["asgi", "foundation", "resource", "openapi"]
```

### Comparing `fondat-4.1.7/PKG-INFO` & `fondat-4.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fondat
-Version: 4.1.7
+Version: 4.1.8
 Summary: A foundation for resource-oriented backend applications.
 Home-page: https://github.com/fondat/fondat/
 License: MIT
 Keywords: asgi,foundation,resource,openapi
 Author: fondat authors
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

