# Comparing `tmp/arctix-0.0.0a23.tar.gz` & `tmp/arctix-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arctix-0.0.0a23.tar", max compression
+gzip compressed data, was "arctix-0.0.1.tar", max compression
```

## Comparing `arctix-0.0.0a23.tar` & `arctix-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1501 2023-07-16 01:43:03.184033 arctix-0.0.0a23/LICENSE
--rw-r--r--   0        0        0     2019 2023-07-16 01:43:03.184033 arctix-0.0.0a23/README.md
--rw-r--r--   0        0        0     4078 2023-07-16 01:43:03.184033 arctix-0.0.0a23/pyproject.toml
--rw-r--r--   0        0        0      689 2023-07-16 01:43:03.184033 arctix-0.0.0a23/src/arctix/__init__.py
--rw-r--r--   0        0        0     3301 2023-07-16 01:43:03.184033 arctix-0.0.0a23/src/arctix/_numpy.py
--rw-r--r--   0        0        0     3338 2023-07-16 01:43:03.184033 arctix-0.0.0a23/src/arctix/_torch.py
--rw-r--r--   0        0        0    16277 2023-07-16 01:43:03.184033 arctix-0.0.0a23/src/arctix/formatter.py
--rw-r--r--   0        0        0    18379 2023-07-16 01:43:03.184033 arctix-0.0.0a23/src/arctix/summarizer.py
--rw-r--r--   0        0        0      348 2023-07-16 01:43:03.184033 arctix-0.0.0a23/src/arctix/testing.py
--rw-r--r--   0        0        0        0 2023-07-16 01:43:03.184033 arctix-0.0.0a23/src/arctix/utils/__init__.py
--rw-r--r--   0        0        0     3399 2023-07-16 01:43:03.184033 arctix-0.0.0a23/src/arctix/utils/format.py
--rw-r--r--   0        0        0     1250 2023-07-16 01:43:03.184033 arctix-0.0.0a23/src/arctix/utils/imports.py
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 arctix-0.0.0a23/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-07-17 04:19:03.663776 arctix-0.0.1/LICENSE
+-rw-r--r--   0        0        0     5537 2023-07-17 04:19:03.663776 arctix-0.0.1/README.md
+-rw-r--r--   0        0        0     4075 2023-07-17 04:19:03.663776 arctix-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      689 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/__init__.py
+-rw-r--r--   0        0        0     3301 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/_numpy.py
+-rw-r--r--   0        0        0     3338 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/_torch.py
+-rw-r--r--   0        0        0    13603 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/formatter.py
+-rw-r--r--   0        0        0    14735 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/summarizer.py
+-rw-r--r--   0        0        0      348 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/testing.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/utils/__init__.py
+-rw-r--r--   0        0        0     3399 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/utils/format.py
+-rw-r--r--   0        0        0     1250 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/utils/imports.py
+-rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 arctix-0.0.1/PKG-INFO
```

### Comparing `arctix-0.0.0a23/LICENSE` & `arctix-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a23/pyproject.toml` & `arctix-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arctix"
-version = "0.0.0a23"
+version = "0.0.1"
 description = "A library to get a text summary of nested objects"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/arctix"
 repository = "https://github.com/durandtibo/arctix"
 keywords = []
 license = "BSD-3-Clause"
```

### Comparing `arctix-0.0.0a23/src/arctix/__init__.py` & `arctix-0.0.1/src/arctix/__init__.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a23/src/arctix/_numpy.py` & `arctix-0.0.1/src/arctix/_numpy.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a23/src/arctix/_torch.py` & `arctix-0.0.1/src/arctix/_torch.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a23/src/arctix/formatter.py` & `arctix-0.0.1/src/arctix/formatter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from __future__ import annotations
 
-__all__ = ["BaseFormatter", "DefaultFormatter", "SequenceFormatter"]
+__all__ = [
+    "BaseFormatter",
+    "DefaultFormatter",
+    "MappingFormatter",
+    "SequenceFormatter",
+    "SetFormatter",
+]
 
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence
 from itertools import islice
 from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
 from arctix.utils.format import str_indent, str_mapping, str_sequence
@@ -214,16 +220,17 @@
             raise TypeError(
                 "Incorrect type for max_characters. Expected int value but "
                 f"received {max_characters}"
             )
         self._max_characters = max_characters
 
 
-class MappingFormatter(BaseFormatter[Mapping]):
-    r"""Implements a formatter for ``Mapping``.
+class BaseCollectionFormatter(BaseFormatter[T]):
+    r"""Implement a base class to implement a formatter for
+    ``Collection``.
 
     Args:
     ----
         max_items (int, optional): Specifies the maximum number
             of items to show. If a negative value is provided,
             all the items are shown. Default: ``5``
         num_spaces (int, optional): Specifies the number of spaces
@@ -236,43 +243,21 @@
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__qualname__}(max_items={self._max_items:,}, "
             f"num_spaces={self._num_spaces})"
         )
 
-    def clone(self) -> MappingFormatter:
-        return self.__class__(max_items=self._max_items)
+    def clone(self) -> BaseCollectionFormatter:
+        return self.__class__(max_items=self._max_items, num_spaces=self._num_spaces)
 
     def equal(self, other: Any) -> bool:
         if not isinstance(other, self.__class__):
             return False
-        return self._max_items == other._max_items
-
-    def format(
-        self, summarizer: BaseSummarizer, value: Mapping, depth: int = 0, max_depth: int = 1
-    ) -> str:
-        if depth >= max_depth:
-            return summarizer.summary(str(value), depth=depth + 1, max_depth=max_depth)
-        typ = type(value)
-        length = len(value)
-        if length == 0:
-            s = str(value)
-        else:
-            s = str_mapping(
-                {
-                    key: summarizer.summary(val, depth=depth + 1, max_depth=max_depth)
-                    for key, val in islice(value.items(), self._max_items)
-                },
-                num_spaces=self._num_spaces,
-            )
-            if length > self._max_items:
-                s = f"{s}\n..."
-            s = f"(length={length:,})\n{s}"
-        return str_indent(f"{typ} {s}", num_spaces=self._num_spaces)
+        return self._max_items == other._max_items and self._num_spaces == other._num_spaces
 
     def load_state_dict(self, state: dict) -> None:
         self._max_items = state["max_items"]
         self._num_spaces = state["num_spaces"]
 
     def state_dict(self) -> dict:
         return {"max_items": self._max_items, "num_spaces": self._num_spaces}
@@ -372,162 +357,78 @@
             raise ValueError(
                 "Incorrect value for num_spaces. Expected a positive integer value but "
                 f"received {num_spaces}"
             )
         self._num_spaces = num_spaces
 
 
-class SequenceFormatter(BaseFormatter[Sequence]):
-    r"""Implements a formatter for ``Sequence``.
-
-    Args:
-    ----
-        max_items (int, optional): Specifies the maximum number
-            of items to show. If a negative value is provided,
-            all the items are shown. Default: ``5``
-        num_spaces (int, optional): Specifies the number of spaces
-            used for the indentation. Default: ``2``.
-    """
-
-    def __init__(self, max_items: int = 5, num_spaces: int = 2) -> None:
-        self.set_max_items(max_items)
-        self.set_num_spaces(num_spaces)
-        # TODO: add a compact representation mode
-
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__qualname__}(max_items={self._max_items:,}, "
-            f"num_spaces={self._num_spaces})"
-        )
-
-    def clone(self) -> SequenceFormatter:
-        return self.__class__(max_items=self._max_items)
-
-    def equal(self, other: Any) -> bool:
-        if not isinstance(other, self.__class__):
-            return False
-        return self._max_items == other._max_items
+class MappingFormatter(BaseCollectionFormatter[Mapping]):
+    r"""Implements a formatter for ``Mapping``."""
 
     def format(
-        self, summarizer: BaseSummarizer, value: Sequence, depth: int = 0, max_depth: int = 1
+        self, summarizer: BaseSummarizer, value: Mapping, depth: int = 0, max_depth: int = 1
     ) -> str:
         if depth >= max_depth:
             return summarizer.summary(str(value), depth=depth + 1, max_depth=max_depth)
         typ = type(value)
         length = len(value)
-        if length == 0:
-            s = f" {value}"
-        else:
-            s = str_sequence(
-                [
-                    summarizer.summary(val, depth=depth + 1, max_depth=max_depth)
-                    for val in value[: self._max_items]
-                ],
+        if length > 0:
+            items = value.items()
+            if self._max_items >= 0:
+                items = islice(value.items(), self._max_items)
+            value = str_mapping(
+                {
+                    key: summarizer.summary(val, depth=depth + 1, max_depth=max_depth)
+                    for key, val in items
+                },
                 num_spaces=self._num_spaces,
             )
-            s = f"\n{s}\n..." if length > self._max_items else f"\n{s}"
-        return str_indent(f"{typ} (length={length:,}){s}", num_spaces=self._num_spaces)
+            if length > self._max_items and self._max_items >= 0:
+                value = f"{value}\n..."
+            value = f"(length={length:,})\n{value}"
+        return str_indent(f"{typ} {value}", num_spaces=self._num_spaces)
 
-    def load_state_dict(self, state: dict) -> None:
-        self._max_items = state["max_items"]
-        self._num_spaces = state["num_spaces"]
 
-    def state_dict(self) -> dict:
-        return {"max_items": self._max_items, "num_spaces": self._num_spaces}
-
-    def get_max_items(self) -> int:
-        r"""Gets the maximum number of items to show.
-
-        Returns:
-        -------
-            int: The maximum number of items to show.
-
-        Example usage:
+class SequenceFormatter(BaseCollectionFormatter[Sequence]):
+    r"""Implements a formatter for ``Sequence``."""
 
-        .. code-block:: pycon
-
-            >>> from arctix.formatter import SequenceFormatter
-            >>> formatter = SequenceFormatter()
-            >>> formatter.get_max_items()
-            5
-        """
-        return self._max_items
-
-    def set_max_items(self, max_items: int) -> None:
-        r"""Set the maximum number of items to show.
-
-        Args:
-        ----
-            max_characters (int): Specifies the maximum number of
-                items to show.
-
-        Raises:
-        ------
-            TypeError if ``max_items`` is not an integer.
-
-        Example usage:
-
-        .. code-block:: pycon
-
-            >>> from arctix.formatter import SequenceFormatter
-            >>> formatter = SequenceFormatter()
-            >>> formatter.set_max_items(10)
-            >>> formatter.get_max_items()
-            10
-        """
-        if not isinstance(max_items, int):
-            raise TypeError(
-                "Incorrect type for max_items. Expected int value but " f"received {max_items}"
+    def format(
+        self, summarizer: BaseSummarizer, value: Sequence, depth: int = 0, max_depth: int = 1
+    ) -> str:
+        if depth >= max_depth:
+            return summarizer.summary(str(value), depth=depth + 1, max_depth=max_depth)
+        typ = type(value)
+        length = len(value)
+        if length > 0:
+            if self._max_items >= 0:
+                value = value[: self._max_items]
+            value = str_sequence(
+                [summarizer.summary(val, depth=depth + 1, max_depth=max_depth) for val in value],
+                num_spaces=self._num_spaces,
             )
-        self._max_items = max_items
-
-    def get_num_spaces(self) -> int:
-        r"""Gets the number of spaces for indentation.
-
-        Returns:
-        -------
-            int: The number of spaces for indentation.
+            if length > self._max_items and self._max_items > 0:
+                value = f"{value}\n..."
+            value = f"(length={length:,})\n{value}"
+        return str_indent(f"{typ} {value}", num_spaces=self._num_spaces)
 
-        Example usage:
 
-        .. code-block:: pycon
+class SetFormatter(BaseCollectionFormatter[set]):
+    r"""Implements a formatter for ``set``."""
 
-            >>> from arctix.formatter import SequenceFormatter
-            >>> formatter = SequenceFormatter()
-            >>> formatter.get_num_spaces()
-            2
-        """
-        return self._num_spaces
-
-    def set_num_spaces(self, num_spaces: int) -> None:
-        r"""Set the number of spaces for indentation.
-
-        Args:
-        ----
-            num_spaces (int): Specifies the number of spaces for
-                indentation.
-
-        Raises:
-        ------
-            TypeError if ``num_spaces`` is not an integer.
-            TValueError if ``num_spaces`` is not a positive integer.
-
-        Example usage:
-
-        .. code-block:: pycon
-
-            >>> from arctix.formatter import MappingFormatter
-            >>> formatter = MappingFormatter()
-            >>> formatter.set_num_spaces(4)
-            >>> formatter.get_num_spaces()
-            4
-        """
-        if not isinstance(num_spaces, int):
-            raise TypeError(
-                f"Incorrect type for num_spaces. Expected int value but received {num_spaces}"
-            )
-        if num_spaces < 0:
-            raise ValueError(
-                "Incorrect value for num_spaces. Expected a positive integer value but "
-                f"received {num_spaces}"
+    def format(
+        self, summarizer: BaseSummarizer, value: set, depth: int = 0, max_depth: int = 1
+    ) -> str:
+        if depth >= max_depth:
+            return summarizer.summary(str(value), depth=depth + 1, max_depth=max_depth)
+        typ = type(value)
+        length = len(value)
+        if length > 0:
+            if self._max_items >= 0:
+                value = islice(value, self._max_items)
+            value = str_sequence(
+                [summarizer.summary(val, depth=depth + 1, max_depth=max_depth) for val in value],
+                num_spaces=self._num_spaces,
             )
-        self._num_spaces = num_spaces
+            if length > self._max_items and self._max_items > 0:
+                value = f"{value}\n..."
+            value = f"(length={length:,})\n{value}"
+        return str_indent(f"{typ} {value}", num_spaces=self._num_spaces)
```

### Comparing `arctix-0.0.0a23/src/arctix/summarizer.py` & `arctix-0.0.1/src/arctix/summarizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import Any
 
 from arctix.formatter import (
     BaseFormatter,
     DefaultFormatter,
     MappingFormatter,
     SequenceFormatter,
+    SetFormatter,
 )
 from arctix.utils.format import str_indent, str_mapping
 
 
 def summary(value: Any, max_depth: int = 1, summarizer: BaseSummarizer | None = None) -> str:
     r"""Summarize the input value in a string.
 
@@ -128,14 +129,15 @@
 
     registry: dict[type[object], BaseFormatter] = {
         Mapping: MappingFormatter(),
         Sequence: SequenceFormatter(),
         dict: MappingFormatter(),
         list: SequenceFormatter(),
         object: DefaultFormatter(),
+        set: SetFormatter(),
         tuple: SequenceFormatter(),
     }
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}(\n  {str_indent(str_mapping(self.registry))}\n)"
 
     def summary(
@@ -259,33 +261,19 @@
         Example usage:
 
         .. code-block:: pycon
 
             >>> from arctix import Summarizer
             >>> Summarizer.load_state_dict({object: {"max_characters": 10}})
             >>> summarizer = Summarizer()
-            >>> summarizer
-            Summarizer(
-              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'object'>): DefaultFormatter(max_characters=10)
-              (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
-            )
+            >>> summarizer.registry[object]
+            DefaultFormatter(max_characters=10)
             >>> Summarizer.load_state_dict({object: {"max_characters": -1}})
-            >>> summarizer
-            Summarizer(
-              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'object'>): DefaultFormatter(max_characters=-1)
-              (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
-            )
+            >>> summarizer.registry[object]
+            DefaultFormatter(max_characters=-1)
         """
         for data_type, formatter in cls.registry.items():
             if (s := state.get(data_type)) is not None:
                 formatter.load_state_dict(s)
 
     @classmethod
     def state_dict(cls) -> dict:
@@ -297,15 +285,15 @@
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> from arctix import Summarizer
             >>> Summarizer.state_dict()  # doctest: +ELLIPSIS
-            {<class 'collections.abc.Mapping'>: {'max_items': 5},...
+            {<class 'collections.abc.Mapping'>: {'max_items': 5, 'num_spaces': 2},...
         """
         return {data_type: formatter.state_dict() for data_type, formatter in cls.registry.items()}
 
     @classmethod
     def set_max_characters(cls, max_characters: int) -> None:
         r"""Set the maximum of characters for the compatible formatter to
         the specified value.
@@ -320,33 +308,19 @@
         Example usage:
 
         .. code-block:: pycon
 
             >>> from arctix import Summarizer
             >>> Summarizer.set_max_characters(10)
             >>> summarizer = Summarizer()
-            >>> summarizer
-            Summarizer(
-              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'object'>): DefaultFormatter(max_characters=10)
-              (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
-            )
+            >>> summarizer.registry[object]
+            DefaultFormatter(max_characters=10)
             >>> Summarizer.set_max_characters(-1)
-            >>> summarizer
-            Summarizer(
-              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'object'>): DefaultFormatter(max_characters=-1)
-              (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
-            )
+            >>> summarizer.registry[object]
+            DefaultFormatter(max_characters=-1)
         """
         for formatter in cls.registry.values():
             if hasattr(formatter, "set_max_characters"):
                 formatter.set_max_characters(max_characters)
 
     @classmethod
     def set_max_items(cls, max_items: int) -> None:
@@ -364,33 +338,19 @@
         Example usage:
 
         .. code-block:: pycon
 
             >>> from arctix import Summarizer
             >>> Summarizer.set_max_items(10)
             >>> summarizer = Summarizer()
-            >>> summarizer
-            Summarizer(
-              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=10, num_spaces=2)
-              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=10, num_spaces=2)
-              (<class 'dict'>): MappingFormatter(max_items=10, num_spaces=2)
-              (<class 'list'>): SequenceFormatter(max_items=10, num_spaces=2)
-              (<class 'object'>): DefaultFormatter(max_characters=-1)
-              (<class 'tuple'>): SequenceFormatter(max_items=10, num_spaces=2)
-            )
+            >>> summarizer.registry[dict]
+            MappingFormatter(max_items=10, num_spaces=2)
             >>> Summarizer.set_max_items(5)
-            >>> summarizer
-            Summarizer(
-              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'object'>): DefaultFormatter(max_characters=-1)
-              (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
-            )
+            >>> summarizer.registry[dict]
+            MappingFormatter(max_items=5, num_spaces=2)
         """
         for formatter in cls.registry.values():
             if hasattr(formatter, "set_max_items"):
                 formatter.set_max_items(max_items)
 
     @classmethod
     def set_num_spaces(cls, num_spaces: int) -> None:
@@ -408,33 +368,19 @@
         Example usage:
 
         .. code-block:: pycon
 
             >>> from arctix import Summarizer
             >>> Summarizer.set_num_spaces(4)
             >>> summarizer = Summarizer()
-            >>> summarizer
-            Summarizer(
-              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=4)
-              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=4)
-              (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=4)
-              (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=4)
-              (<class 'object'>): DefaultFormatter(max_characters=-1)
-              (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=4)
-            )
+            >>> summarizer.registry[dict]
+            MappingFormatter(max_items=5, num_spaces=4)
             >>> Summarizer.set_num_spaces(2)
-            >>> summarizer
-            Summarizer(
-              (<class 'collections.abc.Mapping'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'collections.abc.Sequence'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'dict'>): MappingFormatter(max_items=5, num_spaces=2)
-              (<class 'list'>): SequenceFormatter(max_items=5, num_spaces=2)
-              (<class 'object'>): DefaultFormatter(max_characters=-1)
-              (<class 'tuple'>): SequenceFormatter(max_items=5, num_spaces=2)
-            )
+            >>> summarizer.registry[dict]
+            MappingFormatter(max_items=5, num_spaces=2)
         """
         for formatter in cls.registry.values():
             if hasattr(formatter, "set_num_spaces"):
                 formatter.set_num_spaces(num_spaces)
 
 
 def set_summarizer_options(
```

### Comparing `arctix-0.0.0a23/src/arctix/utils/format.py` & `arctix-0.0.1/src/arctix/utils/format.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.0a23/src/arctix/utils/imports.py` & `arctix-0.0.1/src/arctix/utils/imports.py`

 * *Files identical despite different names*

