# Comparing `tmp/pydantic_partial-0.3.4.tar.gz` & `tmp/pydantic_partial-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_partial-0.3.4.tar", max compression
+gzip compressed data, was "pydantic_partial-0.5.0.tar", max compression
```

## Comparing `pydantic_partial-0.3.4.tar` & `pydantic_partial-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1078 2023-03-08 13:55:08.167594 pydantic_partial-0.3.4/LICENSE
--rw-r--r--   0        0        0     3623 2023-03-08 13:55:08.167594 pydantic_partial-0.3.4/README.md
--rw-r--r--   0        0        0       61 2023-03-08 13:55:08.167594 pydantic_partial-0.3.4/pydantic_partial/__init__.py
--rw-r--r--   0        0        0     4910 2023-03-08 13:55:08.167594 pydantic_partial-0.3.4/pydantic_partial/partial.py
--rw-r--r--   0        0        0        0 2023-03-08 13:55:08.167594 pydantic_partial-0.3.4/pydantic_partial/py.typed
--rw-r--r--   0        0        0      507 2023-03-08 13:55:08.167594 pydantic_partial-0.3.4/pydantic_partial/utils.py
--rw-r--r--   0        0        0      891 2023-03-08 13:55:08.167594 pydantic_partial-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4344 1970-01-01 00:00:00.000000 pydantic_partial-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-17 12:23:45.648156 pydantic_partial-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5597 2023-07-17 12:23:45.648156 pydantic_partial-0.5.0/README.md
+-rw-r--r--   0        0        0       61 2023-07-17 12:23:45.648156 pydantic_partial-0.5.0/pydantic_partial/__init__.py
+-rw-r--r--   0        0        0     2295 2023-07-17 12:23:45.648156 pydantic_partial-0.5.0/pydantic_partial/_compat.py
+-rw-r--r--   0        0        0     5615 2023-07-17 12:23:45.648156 pydantic_partial-0.5.0/pydantic_partial/partial.py
+-rw-r--r--   0        0        0        0 2023-07-17 12:23:45.648156 pydantic_partial-0.5.0/pydantic_partial/py.typed
+-rw-r--r--   0        0        0      691 2023-07-17 12:23:45.648156 pydantic_partial-0.5.0/pydantic_partial/utils.py
+-rw-r--r--   0        0        0      915 2023-07-17 12:23:45.648156 pydantic_partial-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 pydantic_partial-0.5.0/PKG-INFO
```

### Comparing `pydantic_partial-0.3.4/LICENSE` & `pydantic_partial-0.5.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
-
```

### Comparing `pydantic_partial-0.3.4/README.md` & `pydantic_partial-0.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # pydantic-partial
 
 ## Installation
 
 Just use `pip install pydantic-partial` to install the library.
 
+**Note:** `pydantic-partial` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+Python `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
+using `tox`.
+
 ## About
 
 Create partial models from your normal pydantic models. Partial models will allow
 some or all fields to be optional and thus not be required when creating the model
 instance.
 
 Partial models can be used to support PATCH HTTP requests where the user only wants
@@ -32,16 +36,16 @@
 # Something model, then can be used as a partial, too:
 class Something(PartialModelMixin, pydantic.BaseModel):
     name: str
     age: int
 
 
 # Create a full partial model
-FullSomethingPartial = Something.as_partial()
-FullSomethingPartial(name=None, age=None)
+FullSomethingPartial = Something.model_as_partial()
+FullSomethingPartial()  # Same as FullSomethingPartial(name=None, age=None)
 ```
 
 ### Without using the mixin
 
 You also may create partial models without using the mixin:
 
 ```python
@@ -52,15 +56,15 @@
 class Something(pydantic.BaseModel):
     name: str
     age: int
 
 
 # Create a full partial model
 FullSomethingPartial = create_partial_model(Something)
-FullSomethingPartial(name=None, age=None)
+FullSomethingPartial()  # Same as FullSomethingPartial(name=None, age=None)
 ```
 
 ### Only changing some fields to being optional
 
 `pydantic-partial` can be used to create partial models that only change some
 of the fields to being optional. Just pass the list of fields to be optional to
 the `as_partial()` or `create_partial_model()` function.
@@ -71,16 +75,16 @@
 
 class Something(pydantic.BaseModel):
     name: str
     age: int
 
 # Create a partial model only for the name attribute
 FullSomethingPartial = create_partial_model(Something, 'name')
-FullSomethingPartial(name=None)
-# This would still raise an error: FullSomethingPartial(age=None)
+FullSomethingPartial(age=40)  # Same as FullSomethingPartial(name=None, age=40)
+# This would still raise an error: FullSomethingPartial(age=None, ...)
 ```
 
 ### Recursive partials
 
 Partial models can be created changing the field of all nested models to being
 optional, too.
 
@@ -108,13 +112,41 @@
 `pydantic-partial` will not be able to detect which fields may allow to being
 converted to partial models.
 
 **Also note:** My recommendation would be to always create such recursive
 partials by creating partials for all the required models and then override
 the fields on you outer partial model class. This is way more explicit.
 
+## Known limitations
+
+`pydantic-partial` cannot generate new class types that actually are supported by the
+Python typing system rules. This means that the partial models will only be recognized
+as the same as their original model classes - type checkers will not know about the partial
+model changes and thus will think all those partial fields are still required.
+
+This is due to the fact that Python itself has no concept of partials. `pydantic-partial`
+could (in theory) provide plugins for `mypy` for example to "patch" this in, but this would
+be a massive amount of work while being kind of a bad hack. The real solution would be to
+have a partial type in Python itself, but this is not planned for the near future as far
+as I know.
+
+My recommendation is to use `pydantic-partial` only for API use cases where you do not
+need to work with the partial aspects of the models - they are just the DTOs (data transfer
+objects) you are using. If you need to use partial models in other cases you might get
+errors by your type checker - if you use one. Please be aware of this.
+
+**Note:** Not having a good solution in Python itself for this is the reason `pydantic` does
+not support partial models in the first place. `pydantic-partial` is just a really good
+workaround for this issue.  
+See [issue 2](https://github.com/team23/pydantic-partial/issues/2) in this project and
+[issue 1673](https://github.com/pydantic/pydantic/issues/1673#issuecomment-1557267229)
+in the `pydantic` project for reference.
+
+Having that all said: If anyone wants to get a working plugin for `mypy` or others ready,
+I'm going to very much support this.
+
 # Contributing
 
 If you want to contribute to this project, feel free to just fork the project,
 create a dev branch in your fork and then create a pull request (PR). If you
 are unsure about whether your changes really suit the project please create an
 issue first, to talk about this.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydantic_partial-0.3.4/pydantic_partial/partial.py` & `pydantic_partial-0.5.0/pydantic_partial/partial.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,105 +21,106 @@
 FullSomethingPartial(name=None, age=None)
 # You could also create a "partial Partial":
 #AgeSomethingPartial = Something.as_partial("age")
 ```
 """
 
 import functools
-from typing import Any, Dict, List, Optional, Type, TypeVar, Union, get_args, get_origin
+import warnings
+from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union, get_args, get_origin
 
 import pydantic
 
-from .utils import copy_field_info
+from ._compat import PydanticCompat
 
 SelfT = TypeVar("SelfT", bound=pydantic.BaseModel)
+ModelSelfT = TypeVar("ModelSelfT", bound="PartialModelMixin")
 
 
 @functools.lru_cache(maxsize=None, typed=True)
 def create_partial_model(
     base_cls: Type[SelfT],
     *fields: str,
     recursive: bool = False,
 ) -> Type[SelfT]:
     # Convert one type to being partial - if possible
-    def _partial_type(field_name_: str, field_type_: Type) -> Type:
+    def _partial_annotation_arg(field_name_: str, field_annotation: Type) -> Type:
         if (
-                isinstance(field_type_, type)
-                and issubclass(field_type_, PartialModelMixin)
+                isinstance(field_annotation, type)
+                and issubclass(field_annotation, PartialModelMixin)
         ):
             field_prefix = f"{field_name_}."
             children_fields = [
                 field.removeprefix(field_prefix)
                 for field
                 in fields_
                 if field.startswith(field_prefix)
             ]
             if children_fields == ["*"]:
                 children_fields = []
-            return field_type_.as_partial(*children_fields, recursive=recursive)
+            return field_annotation.model_as_partial(*children_fields, recursive=recursive)
         else:
-            return field_type_
+            return field_annotation
+
+    model_compat = PydanticCompat(base_cls)
 
     # By default make all fields optional, but use passed fields when possible
     if fields:
         fields_ = list(fields)
     else:
-        fields_ = list(base_cls.__fields__.keys())
+        fields_ = list(model_compat.model_fields.keys())
 
     # Construct list of optional new field overrides
     optional_fields: dict[str, Any] = {}
-    for field_name in base_cls.__fields__.keys():
-        field_type = base_cls.__fields__[field_name].outer_type_
-        if field_type is None:
-            continue
+    for field_name, field_info in model_compat.model_fields.items():
+        field_annotation = model_compat.get_model_field_info_annotation(field_info)
+        if field_annotation is None:  # pragma: no cover
+            continue  # This is just to handle edge cases for pydantic 1.x - can be removed in pydantic 2.0
 
         # Do we have any fields starting with $FIELD_NAME + "."?
-        has_sub_fields = any(
+        sub_fields_requested = any(
             field.startswith(f"{field_name}.")
             for field
             in fields_
         )
 
         # Continue if this field needs not to be handled
-        if field_name not in fields_ and not has_sub_fields:
+        if field_name not in fields_ and not sub_fields_requested:
             continue
 
         # Change type for sub models, if requested
-        if recursive or has_sub_fields:
-            field_type_origin = get_origin(field_type)
-            if field_type_origin in (Union, list, List, dict, Dict):
-                field_type = field_type_origin[
+        if recursive or sub_fields_requested:
+            field_annotation_origin = get_origin(field_annotation)
+            if field_annotation_origin in (Union, list, Tuple, tuple, List, dict, Dict):
+                field_annotation = field_annotation_origin[
                     tuple(
-                        _partial_type(field_name, field_args_type)
-                        for field_args_type
-                        in get_args(field_type)
+                        _partial_annotation_arg(field_name, field_annotation_arg)
+                        for field_annotation_arg
+                        in get_args(field_annotation)
                     )
                 ]
             else:
-                field_type = _partial_type(field_name, field_type)
+                field_annotation = _partial_annotation_arg(field_name, field_annotation)
 
         # Construct new field definition
         if field_name in fields_:
-            if (
-                base_cls.__fields__[field_name].required
-                or base_cls.__fields__[field_name].default is not None
-            ):
+            if model_compat.is_model_field_info_required(field_info):
                 optional_fields[field_name] = (
-                    Optional[field_type],
-                    copy_field_info(
-                        base_cls.__fields__[field_name].field_info,
+                    Optional[field_annotation],
+                    model_compat.copy_model_field_info(
+                        field_info,
                         default=None,  # Set default to None
                         defaul_factory=None,  # Remove default_factory if set
                         nullable=True,  # For API usage
                     ),
                 )
-        elif recursive or has_sub_fields:
+        elif recursive or sub_fields_requested:
             optional_fields[field_name] = (
-                field_type,
-                copy_field_info(base_cls.__fields__[field_name].field_info),
+                field_annotation,
+                model_compat.copy_model_field_info(field_info),
             )
 
     # Return original model class if nothing has changed
     if not optional_fields:
         return base_cls
 
     # Generate new subclass model with those optional fields
@@ -133,13 +134,25 @@
 class PartialModelMixin(pydantic.BaseModel):
     """
     Partial model mixin. Will allow usage of `as_partial()` on the model class
     to create a partial version of the model class.
     """
 
     @classmethod
-    def as_partial(  # noqa: C901
-        cls: Type[SelfT],
+    def model_as_partial(
+        cls: Type[ModelSelfT],
         *fields: str,
         recursive: bool = False,
-    ) -> Type[SelfT]:
+    ) -> Type[ModelSelfT]:
         return create_partial_model(cls, *fields, recursive=recursive)
+
+    @classmethod
+    def as_partial(
+        cls: Type[ModelSelfT],
+        *fields: str,
+        recursive: bool = False,
+    ) -> Type[ModelSelfT]:
+        warnings.warn(
+            "as_partial(...) is deprecated, use model_as_partial(...) instead",
+            DeprecationWarning,
+        )
+        return cls.model_as_partial(*fields, recursive=recursive)
```

### Comparing `pydantic_partial-0.3.4/pyproject.toml` & `pydantic_partial-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "pydantic-partial"
-version = "0.3.4"
+version = "0.5.0"
 description = "Create partial models from your pydantic models. Partial models may allow None for certain or all fields."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-partial"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = ">=1.9.0,<2.0.0"
+pydantic = ">=1.9.0,<2.1.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.1.2"
+pytest = ">=7.1.2,<8.0.0"
 isort = "^5.10.1"
-mypy = ">=0.971,<1.1"
-flake8 = "^5.0.4"
-flake8-builtins = "^1.5.3"
+mypy = ">=0.971,<2.0"
+flake8 = ">=5.0.4,<7.0.0"
+flake8-builtins = ">=1.5.3,<3.0.0"
 flake8-annotations = ">=2.9.1,<4.0.0"
 flake8-commas = "^2.1.0"
 flake8-isort = ">=4.2,<7.0"
 flake8-print = "^5.0.0"
 flake8-debugger = "^4.1.2"
 pytest-cov = ">=3,<5"
 tox = ">=3.26,<5.0"
```

### Comparing `pydantic_partial-0.3.4/PKG-INFO` & `pydantic_partial-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: pydantic-partial
-Version: 0.3.4
+Version: 0.5.0
 Summary: Create partial models from your pydantic models. Partial models may allow None for certain or all fields.
 Home-page: https://github.com/team23/pydantic-partial
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: pydantic (>=1.9.0,<2.1.0)
 Project-URL: Repository, https://github.com/team23/pydantic-partial
 Description-Content-Type: text/markdown
 
 # pydantic-partial
 
 ## Installation
 
 Just use `pip install pydantic-partial` to install the library.
 
+**Note:** `pydantic-partial` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+Python `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
+using `tox`.
+
 ## About
 
 Create partial models from your normal pydantic models. Partial models will allow
 some or all fields to be optional and thus not be required when creating the model
 instance.
 
 Partial models can be used to support PATCH HTTP requests where the user only wants
@@ -50,16 +54,16 @@
 # Something model, then can be used as a partial, too:
 class Something(PartialModelMixin, pydantic.BaseModel):
     name: str
     age: int
 
 
 # Create a full partial model
-FullSomethingPartial = Something.as_partial()
-FullSomethingPartial(name=None, age=None)
+FullSomethingPartial = Something.model_as_partial()
+FullSomethingPartial()  # Same as FullSomethingPartial(name=None, age=None)
 ```
 
 ### Without using the mixin
 
 You also may create partial models without using the mixin:
 
 ```python
@@ -70,15 +74,15 @@
 class Something(pydantic.BaseModel):
     name: str
     age: int
 
 
 # Create a full partial model
 FullSomethingPartial = create_partial_model(Something)
-FullSomethingPartial(name=None, age=None)
+FullSomethingPartial()  # Same as FullSomethingPartial(name=None, age=None)
 ```
 
 ### Only changing some fields to being optional
 
 `pydantic-partial` can be used to create partial models that only change some
 of the fields to being optional. Just pass the list of fields to be optional to
 the `as_partial()` or `create_partial_model()` function.
@@ -89,16 +93,16 @@
 
 class Something(pydantic.BaseModel):
     name: str
     age: int
 
 # Create a partial model only for the name attribute
 FullSomethingPartial = create_partial_model(Something, 'name')
-FullSomethingPartial(name=None)
-# This would still raise an error: FullSomethingPartial(age=None)
+FullSomethingPartial(age=40)  # Same as FullSomethingPartial(name=None, age=40)
+# This would still raise an error: FullSomethingPartial(age=None, ...)
 ```
 
 ### Recursive partials
 
 Partial models can be created changing the field of all nested models to being
 optional, too.
 
@@ -126,14 +130,42 @@
 `pydantic-partial` will not be able to detect which fields may allow to being
 converted to partial models.
 
 **Also note:** My recommendation would be to always create such recursive
 partials by creating partials for all the required models and then override
 the fields on you outer partial model class. This is way more explicit.
 
+## Known limitations
+
+`pydantic-partial` cannot generate new class types that actually are supported by the
+Python typing system rules. This means that the partial models will only be recognized
+as the same as their original model classes - type checkers will not know about the partial
+model changes and thus will think all those partial fields are still required.
+
+This is due to the fact that Python itself has no concept of partials. `pydantic-partial`
+could (in theory) provide plugins for `mypy` for example to "patch" this in, but this would
+be a massive amount of work while being kind of a bad hack. The real solution would be to
+have a partial type in Python itself, but this is not planned for the near future as far
+as I know.
+
+My recommendation is to use `pydantic-partial` only for API use cases where you do not
+need to work with the partial aspects of the models - they are just the DTOs (data transfer
+objects) you are using. If you need to use partial models in other cases you might get
+errors by your type checker - if you use one. Please be aware of this.
+
+**Note:** Not having a good solution in Python itself for this is the reason `pydantic` does
+not support partial models in the first place. `pydantic-partial` is just a really good
+workaround for this issue.  
+See [issue 2](https://github.com/team23/pydantic-partial/issues/2) in this project and
+[issue 1673](https://github.com/pydantic/pydantic/issues/1673#issuecomment-1557267229)
+in the `pydantic` project for reference.
+
+Having that all said: If anyone wants to get a working plugin for `mypy` or others ready,
+I'm going to very much support this.
+
 # Contributing
 
 If you want to contribute to this project, feel free to just fork the project,
 create a dev branch in your fork and then create a pull request (PR). If you
 are unsure about whether your changes really suit the project please create an
 issue first, to talk about this.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

