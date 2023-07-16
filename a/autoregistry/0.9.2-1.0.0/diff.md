# Comparing `tmp/autoregistry-0.9.2.tar.gz` & `tmp/autoregistry-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoregistry-0.9.2.tar", max compression
+gzip compressed data, was "autoregistry-1.0.0.tar", max compression
```

## Comparing `autoregistry-0.9.2.tar` & `autoregistry-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-02-25 01:09:51.783225 autoregistry-0.9.2/LICENSE
--rw-r--r--   0        0        0     4730 2023-02-25 01:09:51.783225 autoregistry-0.9.2/README.rst
--rw-r--r--   0        0        0      534 2023-02-25 01:10:12.106982 autoregistry-0.9.2/autoregistry/__init__.py
--rw-r--r--   0        0        0     2537 2023-02-25 01:09:51.783225 autoregistry-0.9.2/autoregistry/config.py
--rw-r--r--   0        0        0      592 2023-02-25 01:09:51.783225 autoregistry-0.9.2/autoregistry/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-25 01:09:51.783225 autoregistry-0.9.2/autoregistry/py.typed
--rw-r--r--   0        0        0      693 2023-02-25 01:09:51.783225 autoregistry-0.9.2/autoregistry/regex.py
--rw-r--r--   0        0        0    12273 2023-02-25 01:09:51.783225 autoregistry-0.9.2/autoregistry/registry.py
--rw-r--r--   0        0        0     1685 2023-02-25 01:10:12.102982 autoregistry-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 autoregistry-0.9.2/setup.py
--rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 autoregistry-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-16 23:56:08.039638 autoregistry-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4729 2023-07-16 23:56:08.039638 autoregistry-1.0.0/README.rst
+-rw-r--r--   0        0        0      575 2023-07-16 23:56:36.555737 autoregistry-1.0.0/autoregistry/__init__.py
+-rw-r--r--   0        0        0    11976 2023-07-16 23:56:08.039638 autoregistry-1.0.0/autoregistry/_registry.py
+-rw-r--r--   0        0        0     2908 2023-07-16 23:56:08.039638 autoregistry-1.0.0/autoregistry/config.py
+-rw-r--r--   0        0        0      712 2023-07-16 23:56:08.039638 autoregistry-1.0.0/autoregistry/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-16 23:56:08.039638 autoregistry-1.0.0/autoregistry/py.typed
+-rw-r--r--   0        0        0      842 2023-07-16 23:56:08.039638 autoregistry-1.0.0/autoregistry/regex.py
+-rw-r--r--   0        0        0     3348 2023-07-16 23:56:36.551737 autoregistry-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5398 1970-01-01 00:00:00.000000 autoregistry-1.0.0/PKG-INFO
```

### Comparing `autoregistry-0.9.2/LICENSE` & `autoregistry-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoregistry-0.9.2/README.rst` & `autoregistry-1.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 With AutoRegistry, the lookup is automatically created for you.
 
 
 AutoRegistry has a single  powerful class ``Registry`` that can do the following:
 
 * Be inherited to automatically register subclasses by their name.
 
-* Be directly invoked ``my_registery = Registry()`` to create a decorator
+* Be directly invoked ``my_registry = Registry()`` to create a decorator
   for registering callables like functions.
 
 * Traverse and automatically create registries for other python libraries.
 
 .. inclusion-marker-remove
 
 AutoRegistry is also highly configurable, with features like name-schema-enforcement and name-conversion-rules.
```

### Comparing `autoregistry-0.9.2/autoregistry/__init__.py` & `autoregistry-1.0.0/autoregistry/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Don't manually change, let poetry-dynamic-versioning-plugin handle it.
-__version__ = "0.9.2"
+__version__ = "1.0.0"
 
 __all__ = [
     "CannotDeriveNameError",
     "CannotRegisterPythonBuiltInError",
     "InvalidNameError",
     "KeyCollisionError",
     "ModuleAliasError",
     "Registry",
     "RegistryError",
     "RegistryMeta",
+    "InternalError",
 ]
 
+from ._registry import Registry, RegistryMeta
 from .exceptions import (
     CannotDeriveNameError,
     CannotRegisterPythonBuiltInError,
+    InternalError,
     InvalidNameError,
     KeyCollisionError,
     ModuleAliasError,
     RegistryError,
 )
-from .registry import Registry, RegistryMeta
```

### Comparing `autoregistry-0.9.2/autoregistry/config.py` & `autoregistry-1.0.0/autoregistry/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dataclasses
 import re
 from dataclasses import asdict, dataclass
+from typing import Callable, Optional
 
 from .exceptions import InvalidNameError
-from .regex import key_split, to_snake_case
+from .regex import hyphenate, key_split, to_snake_case
 
 
 @dataclass
 class RegistryConfig:
     case_sensitive: bool = False
     prefix: str = ""
     suffix: str = ""
@@ -20,16 +21,24 @@
     # Classes only; Register to its own registry
     register_self: bool = False
 
     # If ``True``, register new entries in all parent registries.
     # Otherwise, only register in parent.
     recursive: bool = True
 
+    # Convert PascalCase names to snake_case.
     snake_case: bool = False
 
+    # Convert underscores _ to hyphens -
+    hyphen: bool = False
+
+    # Custom user-provided name transform.
+    transform: Optional[Callable[[str], str]] = None
+
+    # Allow registry keys to be overwritten.
     overwrite: bool = False
 
     # Redirect vanilla methods that would collide with the dict-like interface.
     redirect: bool = True
 
     def __post_init__(self):
         if self.regex:
@@ -55,21 +64,20 @@
             if not self.case_sensitive:
                 key = key.lower()
 
             registry = registry[key]
         return registry
 
     def format(self, name: str) -> str:
-        """Convert and validate a PascalCase class name to a registry key.
+        """Convert and validate a function or class name to a registry key.
 
         Parameters
         ----------
         name: str
-            Name to convert to a registry key. For example, converts ``FooBar``
-            into ``foobar``.
+            Name to convert to a registry key.
         """
         if self._regex_validator and not self._regex_validator.match(name):
             raise InvalidNameError(f"{name} name must match regex {self.regex}")
 
         if not name.startswith(self.prefix):
             raise InvalidNameError(f'"{name}" name must start with "{self.prefix}"')
 
@@ -81,11 +89,17 @@
 
         if self.strip_suffix and self.suffix:
             name = name[: -len(self.suffix)]
 
         if self.snake_case:
             name = to_snake_case(name)
 
+        if self.hyphen:
+            name = hyphenate(name)
+
+        if self.transform:
+            name = self.transform(name)
+
         if not self.case_sensitive:
             name = name.lower()
 
         return name
```

### Comparing `autoregistry-0.9.2/autoregistry/exceptions.py` & `autoregistry-1.0.0/autoregistry/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,7 +16,11 @@
 
 class ModuleAliasError(RegistryError):
     """Cannot assign aliases when recursively traversing a module."""
 
 
 class CannotRegisterPythonBuiltInError(RegistryError):
     """AutoRegistry doesn't work with python built-ins."""
+
+
+class InternalError(RegistryError):
+    """Something went wrong internal to AutoRegistry that should never happen."""
```

### Comparing `autoregistry-0.9.2/autoregistry/regex.py` & `autoregistry-1.0.0/autoregistry/regex.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""String manipulation functions.
+"""
 import re
 from typing import List
 
 _to_snake_case_pattern1 = re.compile("(.)([A-Z][a-z]+)")
 _to_snake_case_pattern2 = re.compile("__([A-Z])")
 _to_snake_case_pattern3 = re.compile("([a-z0-9])([A-Z])")
 
@@ -22,9 +24,14 @@
     """
     name = _to_snake_case_pattern1.sub(r"\1_\2", name)
     name = _to_snake_case_pattern2.sub(r"_\1", name)
     name = _to_snake_case_pattern3.sub(r"\1_\2", name)
     return name.lower()
 
 
+def hyphenate(name: str) -> str:
+    """Convert underscores to hyphens."""
+    return name.replace("_", "-")
+
+
 def key_split(s: str) -> List[str]:
     return s.replace("/", ".").split(".")
```

### Comparing `autoregistry-0.9.2/autoregistry/registry.py` & `autoregistry-1.0.0/autoregistry/_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from types import MethodType
 from typing import Any, Callable, Generator, Iterable, Type, Union
 
 from .config import RegistryConfig
 from .exceptions import (
     CannotDeriveNameError,
     CannotRegisterPythonBuiltInError,
+    InternalError,
     InvalidNameError,
     KeyCollisionError,
     ModuleAliasError,
 )
 
 
 class _Registry(dict):
@@ -50,18 +51,18 @@
             Set to ``True`` when calling initial ``__register__``.
             Force register to immediate parent(s).
         """
         # Derive/Validate Name
         if not name:
             try:
                 name = str(obj.__name__)
-            except AttributeError:
+            except AttributeError as e:
                 raise CannotDeriveNameError(
                     f"Cannot derive name from a bare {type(obj)}."
-                )
+                ) from e
             name = self.config.format(name)
         elif "." in name or "/" in name:
             raise InvalidNameError(f'Name "{name}" cannot contain "." or "/".')
 
         if not self.config.overwrite and name in self:
             raise KeyCollisionError(f'"{name}" already registered to {self}')
 
@@ -116,16 +117,15 @@
 
     __registry__: _Registry
 
     def __getitem__(self, key: str) -> Type:
         return self.__registry__.config.getitem(self.__registry__, key)
 
     def __iter__(self) -> Generator[str, None, None]:
-        for val in self.__registry__:
-            yield val
+        yield from self.__registry__
 
     def __len__(self) -> int:
         return len(self.__registry__)
 
     def __contains__(self, key: str) -> bool:
         try:
             self.__registry__.config.getitem(self.__registry__, key)
@@ -136,16 +136,15 @@
     def keys(self) -> KeysView:
         return self.__registry__.keys()
 
     def values(self) -> ValuesView:
         return self.__registry__.values()
 
     def items(self):
-        for item in self.__registry__.items():
-            yield item
+        yield from self.__registry__.items()
 
     def get(self, key: Union[str, Type], default=None) -> Type:
         try:
             return self[key]
         except KeyError:
             pass
         if isinstance(default, str):
@@ -153,15 +152,15 @@
         else:
             return default
 
     def clear(self):
         self.__registry__.clear()
 
 
-class MethodDescriptor(object):
+class MethodDescriptor:
     """
     Non-data-descriptor that dispatches depending if it was called from a Class or an instance.
     """
 
     def __init__(self, user_method, registry_method):
         self.user_method = user_method
         self.registry_method = registry_method
@@ -199,39 +198,31 @@
             Additionally, register this class under these string(s).
         skip : bool
             Do **not** register this class to the appropriate registry(s).
         """
         # Manipulate namespace instead of modifying attributes after calling __new__ so
         # that hooks like __init_subclass__ have appropriately set registry attributes.
         # Each subclass gets its own registry.
-        try:
-            Registry  # pyright: ignore[reportUnusedExpression]
-        except NameError:
-            # Should only happen the very first time that
-            # Registry is being defined.
-            namespace["__registry__"] = _Registry(RegistryConfig(**config))
-            new_cls = super().__new__(cls, cls_name, bases, namespace)
-            return new_cls
 
         # Copy the nearest parent config, then update it with new params
         for parent_cls in bases:
             try:
                 registry_config = parent_cls.__registry__.config.copy()
                 break
             except AttributeError:
                 pass
         else:
-            raise Exception("Should never happen.")  # pragma: no cover
+            # No parent config, create a new one from scratch.
+            namespace["__registry__"] = _Registry(RegistryConfig(**config))
+            new_cls = super().__new__(cls, cls_name, bases, namespace)
+            return new_cls
 
         # Derive registry name before updating registry config, since a classes own name is
         # subject to it's parents configuration, not its own.
-        if name is None:
-            registry_name = registry_config.format(cls_name)
-        else:
-            registry_name = name
+        registry_name = registry_config.format(cls_name) if name is None else name
 
         registry_config.update(config)
 
         namespace["__registry__"] = _Registry(registry_config, name=registry_name)
 
         if namespace["__registry__"].config.redirect:
             for method_name in [
@@ -266,17 +257,17 @@
             name=new_cls.__registry__.name,
             aliases=aliases,
             root=True,  # Always register to direct parents
         )
 
         return new_cls
 
-    def __repr__(self):
+    def __repr__(cls):
         try:
-            return f"<{self.__name__}: {list(self.__registry__.keys())}>"
+            return f"<{cls.__name__}: {list(cls.__registry__.keys())}>"
         except Exception:
             return super().__repr__()
 
 
 class Registry(metaclass=RegistryMeta):
     __call__: Callable
     __contains__: Callable[..., bool]
@@ -335,32 +326,35 @@
             return obj
 
         if aliases:
             raise ModuleAliasError
 
         try:
             obj_file = obj.__file__
-            assert obj_file is not None
-        except (AttributeError, AssertionError):
+        except AttributeError:
+            obj_file = None
+        if obj_file is None:
             raise CannotRegisterPythonBuiltInError(
                 f"Cannot register Python BuiltIn {obj}"
             )
+
         obj_folder = str(Path(obj_file).parent)
         # Skip private and magic attributes
         elem_names = [x for x in dir(obj) if not x.startswith("_")]
         for elem_name in elem_names:
             handle = getattr(obj, elem_name)
             if ismodule(handle):
                 if not config.recursive:
                     continue
                 try:
                     handle_file = handle.__file__
-                    assert handle_file is not None
-                except (AttributeError, AssertionError):
-                    # handle is a python built-in
+                except AttributeError:
+                    handle_file = None
+
+                if handle_file is None:  # handle is a python built-in
                     continue
 
                 handle_folder = str(Path(handle_file).parent)
                 if not handle_folder.startswith(obj_folder):
                     # Only traverse direct submodules
                     continue
```

### Comparing `autoregistry-0.9.2/setup.py` & `autoregistry-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,199 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: autoregistry
+Version: 1.0.0
+Summary: Automatic registry design-pattern for mapping names to functionality.
+Home-page: https://github.com/BrianPugh/autoregistry
+License: Apache-2.0
+Author: Brian Pugh
+Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/BrianPugh/autoregistry
+Description-Content-Type: text/x-rst
 
-packages = \
-['autoregistry']
+.. image:: https://raw.githubusercontent.com/BrianPugh/autoregistry/main/assets/logo_400w.png
 
-package_data = \
-{'': ['*']}
+|Python compat| |PyPi| |GHA tests| |Codecov report| |readthedocs|
 
-setup_kwargs = {
-    'name': 'autoregistry',
-    'version': '0.9.2',
-    'description': 'Automatic registry design-pattern for mapping names to functionality.',
-    'long_description': '.. image:: https://raw.githubusercontent.com/BrianPugh/autoregistry/main/assets/logo_400w.png\n\n|Python compat| |PyPi| |GHA tests| |Codecov report| |readthedocs|\n\n.. inclusion-marker-do-not-remove\n\nAutoRegistry\n============\n\nInvoking functions and class-constructors from a string is a common design pattern\nthat AutoRegistry aims to solve.\nFor example, a user might specify a backend of type ``"sqlite"`` in a yaml configuration\nfile, for which our program needs to construct the ``SQLite`` subclass of our ``Database`` class.\nClassically, you would need to manually create a lookup, mapping the string ``"sqlite"`` to\nthe ``SQLite`` constructor.\nWith AutoRegistry, the lookup is automatically created for you.\n\n\nAutoRegistry has a single  powerful class ``Registry`` that can do the following:\n\n* Be inherited to automatically register subclasses by their name.\n\n* Be directly invoked ``my_registery = Registry()`` to create a decorator\n  for registering callables like functions.\n\n* Traverse and automatically create registries for other python libraries.\n\n.. inclusion-marker-remove\n\nAutoRegistry is also highly configurable, with features like name-schema-enforcement and name-conversion-rules.\n`Checkout the docs for more information <https://autoregistry.readthedocs.io/en/latest/?badge=latest/>`_.\n\n`Watch AutoRegistry in action! <https://youtu.be/4No_NE7bUOM>`_\n\nInstallation\n============\nAutoRegistry requires Python ``>=3.8``.\n\n.. code-block:: bash\n\n   python -m pip install autoregistry\n\n\nExamples\n========\n\nClass Inheritance\n^^^^^^^^^^^^^^^^^\n\n``Registry`` adds a dictionary-like interface to class constructors\nfor looking up subclasses.\n\n.. code-block:: python\n\n   from abc import abstractmethod\n   from dataclasses import dataclass\n   from autoregistry import Registry\n\n\n   @dataclass\n   class Pokemon(Registry):\n       level: int\n       hp: int\n\n       @abstractmethod\n       def attack(self, target):\n           """Attack another Pokemon."""\n\n\n   class Charmander(Pokemon):\n       def attack(self, target):\n           return 1\n\n\n   class Pikachu(Pokemon):\n       def attack(self, target):\n           return 2\n\n\n   class SurfingPikachu(Pikachu):\n       def attack(self, target):\n           return 3\n\n\n   print(f"{len(Pokemon)} Pokemon types registered:")\n   print(f"    {list(Pokemon)}")\n   # By default, lookup is case-insensitive\n   charmander = Pokemon["cHaRmAnDer"](level=7, hp=31)\n   print(f"Created Pokemon: {charmander}")\n\nThis code block produces the following output:\n\n.. code-block::\n\n   3 Pokemon types registered:\n       [\'charmander\', \'pikachu\', \'surfingpikachu\']\n   Created Pokemon: Charmander(level=7, hp=31)\n\n\nFunction Registry\n^^^^^^^^^^^^^^^^^\n\nDirectly instantiating a ``Registry`` object allows you to\nregister functions by decorating them.\n\n.. code-block:: python\n\n   from autoregistry import Registry\n\n   pokeballs = Registry()\n\n\n   @pokeballs\n   def masterball(target):\n       return 1.0\n\n\n   @pokeballs\n   def pokeball(target):\n       return 0.1\n\n\n   for ball in ["pokeball", "masterball"]:\n       success_rate = pokeballs[ball](None)\n       print(f"Ash used {ball} and had {success_rate=}")\n\nThis code block produces the following output:\n\n.. code-block:: text\n\n   Ash used pokeball and had success_rate=0.1\n   Ash used masterball and had success_rate=1.0\n\n\nModule Registry\n^^^^^^^^^^^^^^^\n\nCreate a registry for another python module.\n\n.. code-block:: python\n\n   import torch\n   from autoregistry import Registry\n\n   optims = Registry(torch.optim)\n\n   # "adamw" and ``lr`` could be coming from a configuration file.\n   optimizer = optims["adamw"](model.parameters(), lr=3e-3)\n\n   assert list(optims) == [\n       "asgd",\n       "adadelta",\n       "adagrad",\n       "adam",\n       "adamw",\n       "adamax",\n       "lbfgs",\n       "nadam",\n       "optimizer",\n       "radam",\n       "rmsprop",\n       "rprop",\n       "sgd",\n       "sparseadam",\n       "lr_scheduler",\n       "swa_utils",\n   ]\n\n\n.. |GHA tests| image:: https://github.com/BrianPugh/autoregistry/workflows/tests/badge.svg\n   :target: https://github.com/BrianPugh/autoregistry/actions?query=workflow%3Atests\n   :alt: GHA Status\n.. |Codecov report| image:: https://codecov.io/github/BrianPugh/autoregistry/coverage.svg?branch=main\n   :target: https://codecov.io/github/BrianPugh/autoregistry?branch=main\n   :alt: Coverage\n.. |readthedocs| image:: https://readthedocs.org/projects/autoregistry/badge/?version=latest\n        :target: https://autoregistry.readthedocs.io/en/latest/?badge=latest\n        :alt: Documentation Status\n.. |Python compat| image:: https://img.shields.io/badge/>=python-3.8-blue.svg\n.. |PyPi| image:: https://img.shields.io/pypi/v/autoregistry.svg\n        :target: https://pypi.python.org/pypi/autoregistry\n',
-    'author': 'Brian Pugh',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/BrianPugh/autoregistry',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+.. inclusion-marker-do-not-remove
 
+AutoRegistry
+============
+
+Invoking functions and class-constructors from a string is a common design pattern
+that AutoRegistry aims to solve.
+For example, a user might specify a backend of type ``"sqlite"`` in a yaml configuration
+file, for which our program needs to construct the ``SQLite`` subclass of our ``Database`` class.
+Classically, you would need to manually create a lookup, mapping the string ``"sqlite"`` to
+the ``SQLite`` constructor.
+With AutoRegistry, the lookup is automatically created for you.
+
+
+AutoRegistry has a single  powerful class ``Registry`` that can do the following:
+
+* Be inherited to automatically register subclasses by their name.
+
+* Be directly invoked ``my_registry = Registry()`` to create a decorator
+  for registering callables like functions.
+
+* Traverse and automatically create registries for other python libraries.
+
+.. inclusion-marker-remove
+
+AutoRegistry is also highly configurable, with features like name-schema-enforcement and name-conversion-rules.
+`Checkout the docs for more information <https://autoregistry.readthedocs.io/en/latest/?badge=latest/>`_.
+
+`Watch AutoRegistry in action! <https://youtu.be/4No_NE7bUOM>`_
+
+Installation
+============
+AutoRegistry requires Python ``>=3.8``.
+
+.. code-block:: bash
+
+   python -m pip install autoregistry
+
+
+Examples
+========
+
+Class Inheritance
+^^^^^^^^^^^^^^^^^
+
+``Registry`` adds a dictionary-like interface to class constructors
+for looking up subclasses.
+
+.. code-block:: python
+
+   from abc import abstractmethod
+   from dataclasses import dataclass
+   from autoregistry import Registry
+
+
+   @dataclass
+   class Pokemon(Registry):
+       level: int
+       hp: int
+
+       @abstractmethod
+       def attack(self, target):
+           """Attack another Pokemon."""
+
+
+   class Charmander(Pokemon):
+       def attack(self, target):
+           return 1
+
+
+   class Pikachu(Pokemon):
+       def attack(self, target):
+           return 2
+
+
+   class SurfingPikachu(Pikachu):
+       def attack(self, target):
+           return 3
+
+
+   print(f"{len(Pokemon)} Pokemon types registered:")
+   print(f"    {list(Pokemon)}")
+   # By default, lookup is case-insensitive
+   charmander = Pokemon["cHaRmAnDer"](level=7, hp=31)
+   print(f"Created Pokemon: {charmander}")
+
+This code block produces the following output:
+
+.. code-block::
+
+   3 Pokemon types registered:
+       ['charmander', 'pikachu', 'surfingpikachu']
+   Created Pokemon: Charmander(level=7, hp=31)
+
+
+Function Registry
+^^^^^^^^^^^^^^^^^
+
+Directly instantiating a ``Registry`` object allows you to
+register functions by decorating them.
+
+.. code-block:: python
+
+   from autoregistry import Registry
+
+   pokeballs = Registry()
+
+
+   @pokeballs
+   def masterball(target):
+       return 1.0
+
+
+   @pokeballs
+   def pokeball(target):
+       return 0.1
+
+
+   for ball in ["pokeball", "masterball"]:
+       success_rate = pokeballs[ball](None)
+       print(f"Ash used {ball} and had {success_rate=}")
+
+This code block produces the following output:
+
+.. code-block:: text
+
+   Ash used pokeball and had success_rate=0.1
+   Ash used masterball and had success_rate=1.0
+
+
+Module Registry
+^^^^^^^^^^^^^^^
+
+Create a registry for another python module.
+
+.. code-block:: python
+
+   import torch
+   from autoregistry import Registry
+
+   optims = Registry(torch.optim)
+
+   # "adamw" and ``lr`` could be coming from a configuration file.
+   optimizer = optims["adamw"](model.parameters(), lr=3e-3)
+
+   assert list(optims) == [
+       "asgd",
+       "adadelta",
+       "adagrad",
+       "adam",
+       "adamw",
+       "adamax",
+       "lbfgs",
+       "nadam",
+       "optimizer",
+       "radam",
+       "rmsprop",
+       "rprop",
+       "sgd",
+       "sparseadam",
+       "lr_scheduler",
+       "swa_utils",
+   ]
+
+
+.. |GHA tests| image:: https://github.com/BrianPugh/autoregistry/workflows/tests/badge.svg
+   :target: https://github.com/BrianPugh/autoregistry/actions?query=workflow%3Atests
+   :alt: GHA Status
+.. |Codecov report| image:: https://codecov.io/github/BrianPugh/autoregistry/coverage.svg?branch=main
+   :target: https://codecov.io/github/BrianPugh/autoregistry?branch=main
+   :alt: Coverage
+.. |readthedocs| image:: https://readthedocs.org/projects/autoregistry/badge/?version=latest
+        :target: https://autoregistry.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+.. |Python compat| image:: https://img.shields.io/badge/>=python-3.8-blue.svg
+.. |PyPi| image:: https://img.shields.io/pypi/v/autoregistry.svg
+        :target: https://pypi.python.org/pypi/autoregistry
 
-setup(**setup_kwargs)
```

