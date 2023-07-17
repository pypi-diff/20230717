# Comparing `tmp/runtype-0.3.4.tar.gz` & `tmp/runtype-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtype-0.3.4.tar", max compression
+gzip compressed data, was "runtype-0.3.5.tar", max compression
```

## Comparing `runtype-0.3.4.tar` & `runtype-0.3.5.tar`

### file list

```diff
@@ -1,18 +1,16 @@
--rw-r--r--   0        0        0     1089 2021-12-14 13:06:00.725082 runtype-0.3.4/LICENSE
--rw-r--r--   0        0        0     1196 2023-06-26 18:01:02.868453 runtype-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4098 2022-10-11 13:06:17.811390 runtype-0.3.4/README.md
--rw-r--r--   0        0        0     1536 2023-06-26 18:01:12.615266 runtype-0.3.4/runtype/__init__.py
--rw-r--r--   0        0        0     9279 2022-10-11 12:52:05.446440 runtype-0.3.4/runtype/base_types.py
--rw-r--r--   0        0        0       57 2021-12-14 13:06:00.733081 runtype-0.3.4/runtype/common.py
--rw-r--r--   0        0        0    14069 2023-06-26 17:57:05.431591 runtype-0.3.4/runtype/dataclass.py
--rw-r--r--   0        0        0     8098 2021-12-14 13:06:00.734037 runtype-0.3.4/runtype/datetime_parse.py
--rw-r--r--   0        0        0     6139 2023-06-26 17:57:05.433587 runtype-0.3.4/runtype/dispatch.py
--rw-r--r--   0        0        0      823 2023-04-17 13:00:48.914621 runtype-0.3.4/runtype/mypy.py
--rw-r--r--   0        0        0     3115 2022-06-25 08:55:10.918634 runtype-0.3.4/runtype/mypy_bu.py
--rw-r--r--   0        0        0        0 2022-10-11 12:52:05.449333 runtype-0.3.4/runtype/py.typed
--rw-r--r--   0        0        0    15604 2023-06-26 17:57:05.437588 runtype-0.3.4/runtype/pytypes.py
--rw-r--r--   0        0        0      552 2023-05-29 19:21:24.002389 runtype-0.3.4/runtype/typesystem.py
--rw-r--r--   0        0        0     1379 2023-04-17 13:00:48.921619 runtype-0.3.4/runtype/utils.py
--rw-r--r--   0        0        0     3520 2023-05-30 09:42:18.890424 runtype-0.3.4/runtype/validation.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 runtype-0.3.4/setup.py
--rw-r--r--   0        0        0     5194 1970-01-01 00:00:00.000000 runtype-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1089 2021-12-14 13:06:00.725082 runtype-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1196 2023-07-17 07:59:27.132373 runtype-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4694 2023-07-16 07:45:34.785695 runtype-0.3.5/README.md
+-rw-r--r--   0        0        0     1536 2023-07-17 07:54:41.139358 runtype-0.3.5/runtype/__init__.py
+-rw-r--r--   0        0        0     9478 2023-07-16 07:45:34.749691 runtype-0.3.5/runtype/base_types.py
+-rw-r--r--   0        0        0       57 2021-12-14 13:06:00.733081 runtype-0.3.5/runtype/common.py
+-rw-r--r--   0        0        0    16041 2023-07-16 07:45:34.750692 runtype-0.3.5/runtype/dataclass.py
+-rw-r--r--   0        0        0     7039 2023-07-16 07:45:34.750692 runtype-0.3.5/runtype/datetime_parse.py
+-rw-r--r--   0        0        0     6268 2023-07-16 07:45:34.751693 runtype-0.3.5/runtype/dispatch.py
+-rw-r--r--   0        0        0        0 2022-10-11 12:52:05.449333 runtype-0.3.5/runtype/py.typed
+-rw-r--r--   0        0        0    17013 2023-07-16 07:45:34.752693 runtype-0.3.5/runtype/pytypes.py
+-rw-r--r--   0        0        0      552 2023-05-29 19:21:24.002389 runtype-0.3.5/runtype/typesystem.py
+-rw-r--r--   0        0        0     1379 2023-04-17 13:00:48.921619 runtype-0.3.5/runtype/utils.py
+-rw-r--r--   0        0        0     3520 2023-05-30 09:42:18.890424 runtype-0.3.5/runtype/validation.py
+-rw-r--r--   0        0        0     5510 1970-01-01 00:00:00.000000 runtype-0.3.5/setup.py
+-rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 runtype-0.3.5/PKG-INFO
```

### Comparing `runtype-0.3.4/LICENSE` & `runtype-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `runtype-0.3.4/pyproject.toml` & `runtype-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "runtype"
-version = "0.3.4"
+version = "0.3.5"
 description = "Type dispatch and validation for run-time Python"
 authors = ["Erez Shinan <erezshin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/erezsh/runtype"
 keywords = ["types", "typing", "dispatch", "multimethods", "dataclass", "runtime"]
 classifiers = [
```

### Comparing `runtype-0.3.4/README.md` & `runtype-0.3.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 pip install runtype
 ```
 
 No dependencies.
 
 Requires Python 3.6 or up.
 
-[![Build Status](https://travis-ci.org/erezsh/runtype.svg?branch=master)](https://travis-ci.org/erezsh/runtype)
 [![codecov](https://codecov.io/gh/erezsh/runtype/branch/master/graph/badge.svg)](https://codecov.io/gh/erezsh/runtype)
 
 ## Examples
 
 ### Validation (Isa & Subclass)
 
 ```python
@@ -125,14 +124,41 @@
 #> foobar
 print( append('foo', 4)     )
 # Traceback (most recent call last):
 #    ...
 # runtype.dispatch.DispatchError: Function 'append' not found for signature (<class 'str'>, <class 'int'>)
 ```
 
+Dispatch can also be used for extending the dataclass builtin `__init__`:
+
+```python
+dp = Dispatch()
+
+@dataclass(frozen=False)
+class Point:
+    x: int = 0
+    y: int = 0
+    
+    @dp
+    def __init__(self, points: list | tuple):
+        self.x, self.y = points
+
+    @dp
+    def __init__(self, points: dict):
+        self.x = points['x']
+        self.y = points['y']
+    
+# Test constructors
+p0 = Point()                         # Default constructor
+assert p0 == Point(0, 0)             # Default constructor
+assert p0 == Point([0, 0])           # User constructor
+assert p0 == Point((0, 0))           # User constructor
+assert p0 == Point({"x": 0, "y": 0}) # User constructor
+```
+
 
 ## License
 
 Runtype uses the [MIT license](LICENSE).
 
 ## Donate
```

### Comparing `runtype-0.3.4/runtype/__init__.py` & `runtype-0.3.5/runtype/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .dataclass import dataclass
 from .dispatch import DispatchError, MultiDispatch
 from .validation import (PythonTyping, TypeSystem, TypeMismatchError,
                          assert_isa, isa, issubclass, validate_func, is_subtype, cv_type_checking)
 from .pytypes import Constraint, String, Int
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 __all__ = (
     'dataclass',
     'DispatchError', 'MultiDispatch',
     'PythonTyping', 'TypeSystem', 'TypeMismatchError',
     'assert_isa', 'isa', 'issubclass', 'validate_func', 'is_subtype', 'cv_type_checking',
     'Constraint', 'String', 'Int',
     'Dispatch',
```

### Comparing `runtype-0.3.4/runtype/base_types.py` & `runtype-0.3.5/runtype/base_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 Base Type Classes - contains the basic building blocks of a generic type system
 
 We use comparison operators to indicate whether a type is a subtype of another:
  - t1 <= t2 means "t1 is a subtype of t2"
  - t1 >= t2 means "t2 is a subtype of t1"
 This is consistent with the view that a type hierarchy can be expressed as a poset.
 """
-from typing import Callable, Sequence, Optional
+from typing import Callable, Sequence, Optional, Union
 from abc import ABC, abstractmethod
 
 
 class RuntypeError(TypeError):
     pass
 
 
 class TypeMismatchError(RuntypeError):
     def __str__(self) -> str:
         v, t = self.args
         return f"Expected type '{t}', but got value: {v}."
 
+_Type = Union['Type', type]
 
-
-class Type:
+class Type(ABC):
     """Abstract Type class. All types inherit from it.
     """
-    def __add__(self, other):
+    def __add__(self, other: _Type):
         return SumType.create((self, other))
 
-    def __mul__(self, other):
+    def __mul__(self, other: _Type):
         return ProductType.create((self, other))
 
+    @abstractmethod
+    def __le__(self, other: _Type):
+        return NotImplemented
 
 class AnyType(Type):
     """Represents the Any type.
 
     For any type 't' within the typesystem, t is a subtype of Any (or: t <= Any)
     """
     def __add__(self, other):
@@ -163,16 +166,18 @@
 
 
 class GenericType(ContainerType):
     """Implements a generic type. i.e. a container for items of a specific type.
 
     For any two generic types a[i] and b[j], it's true that a[i] <= b[j] iff a <= b and i <= j.
     """
+    base: Type
+    item: Union[type, Type]
 
-    def __init__(self, base, item=Any):
+    def __init__(self, base: Type, item: Union[type, Type]=Any):
         assert isinstance(item, (Type, type)), item
         if isinstance(base, GenericType):
             if not item <= base.item:
                 raise TypeError(f"Expecting new generic to be a subtype of base, but {item} </= {base.item}")
             base = base.base
 
         self.base = base
@@ -289,15 +294,14 @@
     def validate_instance(self, obj, sampler: Optional[SamplerType]=None):
         """Validates obj, raising a TypeMismatchError if it does not conform.
 
         If sampler is provided, it will be applied to the instance in order to 
         validate only a sample of the object. This approach may validate much faster,
         but might miss anomalies in the data.
         """
-        ...
 
 
     def test_instance(self, obj, sampler=None):
         """Tests obj, returning a True/False for whether it conforms or not.
 
         If sampler is provided, it will be applied to the instance in order to 
         validate only a sample of the object.
```

### Comparing `runtype-0.3.4/runtype/dataclass.py` & `runtype-0.3.5/runtype/dataclass.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 """
 Enhances Python's built-in dataclass, with type-checking and extra ergonomics.
 """
 
 import random
 from copy import copy
 import dataclasses
-from typing import Union, Any, Tuple, Callable, TypeVar
+from typing import Union, Any, Callable, TypeVar, Dict, Optional, overload
+from typing import TYPE_CHECKING, ClassVar, Type
 from abc import ABC, abstractmethod
 import inspect
+import types
+
+if TYPE_CHECKING:
+    from typing_extensions import dataclass_transform
+else:
+    def dataclass_transform(*a, **kw):
+        return lambda f:f
 
 from .utils import ForwardRef
 from .common import CHECK_TYPES
 from .validation import TypeMismatchError, ensure_isa as default_ensure_isa
-from .pytypes import TypeCaster, SumType, NoneType, ATypeCaster
+from .pytypes import TypeCaster, SumType, NoneType, ATypeCaster, PythonType, type_caster
 
 Required = object()
 MAX_SAMPLE_SIZE = 16
 
 class NopTypeCaster(ATypeCaster):
-    cache = {}
+    cache: Dict[int,Union[PythonType, type]] = {}
     def to_canon(self, t):
         return t
 
 class Configuration(ABC):
     """Generic configuration template for dataclass. Mainly for type-checking.
 
     To modify dataclass behavior, inherit and extend this class,
@@ -51,56 +59,66 @@
             >>> Form("no", 12)
             Traceback (most recent call last):
                 ...
             TypeError: 12 is not in range(1, 11)
 
     """
 
+    field_types = (dataclasses.Field,)
+
     def on_default(self, default):
         """Called whenever a dataclass member is assigned a default value.
         """
         return default
 
     def make_type_caster(self, frame) -> ATypeCaster:
         """Return a type caster, as defined in pytypes.TypeCaster
         """
         return NopTypeCaster()
 
     @abstractmethod
     def ensure_isa(self, a, b, sampler=None):
         """Ensure that 'a' is an instance of type 'b'. If not, raise a TypeError.
         """
-        ...
 
     @abstractmethod
     def cast(self, obj, t):
         """Attempt to cast 'obj' to type 't'. If such a cast is not possible, raise a TypeError.
 
         The result is expected to pass `self.ensure_isa(res, t)` without an error,
         however this assertion is not validated, for performance reasons.
         """
-        ...
 
 
 class PythonConfiguration(Configuration):
     """Configuration to support Mypy-like and Pydantic-like features
 
     This is the default class given to the ``dataclass()`` function.
     """
-    make_type_caster = TypeCaster
+    
+    def make_type_caster(self, frame: Optional[types.FrameType]):
+        return TypeCaster(frame)
+
     ensure_isa = staticmethod(default_ensure_isa)
 
     def cast(self, obj, to_type):
         return to_type.cast_from(obj)
 
     def on_default(self, default):
         if isinstance(default, (list, dict, set)):
             def f(_=default):
                 return copy(_)
             return dataclasses.field(default_factory=f)
+        elif isinstance(default, self.field_types):
+            d = default.default
+            if isinstance(d, (list, dict, set)):
+                def f(_=d):
+                    return copy(_)
+                default.default = dataclasses.MISSING
+                default.default_factory = f
         return default
 
 
 def _get_field_type(type_caster, field):
     try:
         return type_caster.cache[id(field)]
     except KeyError:
@@ -179,29 +197,30 @@
         True
     """
     return dataclasses.replace(inst, **kwargs)
 
 
 def __iter__(inst):
     "Yields a list of tuples [(name, value), ...]"
+    # TODO: deprecate this method
     return ((name, getattr(inst, name)) for name in inst.__dataclass_fields__)
 
+def asdict(inst):
+    """Returns a dict of {name: value, ...}
+    """
+    return {name: getattr(inst, name) for name in inst.__dataclass_fields__}
 
 def aslist(inst):
-    """Returns a list of values
-
-    Equivalent to: ``list(dict(inst).values())``
+    """Returns a list of the values
     """
     return [getattr(inst, name) for name in inst.__dataclass_fields__]
 
 
 def astuple(inst):
-    """Returns a tuple of values
-
-    Equivalent to: ``tuple(dict(inst).values())``
+    """Returns a tuple of the values
     """
     return tuple(getattr(inst, name) for name in inst.__dataclass_fields__)
 
 
 def _json_rec(inst):
     if dataclasses.is_dataclass(inst):
         return json(inst)
@@ -227,38 +246,50 @@
 
 
 def _sample(seq, max_sample_size=MAX_SAMPLE_SIZE):
     if len(seq) <= max_sample_size:
         return seq
     return random.sample(seq, max_sample_size)
 
-def _process_class(cls, config, check_types, context_frame, **kw):
+def _process_class(cls: type, config: Configuration, check_types, context_frame, **kw):
+
     for name, type_ in getattr(cls, '__annotations__', {}).items():
         # type_ = config.type_to_canon(type_) if not isinstance(type_, str) else type_
 
         # If default not specified, assign Required, for a later check
         # We don't assign MISSING; we want to bypass dataclass which is too strict for this
         default = getattr(cls, name, Required)
         if default is Required:
             setattr(cls, name, Required)
         elif default is not dataclasses.MISSING:
-            if isinstance(default, dataclasses.Field):
+            if isinstance(default, config.field_types):
                 if default.default is dataclasses.MISSING and default.default_factory is dataclasses.MISSING:
                     default.default = Required
 
             new_default = config.on_default(default)
             if new_default is not default:
                 setattr(cls, name, new_default)
 
+
         cls.__annotations__[name] = type_
 
 
     c = copy(cls)
     orig_post_init = getattr(cls, '__post_init__', None)
 
+    init_f = getattr(c, '__init__', None)
+    if init_f:
+        try:
+            del c.__init__
+        except AttributeError:
+            pass
+        init_dispatcher = getattr(init_f, '__dispatcher__', None)
+    else:
+        init_dispatcher = None
+
     if check_types:
         sampler = _sample if check_types=='sample' else None
         type_caster = config.make_type_caster(context_frame)
         should_cast = check_types == 'cast'
 
         def __post_init__(self):
             # Only now context_frame has complete information
@@ -281,24 +312,34 @@
             if orig_post_init is not None:
                 orig_post_init(self)
 
         c.__post_init__ = __post_init__
 
     _set_if_not_exists(c, {
         'replace': replace,
+        'asdict': asdict,
         'aslist': aslist,
         'astuple': astuple,
         'json': json,
         '__iter__': __iter__,
     })
 
     slots = kw.pop('slots')
     c = dataclasses.dataclass(c, **kw)
     if slots:
         c = _add_slots(c, kw['frozen'])
+    
+    if init_dispatcher:
+        assert init_f
+        # __init__ may have been generated by the dataclass function
+        if hasattr(c, '__init__'):
+            # We will add it to the dispatch
+            c.__init__ = init_dispatcher(c.__init__)
+        else:
+            c.__init__ = init_f
     return c
 
 
 def _dataclass_getstate(self):
     return [getattr(self, f.name) for f in dataclasses.fields(self)]
 
 def _dataclass_setstate(self, state):
@@ -330,41 +371,59 @@
         # Need this for pickling frozen classes with slots.
         cls.__getstate__ = _dataclass_getstate
         cls.__setstate__ = _dataclass_setstate
 
     return cls
 
 
-# This is a super-ugly hack called PEP-0681. https://peps.python.org/pep-0681/
-_T = TypeVar("_T")
-def __dataclass_transform__(
-    *,
-    eq_default: bool = True,
-    order_default: bool = False,
-    kw_only_default: bool = False,
-    field_descriptors: Tuple[Union[type, Callable[..., Any]], ...] = (()),
-) -> Callable[[_T], _T]:
-    return lambda a: a
+_T = TypeVar('_T')
+python_config = PythonConfiguration()
 
+@dataclass_transform(field_specifiers=(dataclasses.field, dataclasses.Field), frozen_default=True)
+@overload
+def dataclass(
+    *,
+    check_types: Union[bool, str] = CHECK_TYPES,
+    config: Configuration = python_config,
+    init: bool = True,
+    repr: bool = True,
+    eq: bool = True,
+    order: bool = False,
+    unsafe_hash: bool = False,
+    frozen: bool = True,
+    slots: bool = ...,
+) -> Callable[[Type[_T]], Type[_T]]: ...
+
+@dataclass_transform(field_specifiers=(dataclasses.field, dataclasses.Field), frozen_default=True)
+@overload
+def dataclass(_cls: Type[_T]) -> Type[_T]: ...
+
+@dataclass_transform(field_specifiers=(dataclasses.field, dataclasses.Field), frozen_default=True)
+def dataclass(cls: Optional[Type[_T]]=None, *,
+              check_types: Union[bool, str] = CHECK_TYPES,
+              config: Configuration = python_config,
+                init: bool = True,
+                repr: bool = True,
+                eq: bool = True,
+                order: bool = False,
+                unsafe_hash: bool = False,
+                frozen: bool = True,
+                slots: bool = ...,
+    ) -> type:
 
-@__dataclass_transform__(eq_default=True, order_default=True)
-def dataclass(cls=None, *, check_types: Union[bool, str] = CHECK_TYPES,
-                           config: Configuration = PythonConfiguration(),
-                           init=True, repr=True, eq=True, order=False,
-                           unsafe_hash=False, frozen=True, slots=False) -> Any:
     """Runtype's dataclass is a drop-in replacement to Python's built-in dataclass, with added functionality.
 
     **Differences from builtin dataclass:**
 
     1. Type validation
       - Adds run-time type validation (when check_types is nonzero)
       - Performs automatic casting (when check_types == 'cast')
 
     2. Ergonomics
-      - Supports assigning mutable literals (i.e. list, set, and dict).
+      - Supports assigning mutable literals (i.e. list, set, and dict). Each instance gets a new copy.
       - Adds convenience methods: replace(), aslist(), astuple(), and iterator for dict(this).
         These methods won't override existing ones. They will be added only if the names aren't used.
       - Setting the default as ``None`` automatically makes the type into ``Optional``, if it isn't already.
       - Members without a default are allowed after members with a default
         (but they are required in order to create the instance)
 
     3. Misc
@@ -393,15 +452,18 @@
             {'x': 2, 'y': 3}
 
             >>> p.replace(x=30)  # New instance
             Point(x=30, y=3)
     """
     assert isinstance(config, Configuration)
 
-    context_frame = inspect.currentframe().f_back   # Get parent frame, to resolve forward-references
+    # Get parent frame, to resolve forward-references
+    _current_frame = inspect.currentframe()
+    context_frame = _current_frame and _current_frame.f_back
+
     def wrap(cls):
         return _process_class(cls, config, check_types, context_frame,
                               init=init, repr=repr, eq=eq, order=order,
                               unsafe_hash=unsafe_hash, frozen=frozen, slots=slots)
 
     # See if we're being called as @dataclass or @dataclass().
     if cls is None:
```

### Comparing `runtype-0.3.4/runtype/datetime_parse.py` & `runtype-0.3.5/runtype/datetime_parse.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,26 +61,21 @@
 
 EPOCH = datetime(1970, 1, 1)
 # if greater than this, the number is in ms, if less than or equal it's in seconds
 # (in seconds this is 11th October 2603, in ms it's 20th August 1970)
 MS_WATERSHED = int(2e10)
 # slightly more than datetime.max in ns - (datetime.max - EPOCH).total_seconds() * 1e9
 MAX_NUMBER = int(3e20)
-StrBytesIntFloat = Union[str, bytes, int, float]
 
 
-def get_numeric(value: StrBytesIntFloat, native_expected_type: str) -> Union[None, int, float]:
-    if isinstance(value, (int, float)):
-        return value
+def get_numeric(value: str, native_expected_type: str) -> Union[None, int, float]:
     try:
         return float(value)
     except ValueError:
         return None
-    except TypeError:
-        raise TypeError(f'invalid type; expected {native_expected_type}, string, bytes, int or float')
 
 
 def from_unix_seconds(seconds: Union[int, float]) -> datetime:
     if seconds > MAX_NUMBER:
         return datetime.max
     elif seconds < -MAX_NUMBER:
         return datetime.min
@@ -103,66 +98,51 @@
             return timezone(timedelta(minutes=offset))
         except ValueError:
             raise error()
     else:
         return None
 
 
-def parse_date(value: Union[date, StrBytesIntFloat]) -> date:
+def parse_date(value: str) -> date:
     """
     Parse a date/int/float/string and return a datetime.date.
 
     Raise ValueError if the input is well formatted but not a valid date.
     Raise ValueError if the input isn't well formatted.
     """
-    if isinstance(value, date):
-        if isinstance(value, datetime):
-            return value.date()
-        else:
-            return value
-
     number = get_numeric(value, 'date')
     if number is not None:
         return from_unix_seconds(number).date()
 
-    if isinstance(value, bytes):
-        value = value.decode()
-
     match = date_re.match(value)  # type: ignore
     if match is None:
         raise DateError()
 
     kw = {k: int(v) for k, v in match.groupdict().items()}
 
     try:
         return date(**kw)
     except ValueError:
         raise DateError()
 
 
-def parse_time(value: Union[time, StrBytesIntFloat]) -> time:
+def parse_time(value: str) -> time:
     """
     Parse a time/string and return a datetime.time.
 
     Raise ValueError if the input is well formatted but not a valid time.
     Raise ValueError if the input isn't well formatted, in particular if it contains an offset.
     """
-    if isinstance(value, time):
-        return value
-
     number = get_numeric(value, 'time')
     if number is not None:
         if number >= 86400:
             # doesn't make sense since the time time loop back around to 0
             raise TimeError()
         return (datetime.min + timedelta(seconds=number)).time()
 
-    if isinstance(value, bytes):
-        value = value.decode()
-
     match = time_re.match(value)  # type: ignore
     if match is None:
         raise TimeError()
 
     kw = match.groupdict()
     if kw['microsecond']:
         kw['microsecond'] = kw['microsecond'].ljust(6, '0')
@@ -173,34 +153,29 @@
 
     try:
         return time(**kw_)  # type: ignore
     except ValueError:
         raise TimeError()
 
 
-def parse_datetime(value: Union[datetime, StrBytesIntFloat]) -> datetime:
+def parse_datetime(value: str) -> datetime:
     """
     Parse a datetime/int/float/string and return a datetime.datetime.
 
     This function supports time zone offsets. When the input contains one,
     the output uses a timezone with a fixed offset from UTC.
 
     Raise ValueError if the input is well formatted but not a valid datetime.
     Raise ValueError if the input isn't well formatted.
     """
-    if isinstance(value, datetime):
-        return value
 
     number = get_numeric(value, 'datetime')
     if number is not None:
         return from_unix_seconds(number)
 
-    if isinstance(value, bytes):
-        value = value.decode()
-
     match = datetime_re.match(value)  # type: ignore
     if match is None:
         raise DateTimeError()
 
     kw = match.groupdict()
     if kw['microsecond']:
         kw['microsecond'] = kw['microsecond'].ljust(6, '0')
@@ -211,31 +186,22 @@
 
     try:
         return datetime(**kw_)  # type: ignore
     except ValueError:
         raise DateTimeError()
 
 
-def parse_duration(value: StrBytesIntFloat) -> timedelta:
+def parse_duration(value: str) -> timedelta:
     """
     Parse a duration int/float/string and return a datetime.timedelta.
 
     The preferred format for durations in Django is '%d %H:%M:%S.%f'.
 
     Also supports ISO 8601 representation.
     """
-    if isinstance(value, timedelta):
-        return value
-
-    if isinstance(value, (int, float)):
-        # below code requires a string
-        value = str(value)
-    elif isinstance(value, bytes):
-        value = value.decode()
-
     try:
         match = standard_duration_re.match(value) or iso8601_duration_re.match(value)
     except TypeError:
         raise TypeError('invalid type; expected timedelta, string, bytes, int or float')
 
     if not match:
         raise DurationError()
```

### Comparing `runtype-0.3.4/runtype/dispatch.py` & `runtype-0.3.5/runtype/dispatch.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .typesystem import TypeSystem
 
 
 class DispatchError(Exception):
     pass
 
 
+# TODO: Remove test_subtypes, replace with support for Type[], like isa(t, Type[t])
 class MultiDispatch:
     """Creates a dispatch group for multiple dispatch
 
     Parameters:
         typesystem - instance for interfacing with the typesystem
         test_subtypes: indices of params that should be matched by subclass instead of isinstance.
     """
@@ -34,14 +35,15 @@
         tree.define_function(f)
 
         @wraps(f)
         def dispatched_f(*args, **kw):
             f = tree.find_function_cached(args)
             return f(*args, **kw)
 
+        dispatched_f.__dispatcher__ = self
         return dispatched_f
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback): 
         pass
```

### Comparing `runtype-0.3.4/runtype/pytypes.py` & `runtype-0.3.5/runtype/pytypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from abc import abstractmethod, ABC
 from contextlib import suppress
 import collections
 from collections import abc
 import sys
 import typing
-from datetime import datetime
+from datetime import datetime, date, time, timedelta
+from types import FrameType
 
 from .utils import ForwardRef
 from .base_types import DataType, Validator, TypeMismatchError
 from . import base_types
 from . import datetime_parse
 
 
@@ -85,19 +86,19 @@
         if self.types and len(obj) != len(self.types):
             raise LengthMismatchError(self, obj)
         for type_, item in zip(self.types, obj):
             type_.validate_instance(item, sampler)
 
 
 class SumType(base_types.SumType, PythonType):
-    def __init__(self, types):
+    def __init__(self, types: typing.Sequence[PythonType]):
         # Here we merge all the instances of OneOf into a single one (if necessary).
         # The alternative is to turn all OneOf instances into SumTypes of single values.
         # I chose this method due to intuition that it's faster for the common use-case.
-        one_ofs: List[OneOf] = [t for t in types if isinstance(t, OneOf)]
+        one_ofs: typing.List[OneOf] = [t for t in types if isinstance(t, OneOf)]
         if len(one_ofs) > 1:
             rest = [t for t in types if not isinstance(t, OneOf)]
             types = rest + [OneOf([v for t in one_ofs for v in t.values])]
         super().__init__(types)
 
     def validate_instance(self, obj, sampler=None):
         if not any(t.test_instance(obj) for t in self.types):
@@ -107,20 +108,20 @@
         for t in self.types:
             with suppress(TypeError):
                return t.cast_from(obj)
 
         raise TypeMismatchError(obj, self)
 
 
-def _flatten_types(t):
-    if isinstance(t, SumType):
-        for t in t.types:
-            yield from _flatten_types(t)
-    else:
-        yield t
+# def _flatten_types(t):
+#     if isinstance(t, SumType):
+#         for t in t.types:
+#             yield from _flatten_types(t)
+#     else:
+#         yield t
 
 
 
 class PythonDataType(DataType, PythonType):
     def __init__(self, kernel, supertypes={Any}):
         self.kernel = kernel
 
@@ -266,20 +267,24 @@
                 vt.validate_instance(v, sampler)
 
     def __getitem__(self, item):
         assert self.item == Any*Any
         return type(self)(self.base, item)
 
     def cast_from(self, obj):
-        # Must already be a dict
-        self.base.validate_instance(obj)
-
         # Optimize for Dict[Any] and empty dicts
         if self.item is Any or not obj:
-            return obj
+            # Already a dict?
+            if self.base.test_instance(obj):
+                return obj
+            # Make sure it's a dict
+            return dict(obj)
+
+        # Must already be a dict
+        self.base.validate_instance(obj)
 
         # Recursively cast each item
         kt, vt = self.item.types
         return {kt.cast_from(k): vt.cast_from(v) for k, v in obj.items()}
 
 
 Object = PythonDataType(object)
@@ -342,14 +347,41 @@
         if isinstance(obj, str):
             try:
                 return datetime_parse.parse_datetime(obj)
             except datetime_parse.DateTimeError:
                 raise TypeMismatchError(obj, self)
         return super().cast_from(obj)
 
+class _Date(PythonDataType):
+    def cast_from(self, obj):
+        if isinstance(obj, str):
+            try:
+                return datetime_parse.parse_date(obj)
+            except datetime_parse.DateTimeError:
+                raise TypeMismatchError(obj, self)
+        return super().cast_from(obj)
+
+class _Time(PythonDataType):
+    def cast_from(self, obj):
+        if isinstance(obj, str):
+            try:
+                return datetime_parse.parse_time(obj)
+            except datetime_parse.DateTimeError:
+                raise TypeMismatchError(obj, self)
+        return super().cast_from(obj)
+
+class _TimeDelta(PythonDataType):
+    def cast_from(self, obj):
+        if isinstance(obj, str):
+            try:
+                return datetime_parse.parse_duration(obj)
+            except datetime_parse.DateTimeError:
+                raise TypeMismatchError(obj, self)
+        return super().cast_from(obj)
+
 
 class _NoneType(OneOf):
     def __init__(self):
         super().__init__([None])
 
     def cast_from(self, obj):
         assert self.values == [None]
@@ -359,14 +391,17 @@
 
 
 String = _String(str)
 Int = _Int(int)
 Float = _Float(float)
 NoneType =  _NoneType()
 DateTime = _DateTime(datetime)
+Date = _Date(date)
+Time = _Time(time)
+TimeDelta = _TimeDelta(timedelta)
 
 
 _type_cast_mapping = {
     iter: Iter,
     list: List,
     set: Set,
     frozenset: FrozenSet,
@@ -376,15 +411,17 @@
     str: String,
     float: Float,
     bytes: Bytes,
     type(None): NoneType,
     object: Any,
     typing.Any: Any,
     datetime: DateTime,
-
+    date: Date,
+    time: Time,
+    timedelta: TimeDelta,
 }
 
 
 if sys.version_info >= (3, 7):
     origin_list = list
     origin_dict = dict
     origin_tuple = tuple
@@ -401,16 +438,16 @@
 
 class ATypeCaster(ABC):
     @abstractmethod
     def to_canon(self, t: typing.Any): ...
 
 
 class TypeCaster(ATypeCaster):
-    def __init__(self, frame=None):
-        self.cache = {}
+    def __init__(self, frame: typing.Optional[FrameType]=None):
+        self.cache: typing.Dict[typing.Union[type, PythonType], PythonType] = {}
         self.frame = frame
 
     def _to_canon(self, t):
         to_canon = self.to_canon
 
         if isinstance(t, (base_types.Type, Validator)):
             return t
```

### Comparing `runtype-0.3.4/runtype/typesystem.py` & `runtype-0.3.5/runtype/typesystem.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.4/runtype/utils.py` & `runtype-0.3.5/runtype/utils.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.4/runtype/validation.py` & `runtype-0.3.5/runtype/validation.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.4/setup.py` & `runtype-0.3.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.7"': ['dataclasses',
                                                          'contextvars']}
 
 setup_kwargs = {
     'name': 'runtype',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'Type dispatch and validation for run-time Python',
-    'long_description': '![alt text](logo.png "Logo")\n\n\nRuntype is a collection of run-time type utilities for Python.\n\nIt is:\n\n:runner: Fast! Uses an internal typesystem for maximum performance.\n\n:brain: Smart! Supports `typing`, forward-references, constraints, auto-casting, and more.\n\n:gear: Configurative! Write your own type system, and use it with *dataclass* and *dispatch*.\n\n------\n\n### Modules\n\n- :star: [**validation**](https://runtype.readthedocs.io/en/latest/validation.html) - Provides a smarter alternative to `isinstance` and `issubclass`, with support for the `typing` module, and type constraints.\n\n- :star: [**dataclass**](https://runtype.readthedocs.io/en/latest/dataclass.html) - Adds run-time type validation to the built-in dataclass.\n\n    - Improves dataclass ergonomics.\n    - Supports most mypy constructs, like `typing` and forward-references (`foo: \'Bar\'`).\n    - Supports automatic value casting, Pydantic-style. (Optional, off by default)\n    - Supports types with constraints. (e.g. `String(max_length=10)`)\n    - Supports optional sampling for faster validation of big lists and dicts.\n    - Twice faster than Pydantic ([read here](https://runtype.readthedocs.io/en/latest/dataclass.html#compared-to-pydantic))\n\n- :star: [**dispatch**](https://runtype.readthedocs.io/en/latest/dispatch.html) - Provides fast multiple-dispatch for functions and methods, via a decorator.\n\n    - Inspired by Julia.\n\n- :star: [**type utilities**](https://runtype.readthedocs.io/en/latest/types.html) - Provides a set of classes to implement your own type-system.\n\n    - Used by runtype itself, to emulate the Python type-system.\n\n\n## Docs\n\nRead the docs here: https://runtype.readthedocs.io/\n\n## Install\n\n```bash\npip install runtype\n```\n\nNo dependencies.\n\nRequires Python 3.6 or up.\n\n[![Build Status](https://travis-ci.org/erezsh/runtype.svg?branch=master)](https://travis-ci.org/erezsh/runtype)\n[![codecov](https://codecov.io/gh/erezsh/runtype/branch/master/graph/badge.svg)](https://codecov.io/gh/erezsh/runtype)\n\n## Examples\n\n### Validation (Isa & Subclass)\n\n```python\nfrom typing import Dict, Mapping\nfrom runtype import isa, issubclass\n\nprint( isa({\'a\': 1}, Dict[str, int]) )\n#> True\nprint( isa({\'a\': \'b\'}, Dict[str, int]) )\n#> False\n\nprint( issubclass(Dict[str, int], Mapping[str, int]) )\n#> True\nprint( issubclass(Dict[str, int], Mapping[int, str]) )\n#> False\n```\n\n### Dataclasses\n\n```python\nfrom typing import List\nfrom datetime import datetime\nfrom runtype import dataclass\n\n@dataclass(check_types=\'cast\')  # Cast values to the target type, when applicable\nclass Person:\n    name: str\n    birthday: datetime = None   # Optional\n    interests: List[str] = []   # The list is copied for each instance\n\n\nprint( Person("Beetlejuice") )\n#> Person(name=\'Beetlejuice\', birthday=None, interests=[])\nprint( Person("Albert", "1955-04-18T00:00", [\'physics\']) )\n#> Person(name=\'Albert\', birthday=datetime.datetime(1955, 4, 18, 0, 0), interests=[\'physics\'])\nprint( Person("Bad", interests=[\'a\', 1]) )\n# Traceback (most recent call last):\n#   ...\n# TypeError: [Person] Attribute \'interests\' expected value of type list[str]. Instead got [\'a\', 1]\n\n#     Failed on item: 1, expected type str\n\n```\n\n### Multiple Dispatch\n\n```python\nfrom runtype import Dispatch\ndp = Dispatch()\n\n@dp\ndef append(a: list, b):\n    return a + [b]\n\n@dp\ndef append(a: tuple, b):\n    return a + (b,)\n\n@dp\ndef append(a: str, b: str):\n    return a + b\n\n\nprint( append([1, 2, 3], 4) )\n#> [1, 2, 3, 4]\nprint( append((1, 2, 3), 4) )\n#> (1, 2, 3, 4)\nprint( append(\'foo\', \'bar\') )\n#> foobar\nprint( append(\'foo\', 4)     )\n# Traceback (most recent call last):\n#    ...\n# runtype.dispatch.DispatchError: Function \'append\' not found for signature (<class \'str\'>, <class \'int\'>)\n```\n\n\n## License\n\nRuntype uses the [MIT license](LICENSE).\n\n## Donate\n\nIf you like Runtype and want to show your appreciation, you can do so at my [patreon page](https://www.patreon.com/erezsh), or [ko-fi page](https://ko-fi.com/erezsh).\n',
+    'long_description': '![alt text](logo.png "Logo")\n\n\nRuntype is a collection of run-time type utilities for Python.\n\nIt is:\n\n:runner: Fast! Uses an internal typesystem for maximum performance.\n\n:brain: Smart! Supports `typing`, forward-references, constraints, auto-casting, and more.\n\n:gear: Configurative! Write your own type system, and use it with *dataclass* and *dispatch*.\n\n------\n\n### Modules\n\n- :star: [**validation**](https://runtype.readthedocs.io/en/latest/validation.html) - Provides a smarter alternative to `isinstance` and `issubclass`, with support for the `typing` module, and type constraints.\n\n- :star: [**dataclass**](https://runtype.readthedocs.io/en/latest/dataclass.html) - Adds run-time type validation to the built-in dataclass.\n\n    - Improves dataclass ergonomics.\n    - Supports most mypy constructs, like `typing` and forward-references (`foo: \'Bar\'`).\n    - Supports automatic value casting, Pydantic-style. (Optional, off by default)\n    - Supports types with constraints. (e.g. `String(max_length=10)`)\n    - Supports optional sampling for faster validation of big lists and dicts.\n    - Twice faster than Pydantic ([read here](https://runtype.readthedocs.io/en/latest/dataclass.html#compared-to-pydantic))\n\n- :star: [**dispatch**](https://runtype.readthedocs.io/en/latest/dispatch.html) - Provides fast multiple-dispatch for functions and methods, via a decorator.\n\n    - Inspired by Julia.\n\n- :star: [**type utilities**](https://runtype.readthedocs.io/en/latest/types.html) - Provides a set of classes to implement your own type-system.\n\n    - Used by runtype itself, to emulate the Python type-system.\n\n\n## Docs\n\nRead the docs here: https://runtype.readthedocs.io/\n\n## Install\n\n```bash\npip install runtype\n```\n\nNo dependencies.\n\nRequires Python 3.6 or up.\n\n[![codecov](https://codecov.io/gh/erezsh/runtype/branch/master/graph/badge.svg)](https://codecov.io/gh/erezsh/runtype)\n\n## Examples\n\n### Validation (Isa & Subclass)\n\n```python\nfrom typing import Dict, Mapping\nfrom runtype import isa, issubclass\n\nprint( isa({\'a\': 1}, Dict[str, int]) )\n#> True\nprint( isa({\'a\': \'b\'}, Dict[str, int]) )\n#> False\n\nprint( issubclass(Dict[str, int], Mapping[str, int]) )\n#> True\nprint( issubclass(Dict[str, int], Mapping[int, str]) )\n#> False\n```\n\n### Dataclasses\n\n```python\nfrom typing import List\nfrom datetime import datetime\nfrom runtype import dataclass\n\n@dataclass(check_types=\'cast\')  # Cast values to the target type, when applicable\nclass Person:\n    name: str\n    birthday: datetime = None   # Optional\n    interests: List[str] = []   # The list is copied for each instance\n\n\nprint( Person("Beetlejuice") )\n#> Person(name=\'Beetlejuice\', birthday=None, interests=[])\nprint( Person("Albert", "1955-04-18T00:00", [\'physics\']) )\n#> Person(name=\'Albert\', birthday=datetime.datetime(1955, 4, 18, 0, 0), interests=[\'physics\'])\nprint( Person("Bad", interests=[\'a\', 1]) )\n# Traceback (most recent call last):\n#   ...\n# TypeError: [Person] Attribute \'interests\' expected value of type list[str]. Instead got [\'a\', 1]\n\n#     Failed on item: 1, expected type str\n\n```\n\n### Multiple Dispatch\n\n```python\nfrom runtype import Dispatch\ndp = Dispatch()\n\n@dp\ndef append(a: list, b):\n    return a + [b]\n\n@dp\ndef append(a: tuple, b):\n    return a + (b,)\n\n@dp\ndef append(a: str, b: str):\n    return a + b\n\n\nprint( append([1, 2, 3], 4) )\n#> [1, 2, 3, 4]\nprint( append((1, 2, 3), 4) )\n#> (1, 2, 3, 4)\nprint( append(\'foo\', \'bar\') )\n#> foobar\nprint( append(\'foo\', 4)     )\n# Traceback (most recent call last):\n#    ...\n# runtype.dispatch.DispatchError: Function \'append\' not found for signature (<class \'str\'>, <class \'int\'>)\n```\n\nDispatch can also be used for extending the dataclass builtin `__init__`:\n\n```python\ndp = Dispatch()\n\n@dataclass(frozen=False)\nclass Point:\n    x: int = 0\n    y: int = 0\n    \n    @dp\n    def __init__(self, points: list | tuple):\n        self.x, self.y = points\n\n    @dp\n    def __init__(self, points: dict):\n        self.x = points[\'x\']\n        self.y = points[\'y\']\n    \n# Test constructors\np0 = Point()                         # Default constructor\nassert p0 == Point(0, 0)             # Default constructor\nassert p0 == Point([0, 0])           # User constructor\nassert p0 == Point((0, 0))           # User constructor\nassert p0 == Point({"x": 0, "y": 0}) # User constructor\n```\n\n\n## License\n\nRuntype uses the [MIT license](LICENSE).\n\n## Donate\n\nIf you like Runtype and want to show your appreciation, you can do so at my [patreon page](https://www.patreon.com/erezsh), or [ko-fi page](https://ko-fi.com/erezsh).\n',
     'author': 'Erez Shinan',
     'author_email': 'erezshin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/erezsh/runtype',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `runtype-0.3.4/PKG-INFO` & `runtype-0.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtype
-Version: 0.3.4
+Version: 0.3.5
 Summary: Type dispatch and validation for run-time Python
 Home-page: https://github.com/erezsh/runtype
 License: MIT
 Keywords: types,typing,dispatch,multimethods,dataclass,runtime
 Author: Erez Shinan
 Author-email: erezshin@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -73,15 +73,14 @@
 pip install runtype
 ```
 
 No dependencies.
 
 Requires Python 3.6 or up.
 
-[![Build Status](https://travis-ci.org/erezsh/runtype.svg?branch=master)](https://travis-ci.org/erezsh/runtype)
 [![codecov](https://codecov.io/gh/erezsh/runtype/branch/master/graph/badge.svg)](https://codecov.io/gh/erezsh/runtype)
 
 ## Examples
 
 ### Validation (Isa & Subclass)
 
 ```python
@@ -153,14 +152,41 @@
 #> foobar
 print( append('foo', 4)     )
 # Traceback (most recent call last):
 #    ...
 # runtype.dispatch.DispatchError: Function 'append' not found for signature (<class 'str'>, <class 'int'>)
 ```
 
+Dispatch can also be used for extending the dataclass builtin `__init__`:
+
+```python
+dp = Dispatch()
+
+@dataclass(frozen=False)
+class Point:
+    x: int = 0
+    y: int = 0
+    
+    @dp
+    def __init__(self, points: list | tuple):
+        self.x, self.y = points
+
+    @dp
+    def __init__(self, points: dict):
+        self.x = points['x']
+        self.y = points['y']
+    
+# Test constructors
+p0 = Point()                         # Default constructor
+assert p0 == Point(0, 0)             # Default constructor
+assert p0 == Point([0, 0])           # User constructor
+assert p0 == Point((0, 0))           # User constructor
+assert p0 == Point({"x": 0, "y": 0}) # User constructor
+```
+
 
 ## License
 
 Runtype uses the [MIT license](LICENSE).
 
 ## Donate
```

