# Comparing `tmp/katalytic-0.2.2.tar.gz` & `tmp/katalytic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-0.2.2.tar", last modified: Mon Jul 10 20:46:26 2023, max compression
+gzip compressed data, was "katalytic-0.3.0.tar", last modified: Mon Jul 17 18:46:36 2023, max compression
```

## Comparing `katalytic-0.2.2.tar` & `katalytic-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0     1066 2023-07-09 19:30:05.161864 katalytic-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0     4412 2023-07-10 04:57:34.292819 katalytic-0.2.2/README.md
--rw-r--r--   0        0        0     1478 2023-07-10 20:46:26.693366 katalytic-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7097 2023-07-10 20:28:25.612937 katalytic-0.2.2/src/katalytic/_pkg/__init__.py
--rw-r--r--   0        0        0    58606 2023-07-09 19:30:05.161864 katalytic-0.2.2/src/katalytic/data/__init__.py
--rw-r--r--   0        0        0    22696 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/data/checks.py
--rw-r--r--   0        0        0    51483 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/files/__init__.py
--rw-r--r--   0        0        0      130 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/katalytic.py
--rw-r--r--   0        0        0     5838 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/maths/__init__.py
--rw-r--r--   0        0        0    22812 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/maths/bboxes.py
--rw-r--r--   0        0        0     4238 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/meta/__init__.py
--rw-r--r--   0        0        0    13200 2023-07-09 19:30:05.165864 katalytic-0.2.2/tests/test_bboxes.py
--rw-r--r--   0        0        0    19288 2023-07-09 19:30:05.165864 katalytic-0.2.2/tests/test_checks.py
--rw-r--r--   0        0        0    52443 2023-07-09 19:30:05.165864 katalytic-0.2.2/tests/test_data.py
--rw-r--r--   0        0        0    67110 2023-07-10 05:03:00.709365 katalytic-0.2.2/tests/test_files.py
--rw-r--r--   0        0        0     3868 2023-07-09 19:30:05.169864 katalytic-0.2.2/tests/test_maths.py
--rw-r--r--   0        0        0     3054 2023-07-10 18:15:32.788541 katalytic-0.2.2/tests/test_meta.py
--rw-r--r--   0        0        0     2957 2023-07-10 18:19:12.880623 katalytic-0.2.2/tests/test_pkg.py
--rw-r--r--   0        0        0     6873 1970-01-01 00:00:00.000000 katalytic-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-09 19:30:05.161864 katalytic-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     4412 2023-07-10 04:57:34.292819 katalytic-0.3.0/README.md
+-rw-r--r--   0        0        0     1467 2023-07-17 18:46:36.817142 katalytic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6689 2023-07-10 10:30:52.511289 katalytic-0.3.0/src/katalytic.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      671 2023-07-10 10:30:52.535289 katalytic-0.3.0/src/katalytic.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-07-10 10:30:52.511289 katalytic-0.3.0/src/katalytic.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       87 2023-07-10 10:30:52.511289 katalytic-0.3.0/src/katalytic.egg-info/requires.txt
+-rw-r--r--   0        0        0       10 2023-07-10 10:30:52.511289 katalytic-0.3.0/src/katalytic.egg-info/top_level.txt
+-rw-r--r--   0        0        0    12706 2023-07-17 16:39:12.350069 katalytic-0.3.0/src/katalytic/_pkg/__init__.py
+-rw-r--r--   0        0        0    55003 2023-07-17 16:39:12.986070 katalytic-0.3.0/src/katalytic/data/__init__.py
+-rw-r--r--   0        0        0    22909 2023-07-17 16:39:12.246069 katalytic-0.3.0/src/katalytic/data/checks.py
+-rw-r--r--   0        0        0    55729 2023-07-17 18:44:32.804837 katalytic-0.3.0/src/katalytic/files/__init__.py
+-rw-r--r--   0        0        0      130 2023-07-17 16:39:11.810068 katalytic-0.3.0/src/katalytic/katalytic.py
+-rw-r--r--   0        0        0     6033 2023-07-17 16:39:11.994068 katalytic-0.3.0/src/katalytic/maths/__init__.py
+-rw-r--r--   0        0        0    23010 2023-07-17 16:39:12.702070 katalytic-0.3.0/src/katalytic/maths/bboxes.py
+-rw-r--r--   0        0        0     4264 2023-07-17 16:39:11.906068 katalytic-0.3.0/src/katalytic/meta/__init__.py
+-rw-r--r--   0        0        0    14079 2023-07-17 16:39:12.858070 katalytic-0.3.0/tests/test_bboxes.py
+-rw-r--r--   0        0        0    20378 2023-07-17 16:39:13.010071 katalytic-0.3.0/tests/test_checks.py
+-rw-r--r--   0        0        0    58941 2023-07-17 16:39:14.662074 katalytic-0.3.0/tests/test_data.py
+-rw-r--r--   0        0        0    68194 2023-07-17 18:44:32.804837 katalytic-0.3.0/tests/test_files.py
+-rw-r--r--   0        0        0     4180 2023-07-17 16:39:12.642070 katalytic-0.3.0/tests/test_maths.py
+-rw-r--r--   0        0        0     3266 2023-07-17 16:39:12.818070 katalytic-0.3.0/tests/test_meta.py
+-rw-r--r--   0        0        0     3032 2023-07-17 16:39:12.866070 katalytic-0.3.0/tests/test_pkg.py
+-rw-r--r--   0        0        0     6873 1970-01-01 00:00:00.000000 katalytic-0.3.0/PKG-INFO
```

### Comparing `katalytic-0.2.2/LICENSE.txt` & `katalytic-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.2/README.md` & `katalytic-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.2/pyproject.toml` & `katalytic-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.build]
 includes = [
-    "src/katalytic/",
+    "src",
 ]
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 
 [project]
 name = "katalytic"
-version = "0.2.2"
+version = "0.3.0"
 description = "We'll take care of the boilerplate, so you can focus on your problems."
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: MIT License",
```

### Comparing `katalytic-0.2.2/src/katalytic/data/__init__.py` & `katalytic-0.3.0/src/katalytic/data/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,209 +14,31 @@
 
     >>> as_dict_of_lists([['a', 'b'], [1, 2], [3, 4]])
     {'a': [1, 3], 'b': [2, 4]}
 
 """
 
 import copy
-from decimal import Decimal
-from fractions import Fraction
-from pathlib import Path
 
 from katalytic.data.checks import (
-    is_any_of, is_iterable, is_iterator, is_none_of, is_primitive, is_dict_of_sequences_uniform, is_sequence,
-    is_sequence_of_sequences_uniform, is_sequence_of_dicts_uniform
+    is_any_of,
+    is_iterable,
+    is_iterator,
+    is_none_of,
+    is_primitive,
+    is_dict_of_sequences_uniform,
+    is_sequence,
+    is_sequence_of_sequences_uniform,
+    is_sequence_of_dicts_uniform,
 )
+
 # noinspection PyProtectedMember
 from katalytic._pkg import _UNDEFINED
 
 
-def _function(): pass
-def _generator(): yield 1
-
-
-class _C:
-    def __call__(self, *args, **kwargs):
-        pass
-
-
-_map = map(int, [])
-_C_obj = _C()
-_obj = object()
-_lambda = lambda x: x
-_generator_expr = (x for x in [])
-_sequences = [[], (), range(0)]
-_dict_views = [{}.keys(), {}.values(), {}.items()]
-_iterators = [_generator, _generator_expr, iter([]), _map, enumerate([]), zip([], [])]
-_iterables = [*_dict_views, *_iterators, *_sequences, set(), {}]
-_collections = [(), set(), frozenset([]), {}, []]
-_booleans = [True, False]
-_singletons = [None, True, False]
-_primitives = [*_singletons, 0, 0.0, '', b'', bytearray(b'')]
-_callables = [_generator, _function, _lambda, _C_obj, _C]
-_numbers = [0, 0.0, 0j, Decimal('0'), Fraction(0, 1)]
-_objects = [_obj, _C_obj]
-_generators = [_generator, _generator_expr]
-_functions = [_generator, _function, _lambda]
-_strings = ['', b'', bytearray(b'')]
-
-_types = {
-    'booleans': _booleans,
-    'bytearray': bytearray(b''),
-    'bytes': b'',
-    'callables': _callables,
-    'callable_obj': _C_obj,
-    'class': _C,
-    'collections': _collections,
-    'complex': 0 + 0j,
-    'decimal': Decimal('0'),
-    'dict': {},
-    'dict_views': _dict_views,
-    'float': 0.0,
-    'fraction': Fraction(0, 1),
-    'frozenset': frozenset([]),
-    'functions': _functions,
-    'generator_expression': _generator_expr,
-    'generator_function': _generator,
-    'generators': _generators,
-    'int': 0,
-    'iterables': _iterables,
-    'iterators': _iterators,
-    'list': [],
-    'map': _map,
-    'none': None,
-    'numbers': _numbers,
-    'objects': _objects,
-    'path': Path(''),
-    'primitives': _primitives,
-    'sequences': _sequences,
-    'set': set(),
-    'singletons': _singletons,
-    'str': '',
-    'strings': _strings,
-    'tuple': (),
-}
-
-
-def all_types(whitelist=None):
-    """
-    Get all supported types or a subset of types based on a whitelist.
-
-    Args:
-        whitelist (str or Iterable[str], optional):
-            A whitelist of type names to include. If None, all supported types are returned.
-            If a string, it is treated as a single type name.
-            If an iterable of strings, it is treated as a collection of type names.
-            Defaults to None.
-
-    Returns:
-        list: A list of values for each type in the whitelist.
-
-    Raises:
-        TypeError: If whitelist is not None, a str, or an iterable.
-        ValueError: If unexpected type names are present in the whitelist.
-
-    Examples:
-        >>> all_types('numbers')
-        [0, 0.0, 0j, Decimal('0'), Fraction(0, 1)]
-        >>> all_types('singletons')
-        [None, True, False]
-
-    """
-    if whitelist is None:
-        return _flatten(_types.values())
-    elif isinstance(whitelist, str):
-        whitelist = [whitelist]
-    elif not is_iterable(whitelist):
-        raise TypeError(f'<whitelist> must be iterable. Got {type(whitelist).__name__}')
-
-    unexpected = set(whitelist) - set(_types.keys())
-    if unexpected:
-        raise ValueError(f'Unexpected types in <whitelist>: {unexpected}')
-
-    return _flatten(_types[t] for t in whitelist)
-
-
-def all_types_besides(blacklist):
-    """
-    Get all supported types except those specified in the blacklist.
-
-    Args:
-        blacklist (str or Iterable[str]):
-            A list of type names to exclude. If a string, it is treated as a single type name.
-            If an iterable of strings, it is treated as a collection of type names.
-
-    Returns:
-        list: A list of values for each type not in the blacklist.
-
-    Raises:
-        TypeError: If blacklist is not a str or iterable.
-        ValueError: If unexpected type names are present in the blacklist.
-
-    Examples:
-        >>> all_types_besides(['iterables', 'generators', 'functions', 'objects', 'path', 'numbers', 'class'])
-        [True, bytearray(b''), b'', None, '']
-
-    """
-    if isinstance(blacklist, str):
-        blacklist = [blacklist]
-    elif not is_iterable(blacklist):
-        raise TypeError(f'<blacklist> must be iterable. Got {type(blacklist).__name__}')
-
-    blacklist = set(blacklist)
-    unexpected = blacklist - set(_types.keys())
-    if unexpected:
-        raise ValueError(f'Unexpected types in <blacklist>: {unexpected}')
-
-    to_remove = _flatten(_types[t] for t in blacklist)
-    all_types = _flatten(_types.values())
-    kept = []
-    for t in all_types:
-        if t in to_remove:
-            continue
-
-        # remove duplicates too
-        # I have to do it this way because python considers
-        # 0 == 0.0 == 0j == Decimal('0') == Fraction(0, 1)
-        if (t, type(t)) in [(x, type(x)) for x in kept]:
-            continue
-
-        kept.append(t)
-
-    return kept
-
-
-def _flatten(iterable):
-    """
-    Flatten iterable with some special rules to make all_types() and
-    all_types_besides() work correctly. Use flatten() for everything else
-
-    Args:
-        iterable (Iterable): The iterable to flatten.
-
-    Returns:
-        list: An iterable flattened by one level.
-
-    Raises:
-        TypeError: If the input is not an iterable.
-
-    """
-    if not is_iterable(iterable):
-        raise TypeError(f'<iterable> expects an iterable. Got {type(iterable).__name__}')
-
-    flat = []
-    for x in iterable:
-        if isinstance(x, (dict, set, list, tuple)) and len(x):
-            flat.extend(x)
-        else:
-            flat.append(x)
-
-    return flat
-
-
 def as_dict_of_lists(data, *, empty_ok=True):
     """
     Convert data into a dictionary of lists format.
 
     This format is useful when you need to perform operations on each column
     of a table. It provides a compact representation of the data, but may be less intuitive.
 
@@ -238,29 +60,31 @@
         {'a': [1, 3], 'b': [2, 4]}
 
         >>> as_dict_of_lists([['b', 'a'], [1, 2], [3, 4]])
         {'b': [1, 3], 'a': [2, 4]}
 
     """
     if not isinstance(empty_ok, bool):
-        raise TypeError(f'<empty_ok> expects False or True. Got {type(empty_ok)}')
+        raise TypeError(f"<empty_ok> expects False or True. Got {type(empty_ok)}")
 
     if (isinstance(data, dict) or is_sequence(data)) and len(data) == 0:
         if empty_ok:
             return []
         else:
-            raise ValueError(f'Empty collection not allowed when <empty_ok> is False')
+            raise ValueError(f"Empty collection not allowed when <empty_ok> is False")
     elif is_sequence_of_dicts_uniform(data):
         return {k: [d[k] for d in data] for k in data[0]}
     elif is_sequence_of_sequences_uniform(data):
         return {k: [v[i] for v in data[1:]] for i, k in enumerate(data[0])}
     elif is_dict_of_sequences_uniform(data):
         return {k: list(v) for k, v in data.items()}
     else:
-        raise TypeError(f'Unexpected format for <data>. Got {type(data).__name__}: {data!r}')
+        raise TypeError(
+            f"Unexpected format for <data>. Got {type(data).__name__}: {data!r}"
+        )
 
 
 def as_list_of_dicts(data, *, empty_ok=True):
     """
     Convert data into a list of dictionaries format.
 
     This format is useful when you need to perform operations on each row of a table.
@@ -283,32 +107,34 @@
         [{'b': 1, 'a': 2}, {'b': 3, 'a': 4}]
 
         >>> as_list_of_dicts([{'b': 2, 'a': 1}, {'a': 3, 'b': 4}])
         [{'b': 2, 'a': 1}, {'b': 4, 'a': 3}]
 
     """
     if not isinstance(empty_ok, bool):
-        raise TypeError(f'<empty_ok> expects False or True. Got {type(empty_ok)}')
+        raise TypeError(f"<empty_ok> expects False or True. Got {type(empty_ok)}")
 
     if (isinstance(data, dict) or is_sequence(data)) and len(data) == 0:
         if empty_ok:
             return []
         else:
-            raise ValueError(f'Empty collection not allowed when <empty_ok> is False')
+            raise ValueError(f"Empty collection not allowed when <empty_ok> is False")
     elif is_sequence_of_dicts_uniform(data):
         header = list(data[0].keys())
         return [{k: d[k] for k in header} for d in data]
     elif is_sequence_of_sequences_uniform(data):
         return [dict(zip(data[0], row)) for row in data[1:]]
     elif is_dict_of_sequences_uniform(data):
         first_seq = list(data.values())[0]
         seq_len = len(first_seq)
         return [{k: v[i] for k, v in data.items()} for i in range(seq_len)]
     else:
-        raise TypeError(f'Unexpected format for <data>. Got {type(data).__name__}: {data!r}')
+        raise TypeError(
+            f"Unexpected format for <data>. Got {type(data).__name__}: {data!r}"
+        )
 
 
 def as_list_of_lists(data, *, empty_ok=True):
     """
     Convert data into a list of lists format.
 
     This format, along with the dict_of_sequences format, is the most compact for storing tabular data.
@@ -332,34 +158,36 @@
         [['a', 'b'], [1, 2], [3, 4]]
 
         >>> as_list_of_lists([['b', 'a'], [1, 2], [3, 4]])
         [['b', 'a'], [1, 2], [3, 4]]
 
     """
     if not isinstance(empty_ok, bool):
-        raise TypeError(f'<empty_ok> expects False or True. Got {type(empty_ok)}')
+        raise TypeError(f"<empty_ok> expects False or True. Got {type(empty_ok)}")
 
     if (isinstance(data, dict) or is_sequence(data)) and len(data) == 0:
         if empty_ok:
             return []
         else:
-            raise ValueError(f'Empty collection not allowed when <empty_ok> is False')
+            raise ValueError(f"Empty collection not allowed when <empty_ok> is False")
     elif is_sequence_of_dicts_uniform(data):
         header = [list(data[0].keys())]
         rows = [[d[k] for k in header[0]] for d in data]
         return header + rows
     elif is_sequence_of_sequences_uniform(data):
         return list(map(list, data))
     elif is_dict_of_sequences_uniform(data):
         header = [list(data.keys())]
         n = len(list(data.values())[0])
         rows = [[v[i] for v in data.values()] for i in range(n)]
         return header + rows
     else:
-        raise TypeError(f'Unexpected format for <data>. Got {type(data).__name__}: {data!r}')
+        raise TypeError(
+            f"Unexpected format for <data>. Got {type(data).__name__}: {data!r}"
+        )
 
 
 def detect_fronts(bits):
     """
     Detects the fronts in a sequence of bits.
 
     A front is a change from 0 to 1 (positive) or from 1 to 0 (negative).
@@ -394,22 +222,22 @@
     """
     if is_iterator(bits):
         bits = list(bits)
     elif isinstance(bits, str):
         bits = list(map(int, bits))
 
     if not all(is_any_of(b, (0, 1, True, False)) for b in bits):
-        raise TypeError(f'Only 0/1 or True/False are allowed. Got {bits!r}')
+        raise TypeError(f"Only 0/1 or True/False are allowed. Got {bits!r}")
 
     fronts = []
     for i, (a, b) in enumerate(zip(bits, bits[1:])):
         if (a, b) == (0, 1):  # it works for (False, True) as well
-            fronts.append((i+1, 1))
+            fronts.append((i + 1, 1))
         elif (a, b) == (1, 0):  # it works for (True, False) as well
-            fronts.append((i+1, -1))
+            fronts.append((i + 1, -1))
 
     return fronts
 
 
 def detect_fronts_positive(bits):
     """Detects the positive fronts (a 0 to 1 transition).
 
@@ -482,15 +310,15 @@
 
         >>> data = [1, 2, 3, 4, 5]
         >>> first(data, condition=lambda x: x % 2 == 0)
         2
 
     """
     if isinstance(data, set):
-        raise TypeError(f'<data> expects a sequence. Got set. Use `one(data)` instead')
+        raise TypeError(f"<data> expects a sequence. Got set. Use `one(data)` instead")
 
     return one(data, condition=condition)
 
 
 def first_with_idx(data, *, condition=lambda _: True):
     """
     Returns the first element and its index from a sequence.
@@ -517,17 +345,19 @@
         (0, 1)
         >>> first_with_idx([10, 20, 30, 40, 50], condition=lambda x: x % 3 == 0)
         (2, 30)
         >>> first_with_idx([1, 3, 5], condition=lambda x: x % 2 == 0)
 
     """
     if isinstance(data, set):
-        raise TypeError(f'<data> expects a sequence. Got set. Use `one(data)` instead')
+        raise TypeError(f"<data> expects a sequence. Got set. Use `one(data)` instead")
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}: {condition!r}"
+        )
 
     for i, v in enumerate(data):
         if condition(v):
             return (i, v)
 
     return None
 
@@ -546,15 +376,17 @@
         TypeError: If the input is not an iterable.
 
     Examples:
         >>>
 
     """
     if not is_iterable(iterable):
-        raise TypeError(f'<iterable> expects an iterable. Got {type(iterable).__name__}')
+        raise TypeError(
+            f"<iterable> expects an iterable. Got {type(iterable).__name__}"
+        )
 
     flat = []
     for x in iterable:
         if is_iterable(x):
             flat.extend(x)
         else:
             flat.append(x)
@@ -604,15 +436,15 @@
         5
 
         >>> last([1, 2, 3, 4, 5], condition=lambda x: x % 2 == 0)
         4
 
     """
     if isinstance(data, set):
-        raise TypeError(f'<data> expects a sequence. Got set. Use `one(data)` instead')
+        raise TypeError(f"<data> expects a sequence. Got set. Use `one(data)` instead")
 
     if is_iterator(data) or isinstance(data, dict):
         data = list(data)
 
     return one(reversed(data), condition=condition)
 
 
@@ -642,17 +474,19 @@
         (4, 5)
         >>> last_with_idx([1, 2, 3, 4, 5], condition=lambda x: x % 2 == 0)
         (3, 4)
         >>> last_with_idx([1, 3, 5], condition=lambda x: x % 2 == 0)
 
     """
     if isinstance(data, set):
-        raise TypeError(f'<data> expects a sequence. Got set. Use `one(data)` instead')
+        raise TypeError(f"<data> expects a sequence. Got set. Use `one(data)` instead")
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}: {condition!r}"
+        )
 
     if is_iterator(data) or isinstance(data, dict):
         data = list(data)
 
     for i, v in enumerate(reversed(data), start=1):
         if condition(v):
             return (len(data) - i, v)
@@ -690,19 +524,21 @@
         ...
         >>> data = {1: 'one', 2: 'two', 3: 'three'}
         >>> map_dict_keys(square, data, condition=is_even)
         {1: 'one', 4: 'two', 3: 'three'}
 
     """
     if not callable(f):
-        raise TypeError(f'<f> expects a function. Got {type(f).__name__}: {f!r}')
+        raise TypeError(f"<f> expects a function. Got {type(f).__name__}: {f!r}")
     elif not isinstance(data, dict):
-        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
-    elif not(condition is None or callable(condition)):
-        raise TypeError(f'<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(f"<data> expects a dict. Got {type(data).__name__}: {data!r}")
+    elif not (condition is None or callable(condition)):
+        raise TypeError(
+            f"<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}"
+        )
 
     if condition is None:
         return {f(k): v for k, v in data.items()}
     else:
         return {f(k) if condition(k) else k: v for k, v in data.items()}
 
 
@@ -736,19 +572,21 @@
         ...
         >>> data = {'a': 'apple', 'b': 'banana', 'c': 'cherry'}
         >>> map_dict_values(uppercase, data, condition=is_long)
         {'a': 'apple', 'b': 'BANANA', 'c': 'CHERRY'}
 
     """
     if not callable(f):
-        raise TypeError(f'<f> expects a function. Got {type(f).__name__}: {f!r}')
+        raise TypeError(f"<f> expects a function. Got {type(f).__name__}: {f!r}")
     elif not isinstance(data, dict):
-        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
-    elif not(condition is None or callable(condition)):
-        raise TypeError(f'<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(f"<data> expects a dict. Got {type(data).__name__}: {data!r}")
+    elif not (condition is None or callable(condition)):
+        raise TypeError(
+            f"<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}"
+        )
 
     if condition is None:
         return {k: f(v) for k, v in data.items()}
     else:
         return {k: f(v) if condition(v) else v for k, v in data.items()}
 
 
@@ -786,46 +624,62 @@
             >>> def double(x):
             ...     return 2 * x
             >>> map_recursive(double, data)
             {'a': [2, 4, 6], 'b': {'c': [8, 10, 12]}}
 
     """
     if not callable(f):
-        raise TypeError(f'<f> expects a function. Got {type(f).__name__}: {f!r}')
+        raise TypeError(f"<f> expects a function. Got {type(f).__name__}: {f!r}")
     elif not is_iterable(data):
-        raise TypeError(f'<data> expects an iterable. Got {type(data).__name__}: {data!r}')
-    elif not(condition is None or callable(condition)):
-        raise TypeError(f'<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<data> expects an iterable. Got {type(data).__name__}: {data!r}"
+        )
+    elif not (condition is None or callable(condition)):
+        raise TypeError(
+            f"<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}"
+        )
     elif not isinstance(on_dict_keys, bool):
-        raise TypeError(f'<on_dict_keys> expects True or False. Got {type(on_dict_keys).__name__}: {on_dict_keys!r}')
+        raise TypeError(
+            f"<on_dict_keys> expects True or False. Got {type(on_dict_keys).__name__}: {on_dict_keys!r}"
+        )
 
     if is_iterator(data):
         new_data = (
             map_recursive(f, v, condition=condition, on_dict_keys=on_dict_keys)
-            if is_iterable(v) else f(v) if condition(v) else v for v in data
+            if is_iterable(v)
+            else f(v)
+            if condition(v)
+            else v
+            for v in data
         )
     elif isinstance(data, dict):
         new_data = {}
         for k, v in data.items():
             if on_dict_keys:
                 if is_iterable(k):
-                    k = map_recursive(f, k, condition=condition, on_dict_keys=on_dict_keys)
+                    k = map_recursive(
+                        f, k, condition=condition, on_dict_keys=on_dict_keys
+                    )
                 if condition(k):
                     k = f(k)
 
             if is_iterable(v):
                 v = map_recursive(f, v, condition=condition, on_dict_keys=on_dict_keys)
             if condition(v):
                 v = f(v)
 
             new_data[k] = v
     else:
         new_data = type(data)(
             map_recursive(f, v, condition=condition, on_dict_keys=on_dict_keys)
-            if is_iterable(v) else f(v) if condition(v) else v for v in data
+            if is_iterable(v)
+            else f(v)
+            if condition(v)
+            else v
+            for v in data
         )
 
     if condition(new_data):
         return f(new_data)
     else:
         return new_data
 
@@ -855,17 +709,21 @@
         2
 
         >>> data = [1, 3, 5]
         >>> one(data, condition=lambda x: x % 2 == 0)
 
     """
     if not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}: {condition!r}"
+        )
     elif not is_iterable(data):
-        raise TypeError(f'<data> expects an iterable. Got {type(data).__name__}: {data!r}')
+        raise TypeError(
+            f"<data> expects an iterable. Got {type(data).__name__}: {data!r}"
+        )
 
     try:
         return next(filter(condition, data))
     except StopIteration:
         return None
 
 
@@ -903,27 +761,34 @@
         2. Pop the minimum element from a list using a condition function:
             >>> data = ['apple', 'banana', 'cherry']
             >>> pop_min(data, condition=len)
             ('apple', ['banana', 'cherry'])
 
     """
     if not is_iterable(data):
-        raise TypeError(f'<data> expects an iterable. Got {type(data).__name__}: {data!r}')
+        raise TypeError(
+            f"<data> expects an iterable. Got {type(data).__name__}: {data!r}"
+        )
     elif isinstance(data, dict):
         raise TypeError(
-            '<data> expects any iterable besides dict. '
-            'For dict, use `pop_min_key` or `pop_min_value` instead')
+            "<data> expects any iterable besides dict. "
+            "For dict, use `pop_min_key` or `pop_min_value` instead"
+        )
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}: {condition!r}"
+        )
 
     original_type = type(data)
     data = [copy.deepcopy(item) for item in data]
     found = min(data, key=condition, default=_UNDEFINED)
     if found is _UNDEFINED and default is _UNDEFINED:
-        raise ValueError('Cannot pop from an empty collection unless a default value is provided')
+        raise ValueError(
+            "Cannot pop from an empty collection unless a default value is provided"
+        )
 
     data.remove(found)
     if original_type in (list, tuple, set, frozenset):
         return found, original_type(data)
     else:
         return found, data
 
@@ -962,27 +827,34 @@
         2. Pop the maximum element from a list using a condition function:
             >>> data = ['apple', 'banana', 'cherry']
             >>> pop_max(data, condition=len)
             ('banana', ['apple', 'cherry'])
 
     """
     if not is_iterable(data):
-        raise TypeError(f'<data> expects an iterable. Got {type(data).__name__}: {data!r}')
+        raise TypeError(
+            f"<data> expects an iterable. Got {type(data).__name__}: {data!r}"
+        )
     elif isinstance(data, dict):
         raise TypeError(
-            '<data> expects any iterable besides dict. '
-            'For dict, use `pop_max_key` or `pop_max_value` instead')
+            "<data> expects any iterable besides dict. "
+            "For dict, use `pop_max_key` or `pop_max_value` instead"
+        )
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}: {condition!r}"
+        )
 
     original_type = type(data)
     data = [copy.deepcopy(item) for item in data]
     found = max(data, key=condition, default=_UNDEFINED)
     if found is _UNDEFINED and default is _UNDEFINED:
-        raise ValueError('Cannot pop from an empty collection unless a default value is provided')
+        raise ValueError(
+            "Cannot pop from an empty collection unless a default value is provided"
+        )
 
     data.remove(found)
     if original_type in (list, tuple, set, frozenset):
         return found, original_type(data)
     else:
         return found, data
 
@@ -1018,22 +890,26 @@
         2. Pop the maximum (key, value) pair from a dictionary using a condition function:
             >>> data = {'apple': 3, 'banana': 2, 'cherry': 5}
             >>> pop_max_by_dict_key(data, condition=len)
             (('banana', 2), {'apple': 3, 'cherry': 5})
 
     """
     if not isinstance(data, dict):
-        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
+        raise TypeError(f"<data> expects a dict. Got {type(data).__name__}: {data!r}")
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}: {condition!r}"
+        )
 
     data = copy.deepcopy(data)
     dict_key = max(data.keys(), key=condition, default=_UNDEFINED)
     if dict_key is _UNDEFINED and default is _UNDEFINED:
-        raise ValueError('Cannot pop from an empty dict unless a default value is provided')
+        raise ValueError(
+            "Cannot pop from an empty dict unless a default value is provided"
+        )
 
     value = data.pop(dict_key)
     return (dict_key, value), data
 
 
 def pop_min_by_dict_key(data, *, condition=lambda x: x, default=_UNDEFINED):
     """
@@ -1066,22 +942,26 @@
         2. Pop the minimum (key, value) pair from a dictionary using a condition function:
             >>> data = {'apple': 3, 'banana': 2, 'cherry': 5}
             >>> pop_min_by_dict_key(data, condition=len)
             (('apple', 3), {'banana': 2, 'cherry': 5})
 
     """
     if not isinstance(data, dict):
-        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
+        raise TypeError(f"<data> expects a dict. Got {type(data).__name__}: {data!r}")
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}: {condition!r}"
+        )
 
     data = copy.deepcopy(data)
     dict_key = min(data.keys(), key=condition, default=_UNDEFINED)
     if dict_key is _UNDEFINED and default is _UNDEFINED:
-        raise ValueError('Cannot pop from an empty dict unless a default value is provided')
+        raise ValueError(
+            "Cannot pop from an empty dict unless a default value is provided"
+        )
 
     value = data.pop(dict_key)
     return (dict_key, value), data
 
 
 def pop_max_by_dict_value(data, *, condition=lambda x: x, default=_UNDEFINED):
     """
@@ -1108,22 +988,26 @@
     Examples:
         >>> data = {'a': 1, 'b': 2, 'c': 3}
         >>> pop_max_by_dict_value(data)
         (('c', 3), {'a': 1, 'b': 2})
 
     """
     if not isinstance(data, dict):
-        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
+        raise TypeError(f"<data> expects a dict. Got {type(data).__name__}: {data!r}")
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}: {condition!r}"
+        )
 
     data = copy.deepcopy(data)
     item = max(data.items(), key=lambda kv: condition(kv[1]), default=_UNDEFINED)
     if item is _UNDEFINED and default is _UNDEFINED:
-        raise ValueError('Cannot pop from an empty dict unless a default value is provided')
+        raise ValueError(
+            "Cannot pop from an empty dict unless a default value is provided"
+        )
 
     _ = data.pop(item[0])
     return item, data
 
 
 def pop_min_by_dict_value(data, *, condition=lambda x: x, default=_UNDEFINED):
     """
@@ -1150,22 +1034,26 @@
     Examples:
         >>> data = {'a': 1, 'b': 2, 'c': 3}
         >>> pop_min_by_dict_value(data)
         (('a', 1), {'b': 2, 'c': 3})
 
     """
     if not isinstance(data, dict):
-        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
+        raise TypeError(f"<data> expects a dict. Got {type(data).__name__}: {data!r}")
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}: {condition!r}"
+        )
 
     data = copy.deepcopy(data)
     item = min(data.items(), key=lambda kv: condition(kv[1]), default=_UNDEFINED)
     if item is _UNDEFINED and default is _UNDEFINED:
-        raise ValueError('Cannot pop from an empty dict unless a default value is provided')
+        raise ValueError(
+            "Cannot pop from an empty dict unless a default value is provided"
+        )
 
     _ = data.pop(item[0])
     return item, data
 
 
 def pick_all(needles, haystack):
     """
@@ -1185,17 +1073,21 @@
         >>> needles = [2, 4, 6]
         >>> haystack = [1, 2, 3, 4, 5, 6]
         >>> pick_all(needles, haystack)
         [2, 4, 6]
 
     """
     if not is_iterable(needles):
-        raise TypeError(f'<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}')
+        raise TypeError(
+            f"<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}"
+        )
     elif not is_iterable(haystack):
-        raise TypeError(f'<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}')
+        raise TypeError(
+            f"<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}"
+        )
 
     return [needle for needle in needles if is_any_of(needle, haystack)]
 
 
 def pick_all_besides(needles, haystack):
     """
     Returns a list of elements from the needles that are not present in the haystack.
@@ -1214,17 +1106,21 @@
         >>> needles = [2, 4, 6, 7]
         >>> haystack = [1, 2, 3, 4, 5]
         >>> pick_all_besides(needles, haystack)
         [6, 7]
 
     """
     if not is_iterable(needles):
-        raise TypeError(f'<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}')
+        raise TypeError(
+            f"<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}"
+        )
     elif not is_iterable(haystack):
-        raise TypeError(f'<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}')
+        raise TypeError(
+            f"<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}"
+        )
 
     return [needle for needle in needles if is_none_of(needle, haystack)]
 
 
 def pick_any(needles, haystack):
     """
     Returns the first element from the needles that is present in the haystack.
@@ -1243,17 +1139,21 @@
         >>> needles = [2, 4, 6]
         >>> haystack = [1, 2, 3, 4, 5, 6]
         >>> pick_any(needles, haystack)
         2
 
     """
     if not is_iterable(needles):
-        raise TypeError(f'<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}')
+        raise TypeError(
+            f"<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}"
+        )
     elif not is_iterable(haystack):
-        raise TypeError(f'<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}')
+        raise TypeError(
+            f"<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}"
+        )
 
     for needle in needles:
         if is_any_of(needle, haystack):
             return needle
 
     return None
 
@@ -1279,24 +1179,30 @@
     Examples:
         >>> data = {'b': 2, 'a': 1, 'c': 3}
         >>> sort_dict_by_keys(data)
         {'a': 1, 'b': 2, 'c': 3}
 
     """
     if not isinstance(data, dict):
-        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
-    elif not(condition is None or callable(condition)):
-        raise TypeError(f'<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(f"<data> expects a dict. Got {type(data).__name__}: {data!r}")
+    elif not (condition is None or callable(condition)):
+        raise TypeError(
+            f"<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}"
+        )
     elif not isinstance(reverse, bool):
-        raise TypeError(f'<reverse> expects True or False. Got {type(reverse).__name__}: {reverse!r}')
+        raise TypeError(
+            f"<reverse> expects True or False. Got {type(reverse).__name__}: {reverse!r}"
+        )
 
     if condition is None:
         return dict(sorted(data.items(), reverse=reverse))
     else:
-        return dict(sorted(data.items(), key=lambda kv: condition(kv[0]), reverse=reverse))
+        return dict(
+            sorted(data.items(), key=lambda kv: condition(kv[0]), reverse=reverse)
+        )
 
 
 def sort_dict_by_keys_recursive(data, *, condition=None, reverse=False):
     """
     Recursively sorts a dictionary and its nested containers by their keys and returns a new structure.
 
     Args:
@@ -1316,32 +1222,51 @@
     Examples:
         >>> data = {'b': {'c': 30, 'b': 20, 'a': 10}, 'a': {'c': 3, 'b': 2, 'a': 1}}
         >>> sort_dict_by_keys_recursive(data)
         {'a': {'a': 1, 'b': 2, 'c': 3}, 'b': {'a': 10, 'b': 20, 'c': 30}}
 
     """
     if not is_iterable(data):
-        raise TypeError(f'<data> expects an iterable. Got {type(data).__name__}: {data!r}')
-    elif not(condition is None or callable(condition)):
-        raise TypeError(f'<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<data> expects an iterable. Got {type(data).__name__}: {data!r}"
+        )
+    elif not (condition is None or callable(condition)):
+        raise TypeError(
+            f"<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}"
+        )
     elif not isinstance(reverse, bool):
-        raise TypeError(f'<reverse> expects True or False. Got {type(reverse).__name__}: {reverse!r}')
+        raise TypeError(
+            f"<reverse> expects True or False. Got {type(reverse).__name__}: {reverse!r}"
+        )
 
     if isinstance(data, dict):
         return sort_dict_by_keys(
-            {k: sort_dict_by_keys_recursive(v, condition=condition, reverse=reverse) if is_iterable(v) else v
-                for k, v in data.items()},
+            {
+                k: sort_dict_by_keys_recursive(v, condition=condition, reverse=reverse)
+                if is_iterable(v)
+                else v
+                for k, v in data.items()
+            },
             condition=condition,
-            reverse=reverse)
+            reverse=reverse,
+        )
     elif is_iterator(data):
-        return (sort_dict_by_keys_recursive(v, condition=condition, reverse=reverse) if is_iterable(v) else v
-                for v in data)
+        return (
+            sort_dict_by_keys_recursive(v, condition=condition, reverse=reverse)
+            if is_iterable(v)
+            else v
+            for v in data
+        )
     elif is_iterable(data):
-        return type(data)(sort_dict_by_keys_recursive(v, condition=condition, reverse=reverse) if is_iterable(v) else v
-                          for v in data)
+        return type(data)(
+            sort_dict_by_keys_recursive(v, condition=condition, reverse=reverse)
+            if is_iterable(v)
+            else v
+            for v in data
+        )
 
 
 def sort_dict_by_values(data, *, condition=None, reverse=False):
     """
     Sorts a dictionary by its values and returns a new dictionary.
 
     Args:
@@ -1361,24 +1286,30 @@
     Examples:
         >>> data = {'a': 3, 'b': 1, 'c': 2}
         >>> sort_dict_by_values(data)
         {'b': 1, 'c': 2, 'a': 3}
 
     """
     if not isinstance(data, dict):
-        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
-    elif not(condition is None or callable(condition)):
-        raise TypeError(f'<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(f"<data> expects a dict. Got {type(data).__name__}: {data!r}")
+    elif not (condition is None or callable(condition)):
+        raise TypeError(
+            f"<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}"
+        )
     elif not isinstance(reverse, bool):
-        raise TypeError(f'<reverse> expects True or False. Got {type(reverse).__name__}: {reverse!r}')
+        raise TypeError(
+            f"<reverse> expects True or False. Got {type(reverse).__name__}: {reverse!r}"
+        )
 
     if condition is None:
         return dict(sorted(data.items(), key=lambda kv: kv[1], reverse=reverse))
     else:
-        return dict(sorted(data.items(), key=lambda kv: condition(kv[1]), reverse=reverse))
+        return dict(
+            sorted(data.items(), key=lambda kv: condition(kv[1]), reverse=reverse)
+        )
 
 
 def sort_dict_by_values_recursive(data, *, condition=None, reverse=False):
     """
     Recursively sorts a dictionary and its nested containers by their values and returns a new structure.
 
     Args:
@@ -1393,38 +1324,65 @@
         A new structure with the nested dictionaries and containers sorted by values.
 
     Raises:
         TypeError: If data is not an iterable, condition is not callable or None, or reverse is not a boolean.
 
     """
     if not is_iterable(data):
-        raise TypeError(f'<data> expects an iterable. Got {type(data).__name__}: {data!r}')
-    elif not(condition is None or callable(condition)):
-        raise TypeError(f'<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}')
+        raise TypeError(
+            f"<data> expects an iterable. Got {type(data).__name__}: {data!r}"
+        )
+    elif not (condition is None or callable(condition)):
+        raise TypeError(
+            f"<condition> expects None or a function. Got {type(condition).__name__}: {condition!r}"
+        )
     elif not isinstance(reverse, bool):
-        raise TypeError(f'<reverse> expects True or False. Got {type(reverse).__name__}: {reverse!r}')
+        raise TypeError(
+            f"<reverse> expects True or False. Got {type(reverse).__name__}: {reverse!r}"
+        )
 
     if isinstance(data, dict):
         return sort_dict_by_values(
-            {k: sort_dict_by_values_recursive(v, condition=condition, reverse=reverse) if is_iterable(v) else v
-                for k, v in data.items()},
+            {
+                k: sort_dict_by_values_recursive(
+                    v, condition=condition, reverse=reverse
+                )
+                if is_iterable(v)
+                else v
+                for k, v in data.items()
+            },
             condition=condition,
-            reverse=reverse)
+            reverse=reverse,
+        )
     elif is_iterator(data):
-        return (sort_dict_by_values_recursive(v, condition=condition, reverse=reverse) if is_iterable(v) else v
-                for v in data)
+        return (
+            sort_dict_by_values_recursive(v, condition=condition, reverse=reverse)
+            if is_iterable(v)
+            else v
+            for v in data
+        )
     elif is_iterable(data):
         return type(data)(
-            sort_dict_by_values_recursive(v, condition=condition, reverse=reverse) if is_iterable(v) else v
-            for v in data)
+            sort_dict_by_values_recursive(v, condition=condition, reverse=reverse)
+            if is_iterable(v)
+            else v
+            for v in data
+        )
 
 
 def sort_recursive(
-    data, *, condition=lambda x: x, reverse=False, sort_dicts_by='keys',
-    sort_iters=True, sort_lists=True, sort_sets=True, sort_tuples=True
+    data,
+    *,
+    condition=lambda x: x,
+    reverse=False,
+    sort_dicts_by="keys",
+    sort_iters=True,
+    sort_lists=True,
+    sort_sets=True,
+    sort_tuples=True,
 ):
     """
     Recursively sorts an iterable data structure with customizable sorting options.
     The collections are sorted from the innermost to the outermost one
 
     Args:
         data: The data structure to be sorted. Must be an iterable.
@@ -1451,49 +1409,68 @@
     Examples:
         >>> data = [{'c': 3, 'b': {'z': 3, 'x': 2, 'y': 1}, 'a': 1}]
         >>> sort_recursive(data)
         [{'a': 1, 'b': {'x': 2, 'y': 1, 'z': 3}, 'c': 3}]
 
     """
     if not is_iterable(data):
-        raise TypeError(f'<data> expects an iterable. Got {type(data).__name__}')
+        raise TypeError(f"<data> expects an iterable. Got {type(data).__name__}")
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}"
+        )
     elif not isinstance(reverse, bool):
-        raise TypeError(f'<reverse> expects True or False. Got {type(reverse).__name__}')
-    elif is_none_of(sort_dicts_by, ('keys', 'values', None)):
-        raise ValueError(f'<sort_dicts_by> expects "keys", "values" or None. Got {sort_dicts_by!r}')
+        raise TypeError(
+            f"<reverse> expects True or False. Got {type(reverse).__name__}"
+        )
+    elif is_none_of(sort_dicts_by, ("keys", "values", None)):
+        raise ValueError(
+            f'<sort_dicts_by> expects "keys", "values" or None. Got {sort_dicts_by!r}'
+        )
     elif not isinstance(sort_iters, bool):
-        raise TypeError(f'<sort_iters> expects True or False. Got {type(sort_iters).__name__}')
+        raise TypeError(
+            f"<sort_iters> expects True or False. Got {type(sort_iters).__name__}"
+        )
     elif not isinstance(sort_lists, bool):
-        raise TypeError(f'<sort_lists> expects True or False. Got {type(sort_lists).__name__}')
+        raise TypeError(
+            f"<sort_lists> expects True or False. Got {type(sort_lists).__name__}"
+        )
     elif not isinstance(sort_sets, bool):
-        raise TypeError(f'<sort_sets> expects True or False. Got {type(sort_sets).__name__}')
+        raise TypeError(
+            f"<sort_sets> expects True or False. Got {type(sort_sets).__name__}"
+        )
     elif not isinstance(sort_tuples, bool):
-        raise TypeError(f'<sort_tuples> expects True or False. Got {type(sort_tuples).__name__}')
+        raise TypeError(
+            f"<sort_tuples> expects True or False. Got {type(sort_tuples).__name__}"
+        )
 
     initial_type = type(data)
     kwargs = {
-        'condition': condition,
-        'reverse': reverse,
-        'sort_dicts_by': sort_dicts_by,
-        'sort_iters': sort_iters,
-        'sort_lists': sort_lists,
-        'sort_sets': sort_sets,
-        'sort_tuples': sort_tuples,
+        "condition": condition,
+        "reverse": reverse,
+        "sort_dicts_by": sort_dicts_by,
+        "sort_iters": sort_iters,
+        "sort_lists": sort_lists,
+        "sort_sets": sort_sets,
+        "sort_tuples": sort_tuples,
     }
 
     if isinstance(data, dict):
         # You shouldn't sort the keys, even if they are tuple,
         # as they are likely to be used as IDs
-        inner_sorted = {k: sort_recursive(v, **kwargs) if is_iterable(v) else v for k, v in data.items()}
-        if sort_dicts_by == 'keys':
+        inner_sorted = {
+            k: sort_recursive(v, **kwargs) if is_iterable(v) else v
+            for k, v in data.items()
+        }
+        if sort_dicts_by == "keys":
             return sort_dict_by_keys(inner_sorted, condition=condition, reverse=reverse)
-        elif sort_dicts_by == 'values':
-            return sort_dict_by_values(inner_sorted, condition=condition, reverse=reverse)
+        elif sort_dicts_by == "values":
+            return sort_dict_by_values(
+                inner_sorted, condition=condition, reverse=reverse
+            )
         else:
             return inner_sorted
 
     inner_sorted = (sort_recursive(v, **kwargs) if is_iterable(v) else v for v in data)
     if is_iterator(data) and not sort_iters:
         return inner_sorted
     elif isinstance(data, list) and not sort_lists:
@@ -1505,15 +1482,17 @@
     elif is_iterator(data) or isinstance(data, (set, list, tuple)):
         data = sorted(inner_sorted, key=condition, reverse=reverse)
         if initial_type == tuple:
             return tuple(data)
         else:
             return data
     else:  # pragma: no cover
-        raise AssertionError(f'Unexpected branch for <data> of type {type(data).__name__}')
+        raise AssertionError(
+            f"Unexpected branch for <data> of type {type(data).__name__}"
+        )
 
 
 def swap_keys_and_values(data):
     """
     Swaps the keys and values in a dictionary.
 
     Args:
@@ -1528,15 +1507,15 @@
     Examples:
         Swap keys and values in a dictionary:
             >>> swap_keys_and_values({'a': 1, 'b': 2, 'c': 3})
             {1: 'a', 2: 'b', 3: 'c'}
 
     """
     if not isinstance(data, dict):
-        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}')
+        raise TypeError(f"<data> expects a dict. Got {type(data).__name__}")
 
     return {v: k for k, v in data.items()}
 
 
 def xor(*values, condition=bool):
     """
     Performs an exclusive OR (XOR) operation on multiple values using a condition function.
@@ -1563,17 +1542,19 @@
             >>> xor('hello', '', 'world', condition=len)
 
             >>> xor('', 'hello', '', condition=len)
             'hello'
 
     """
     if len(values) < 2:
-        raise ValueError('<values> expects at least two values')
+        raise ValueError("<values> expects at least two values")
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}"
+        )
 
     v = None
     for value in values:
         if condition(value):
             if v is None:
                 v = value
             else:
@@ -1608,25 +1589,28 @@
             >>> xor_with_idx('hello', '', 'world', condition=len)
 
             >>> xor_with_idx('', 'hello', '', condition=len)
             (1, 'hello')
 
     """
     if len(values) < 2:
-        raise ValueError('<values> expects at least two values')
+        raise ValueError("<values> expects at least two values")
     elif not callable(condition):
-        raise TypeError(f'<condition> expects a function. Got {type(condition).__name__}')
+        raise TypeError(
+            f"<condition> expects a function. Got {type(condition).__name__}"
+        )
 
     v = None
     for i, value in enumerate(values):
         if condition(value):
             if v is None:
                 v = (i, value)
             else:
                 return None
 
     return v
 
 
-if __name__ == '__main__':  # pragma: no cover
+if __name__ == "__main__":  # pragma: no cover
     import doctest
+
     doctest.testmod()
```

### Comparing `katalytic-0.2.2/src/katalytic/data/checks.py` & `katalytic-0.3.0/src/katalytic/data/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,21 @@
         >>> contains_all_of([4, True, None, 1, 3], [1, True, 3])
         True
         >>> contains_all_of([1, 2, True], [1, 2, 3])
         False
 
     """
     if not is_iterable(haystack):
-        raise TypeError(f'<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}')
+        raise TypeError(
+            f"<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}"
+        )
     elif not is_iterable(needles):
-        raise TypeError(f'<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}')
+        raise TypeError(
+            f"<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}"
+        )
 
     for needle in needles:
         if not is_any_of(needle, haystack):
             return False
 
     return True
 
@@ -83,17 +87,21 @@
         >>> contains_any_of([1, True, 3], [4, True, None])
         True
         >>> contains_any_of([1, 2, 3], [4, True, None])
         False
 
     """
     if not is_iterable(haystack):
-        raise TypeError(f'<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}')
+        raise TypeError(
+            f"<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}"
+        )
     elif not is_iterable(needles):
-        raise TypeError(f'<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}')
+        raise TypeError(
+            f"<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}"
+        )
 
     for needle in needles:
         if is_any_of(needle, haystack):
             return True
 
     return False
 
@@ -150,38 +158,42 @@
         >>> dicts_share_key_order({'a': 1, 'b': 2}, {'c': 1, 'd': 2})
         False
         >>> dicts_share_key_order({'a': 1, 'b': 2}, {'c': 1})
         False
 
     """
     if not isinstance(recursive, bool):
-        raise TypeError(f'<dict_2> must be True or False. Got {type(recursive)}')
+        raise TypeError(f"<dict_2> must be True or False. Got {type(recursive)}")
 
     if isinstance(dict_1, dict):
         if not isinstance(dict_2, dict):
-            raise TypeError(f'<dict_2> must be a dict. Got {type(dict_2)}')
+            raise TypeError(f"<dict_2> must be a dict. Got {type(dict_2)}")
 
         if list(dict_1.keys()) != list(dict_2.keys()):
             return False
 
         if recursive:
             return all(
                 dicts_share_key_order(v_1, v_2, recursive=recursive)
-                for v_1, v_2 in zip(dict_1.values(), dict_2.values()))
+                for v_1, v_2 in zip(dict_1.values(), dict_2.values())
+            )
         else:
             return True
     elif recursive and is_sequence(dict_1):
         if not is_sequence(dict_2):
-            raise TypeError(f'<dict_2> must be a sequence. Got {type(dict_2)}')
+            raise TypeError(f"<dict_2> must be a sequence. Got {type(dict_2)}")
 
         return all(
             dicts_share_key_order(d_1, d_2, recursive=recursive)
-            for d_1, d_2 in zip(dict_1, dict_2))
+            for d_1, d_2 in zip(dict_1, dict_2)
+        )
     elif not recursive:
-        raise TypeError(f'<dict_1> and <dict_2> must be dicts. Got {type(dict_1)} and {type(dict_2)}')
+        raise TypeError(
+            f"<dict_1> and <dict_2> must be dicts. Got {type(dict_1)} and {type(dict_2)}"
+        )
     else:
         return True
 
 
 def dicts_share_value_order(dict_1, dict_2, recursive=False):
     """
     Check if two dictionaries share the same value order.
@@ -208,35 +220,39 @@
         >>> dicts_share_value_order({'a': 1, 'b': 2}, {'c': 1, 'd': 3})
         False
         >>> dicts_share_value_order({'a': 1, 'b': 2}, {'c': 1})
         False
 
     """
     if not isinstance(recursive, bool):
-        raise TypeError(f'<dict_2> must be True or False. Got {type(recursive)}')
+        raise TypeError(f"<dict_2> must be True or False. Got {type(recursive)}")
 
     if isinstance(dict_1, dict):
         if not isinstance(dict_2, dict):
-            raise TypeError(f'<dict_2> must be a dict. Got {type(dict_2)}')
+            raise TypeError(f"<dict_2> must be a dict. Got {type(dict_2)}")
 
         if list(dict_1.values()) != list(dict_2.values()):
             return False
 
         if recursive:
             return all(
                 dicts_share_value_order(v_1, v_2, recursive=recursive)
-                for v_1, v_2 in zip(dict_1.values(), dict_2.values()))
+                for v_1, v_2 in zip(dict_1.values(), dict_2.values())
+            )
         else:
             return True
     elif recursive and is_sequence(dict_1):
         return all(
             dicts_share_value_order(d_1, d_2, recursive=recursive)
-            for d_1, d_2 in zip(dict_1, dict_2))
+            for d_1, d_2 in zip(dict_1, dict_2)
+        )
     elif not recursive:
-        raise TypeError(f'<dict_1> and <dict_2> must be dicts. Got {type(dict_1)} and {type(dict_2)}')
+        raise TypeError(
+            f"<dict_1> and <dict_2> must be dicts. Got {type(dict_1)} and {type(dict_2)}"
+        )
     else:
         return True
 
 
 def is_any_of(needle, haystack):
     """
     Check if the needle is in the haystack. This correctly compares singletons (None, True, False)
@@ -262,15 +278,17 @@
         >>> is_any_of(0, [1, 2, 3])
         False
         >>> is_any_of(True, [1, 2, 3])
         False
 
     """
     if not is_iterable(haystack):
-        raise TypeError(f'<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}')
+        raise TypeError(
+            f"<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}"
+        )
 
     return any(is_equal(needle, x) for x in haystack)
 
 
 def is_dict_of_sequences(x, *, empty_ok=True):
     """
     Check if the input is a dictionary where all values are sequences.
@@ -295,15 +313,15 @@
         >>> is_dict_of_sequences({}, empty_ok=False)
         False
         >>> is_dict_of_sequences({}, empty_ok=True)
         True
 
     """
     if not isinstance(empty_ok, bool):
-        raise TypeError(f'<empty_ok> expects False or True. Got {type(empty_ok)}')
+        raise TypeError(f"<empty_ok> expects False or True. Got {type(empty_ok)}")
 
     if isinstance(x, dict):
         if len(x) >= 1 and all(is_sequence(v) for v in x.values()):
             return True
         elif len(x) == 0 and empty_ok:
             return True
 
@@ -643,15 +661,17 @@
         False
         >>> is_sequence({1, 2, 3})
         False
         >>> is_sequence({'a': 1})
         False
 
     """
-    return isinstance(x, collections.abc.Sequence) and not isinstance(x, (str, bytes, bytearray))
+    return isinstance(x, collections.abc.Sequence) and not isinstance(
+        x, (str, bytes, bytearray)
+    )
 
 
 def is_sequence_of_dicts(x, *, empty_ok=True):
     """
     Check if an object is a sequence of dictionaries.
 
     Args:
@@ -671,15 +691,15 @@
         >>> is_sequence_of_dicts([], empty_ok=False)
         False
         >>> is_sequence_of_dicts([], empty_ok=True)
         True
 
     """
     if not isinstance(empty_ok, bool):
-        raise TypeError(f'<empty_ok> expects False or True. Got {type(empty_ok)}')
+        raise TypeError(f"<empty_ok> expects False or True. Got {type(empty_ok)}")
 
     if is_sequence(x):
         if len(x) >= 1 and all(isinstance(xi, dict) for xi in x):
             return True
         elif len(x) == 0 and empty_ok:
             return True
 
@@ -740,15 +760,15 @@
         >>> is_sequence_of_sequences([], empty_ok=False)
         False
         >>> is_sequence_of_sequences([], empty_ok=True)
         True
 
     """
     if not isinstance(empty_ok, bool):
-        raise TypeError(f'<empty_ok> expects False or True. Got {type(empty_ok)}')
+        raise TypeError(f"<empty_ok> expects False or True. Got {type(empty_ok)}")
 
     if is_sequence(x):
         if len(x) >= 1 and all(is_sequence(xi) for xi in x):
             return True
         elif len(x) == 0 and empty_ok:
             return True
 
@@ -834,10 +854,11 @@
         >>> is_singleton({'a': 1})
         False
 
     """
     return isinstance(x, (bool, type(None)))
 
 
-if __name__ == '__main__':  # pragma: no cover
+if __name__ == "__main__":  # pragma: no cover
     import doctest
+
     doctest.testmod()
```

### Comparing `katalytic-0.2.2/src/katalytic/files/__init__.py` & `katalytic-0.3.0/src/katalytic/files/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import csv
+
+
 import errno
 import itertools
 import re
 import shutil
 import tempfile
 import warnings
 
+
 from pathlib import Path
 
 try:
     # use a faster json package by default
     import ujson as json
 except ImportError:  # pragma: no cover -- can't test both branches in the same run
     # fallback to the stdlib version
     import json
 
 from katalytic.data import as_list_of_lists, sort_dict_by_keys, is_none_of
 from katalytic.meta import extract_call_stack_info
+
 # noinspection PyProtectedMember
-from katalytic._pkg import _UNDEFINED, find_functions_marked_with, mark, KatalyticInterrupt
+from katalytic._pkg import (
+    _UNDEFINED,
+    find_functions_marked_with,
+    mark,
+    KatalyticInterrupt,
+)
 
 
-@mark('load::csv')
-def load_csv(path, *, default=_UNDEFINED, encoding='utf-8'):
+@mark("load::csv")
+def load_csv(path, *, default=_UNDEFINED, encoding="utf-8"):
     """
     Load data from a CSV file and return it as a list of dictionaries.
     It will guess the data type of each column based on its values.
 
     Args:
         path (str):
             The path to the CSV file.
@@ -44,43 +53,47 @@
     """
     # Using the wrong extension would return default or raise an error even if the file exists.
     # Trigger the warning before that happens, to provide a hint to the user about the real problem
     _warn_if_another_function_should_be_used(path, _load_funcs)
     if not Path(path).exists() and default is not _UNDEFINED:
         return default
 
-    with open(path, 'r', encoding=encoding) as f:
-        dialect = csv.Sniffer().sniff(f.read(1024))
+    with open(path, "r", encoding=encoding) as f:
+        peek = f.read(1024)
+        if peek.strip() == "":
+            return []
+
+        dialect = csv.Sniffer().sniff(peek)
         f.seek(0)
 
         reader = csv.reader(f, dialect)
         header = next(reader)
         data = [dict(zip(header, row)) for row in reader]
 
     for col in header:
         t = _guess_type(col, data)
 
         for i, row in enumerate(data):
             # The csv reader reads missing values as empty strings.
             # Convert all empty strings to None even though they might
             # be actual empty strings
-            if row[col] in ('None', ''):
+            if row[col] in ("None", ""):
                 data[i][col] = None
 
-        if t == 'bool':
+        if t == "bool":
             for i, row in enumerate(data):
-                if row[col] == 'True':
+                if row[col] == "True":
                     data[i][col] = True
-                elif row[col] == 'False':
+                elif row[col] == "False":
                     data[i][col] = False
-        elif t == 'float':
+        elif t == "float":
             for i, row in enumerate(data):
                 if row[col] is not None:
                     data[i][col] = float(row[col])
-        elif t == 'int':
+        elif t == "int":
             for i, row in enumerate(data):
                 if row[col] is not None:
                     data[i][col] = int(row[col])
 
     return data
 
 
@@ -103,43 +116,43 @@
     is_bool = True
     is_float = False
     is_number = True
 
     for i, row in enumerate(data):
         v = row[col]
         if not (is_number or is_bool):
-            return 'str'
+            return "str"
 
-        if v in ('None', ''):
+        if v in ("None", ""):
             continue
 
-        if v in ('True', 'False'):
+        if v in ("True", "False"):
             is_number = False
             continue
         else:
             is_bool = False
 
-        if not re.search(r'^-?\d+(\.\d+)?$', v):
+        if not re.search(r"^-?\d+(\.\d+)?$", v):
             is_number = False
-        elif '.' in v:
+        elif "." in v:
             is_float = True
 
     if is_bool:
-        return 'bool'
+        return "bool"
     elif is_number:
         if is_float:
-            return 'float'
+            return "float"
         else:
-            return 'int'
+            return "int"
     else:
-        return 'str'
+        return "str"
 
 
-@mark('save::csv')
-def save_csv(data, path, *, encoding='utf-8', exists='replace', make_dirs=True):
+@mark("save::csv")
+def save_csv(data, path, *, encoding="utf-8", exists="replace", make_dirs=True):
     """
     Save data to a CSV file.
 
     Args:
         data (iterable):
             The data to be saved. It can be any of the following formats:
             a dict of lists, a list of lists, a list of dicts
@@ -162,87 +175,94 @@
     Returns:
         None
 
     Raises:
         IOError:
             If there is an error while saving the CSV file.
     """
-    if exists not in ('error', 'replace', 'skip'):
-        raise ValueError(f'<exists> expects "error", "replace", or "skip". Got {exists!r}')
+    if exists not in ("error", "replace", "skip"):
+        raise ValueError(
+            f'<exists> expects "error", "replace", or "skip". Got {exists!r}'
+        )
     elif not isinstance(make_dirs, bool):
-        raise TypeError(f'<make_dirs> expects False, or True. Got {make_dirs!r}')
+        raise TypeError(f"<make_dirs> expects False, or True. Got {make_dirs!r}")
 
     # optimization: trigger the warning only if the parameter preconditions are valid
     _warn_if_another_function_should_be_used(path, _save_funcs)
 
     # optimization: run the checks before starting to save the file, just in case the
     # path exists already when the function is called. This will ensure we don't
     # waste time saving the file only to raise an error or skip it when we do the same checks
     # right at the end of the function
     if Path(path).exists():
-        if exists == 'error':
-            raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
-        elif exists == 'replace':
+        if exists == "error":
+            raise FileExistsError(f"[Errno {errno.EEXIST}] File exists: {str(path)!r}")
+        elif exists == "replace":
             pass  # continue executing
-        elif exists == 'skip':
+        elif exists == "skip":
             return
 
     dest_dir = Path(path).parent
     if make_dirs:
         make_dir(dest_dir, create_parents=True, exists_ok=True)
     elif not dest_dir.exists():
-        raise FileNotFoundError(f'[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}')
+        raise FileNotFoundError(
+            f"[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}"
+        )
     elif not dest_dir.is_dir():
-        raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}')
+        raise NotADirectoryError(
+            f"[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}"
+        )
 
     data = as_list_of_lists(data)
 
     try:
-        tmp_path = f'{path}.part'
-        with open(tmp_path, 'w', newline='', encoding=encoding) as f:
+        tmp_path = f"{path}.part"
+        with open(tmp_path, "w", newline="", encoding=encoding) as f:
             csv.writer(f, quoting=csv.QUOTE_ALL).writerows(data)
 
         # You could move the atomicity code higher in the function, but then
         # you wouldn't be testing the function for the worst case scenario
         if save_csv.__katalytic_test_atomicity_race_condition__:
             save_csv.__katalytic_test_atomicity_race_condition__ = False
 
             # I can't use save_csv([{'race': 'condition'}], path) directly
             # It would replace the tmp_path = f'{path}.part' created above
             # and then move it to the target `path`. This function wouldn't
             # be able to find the tmp_path anymore and will throw an error
             # at the end of the function: `Path(tmp_path).rename(path)`
-            tmp_path_2 = path.replace('.csv', '.2.csv')
-            save_csv([{'race': 'condition'}], tmp_path_2)
+            tmp_path_2 = path.replace(".csv", ".2.csv")
+            save_csv([{"race": "condition"}], tmp_path_2)
             Path(tmp_path_2).rename(path)
 
         # Checking these conditions again to make the function
         # as robust as possible against race conditions
         if Path(path).exists():
-            if exists == 'error':
-                raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
-            elif exists == 'replace':
+            if exists == "error":
+                raise FileExistsError(
+                    f"[Errno {errno.EEXIST}] File exists: {str(path)!r}"
+                )
+            elif exists == "replace":
                 pass  # continue executing
-            elif exists == 'skip':
+            elif exists == "skip":
                 return
 
         if save_csv.__katalytic_test_atomicity_interrupt__:
             save_csv.__katalytic_test_atomicity_interrupt__ = False
-            raise KatalyticInterrupt(f'Testing atomicity ...')
+            raise KatalyticInterrupt(f"Testing atomicity ...")
 
         # The rename is atomic on POSIX systems, but not guaranteed on Windows
         Path(tmp_path).rename(path)
     except BaseException as e:
         if not isinstance(e, KatalyticInterrupt):
             raise
 
 
-
-@mark('load::json')
-def load_json(path, *, default=_UNDEFINED, encoding='utf-8'):
+@mark("load::json")
+def load_json(path, *, default=_UNDEFINED, encoding="utf-8"):
     """
     Load data from a JSON file.
 
     Args:
         path (str):
             The path to the JSON file.
         default (Any):
@@ -269,16 +289,25 @@
     if not Path(path).exists() and default is not _UNDEFINED:
         return default
 
     with open(path, encoding=encoding) as f:
         return json.load(f)
 
 
-@mark('save::json')
-def save_json(data, path, *, encoding='utf-8', exists='replace', indent=4, make_dirs=True, sort_keys=True):
+@mark("save::json")
+def save_json(
+    data,
+    path,
+    *,
+    encoding="utf-8",
+    exists="replace",
+    indent=4,
+    make_dirs=True,
+    sort_keys=True,
+):
     """
     Save data to a JSON file.
 
     Args:
         data (dict or list):
             The data to be saved as JSON. It should be a dictionary or a list.
         path (str):
@@ -315,83 +344,91 @@
         IOError:
             If there is an error while saving the JSON file.
 
     """
     if isinstance(indent, float) and indent.is_integer():
         indent = int(indent)
     elif not isinstance(indent, int):
-        raise TypeError(f'<indent> expects a positive integer. Got {indent!r}')
+        raise TypeError(f"<indent> expects a positive integer. Got {indent!r}")
     elif isinstance(indent, bool):
-        raise TypeError(f'<indent> expects a positive integer. Got {indent!r}')
+        raise TypeError(f"<indent> expects a positive integer. Got {indent!r}")
     elif indent < 0:
-        raise ValueError(f'<indent> expects a positive integer. Got {indent!r}')
-    elif exists not in ('error', 'replace', 'skip'):
-        raise ValueError(f'<exists> expects "error", "replace", or "skip". Got {exists!r}')
+        raise ValueError(f"<indent> expects a positive integer. Got {indent!r}")
+    elif exists not in ("error", "replace", "skip"):
+        raise ValueError(
+            f'<exists> expects "error", "replace", or "skip". Got {exists!r}'
+        )
     elif not isinstance(make_dirs, bool):
-        raise TypeError(f'<make_dirs> expects False, or True. Got {make_dirs!r}')
+        raise TypeError(f"<make_dirs> expects False, or True. Got {make_dirs!r}")
 
     # optimization: trigger the warning only if the preconditions are valid
     _warn_if_another_function_should_be_used(path, _save_funcs)
     if Path(path).exists():
-        if exists == 'error':
-            raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
-        elif exists == 'replace':
+        if exists == "error":
+            raise FileExistsError(f"[Errno {errno.EEXIST}] File exists: {str(path)!r}")
+        elif exists == "replace":
             pass  # continue executing
-        elif exists == 'skip':
+        elif exists == "skip":
             return
 
     dest_dir = Path(path).parent
     if make_dirs:
         make_dir(dest_dir, create_parents=True, exists_ok=True)
     elif not dest_dir.exists():
-        raise FileNotFoundError(f'[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}')
+        raise FileNotFoundError(
+            f"[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}"
+        )
     elif not dest_dir.is_dir():
-        raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}')
+        raise NotADirectoryError(
+            f"[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}"
+        )
 
     try:
-        tmp_path = f'{path}.part'
-        with open(tmp_path, 'w', encoding=encoding) as f:
+        tmp_path = f"{path}.part"
+        with open(tmp_path, "w", encoding=encoding) as f:
             json.dump(data, f, indent=indent, sort_keys=sort_keys)
 
         # You could move the atomicity code higher in the function, but then
         # you wouldn't be testing the function for the worst case scenario
         if save_json.__katalytic_test_atomicity_race_condition__:
             save_json.__katalytic_test_atomicity_race_condition__ = False
 
             # I can't use save_json([{'race': 'condition'}], path) directly
             # It would replace the tmp_path = f'{path}.part' created above
             # and then move it to the target `path`. This function wouldn't
             # be able to find the tmp_path anymore and will throw an error
             # at the end of the function: `Path(tmp_path).rename(path)`
-            tmp_path_2 = path.replace('.json', '.2.json')
-            save_json([{'race': 'condition'}], tmp_path_2)
+            tmp_path_2 = path.replace(".json", ".2.json")
+            save_json([{"race": "condition"}], tmp_path_2)
             Path(tmp_path_2).rename(path)
 
         # Checking these conditions again to make the function
         # as robust as possible against race conditions
         if Path(path).exists():
-            if exists == 'error':
-                raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
-            elif exists == 'replace':
+            if exists == "error":
+                raise FileExistsError(
+                    f"[Errno {errno.EEXIST}] File exists: {str(path)!r}"
+                )
+            elif exists == "replace":
                 pass  # continue executing
-            elif exists == 'skip':
+            elif exists == "skip":
                 return
 
         if save_json.__katalytic_test_atomicity_interrupt__:
             save_json.__katalytic_test_atomicity_interrupt__ = False
-            raise KatalyticInterrupt(f'Testing atomicity ...')
+            raise KatalyticInterrupt(f"Testing atomicity ...")
 
         Path(tmp_path).rename(path)
     except BaseException as e:
         if not isinstance(e, KatalyticInterrupt):
             raise
 
 
-@mark('load::txt')
-def load_text(path, *, default=_UNDEFINED, encoding='utf-8'):
+@mark("load::txt")
+def load_text(path, *, default=_UNDEFINED, encoding="utf-8"):
     """
     Load data from a text file.
 
     Args:
         path (str):
             The path to the text file.
         default (Any):
@@ -416,16 +453,16 @@
     if not Path(path).exists() and default is not _UNDEFINED:
         return default
 
     with open(path, encoding=encoding) as f:
         return f.read()
 
 
-@mark('save::txt')
-def save_text(data, path, *, encoding='utf-8', exists='replace', make_dirs=True):
+@mark("save::txt")
+def save_text(data, path, *, encoding="utf-8", exists="replace", make_dirs=True):
     """
     Save data to a text file.
 
     Args:
         data (str):
             The text content to be saved.
         path (str):
@@ -449,69 +486,77 @@
             The number of characters written to the file.
 
     Raises:
         IOError:
             If there is an error while saving the text file.
 
     """
-    if exists not in ('error', 'replace', 'skip'):
-        raise ValueError(f'<exists> expects "error", "replace", or "skip". Got {exists!r}')
+    if exists not in ("error", "replace", "skip"):
+        raise ValueError(
+            f'<exists> expects "error", "replace", or "skip". Got {exists!r}'
+        )
     elif not isinstance(make_dirs, bool):
-        raise TypeError(f'<make_dirs> expects False, or True. Got {make_dirs!r}')
+        raise TypeError(f"<make_dirs> expects False, or True. Got {make_dirs!r}")
 
     # optimization: trigger the warning only if the preconditions are valid
     _warn_if_another_function_should_be_used(path, _save_funcs)
     if Path(path).exists():
-        if exists == 'error':
-            raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
-        elif exists == 'replace':
+        if exists == "error":
+            raise FileExistsError(f"[Errno {errno.EEXIST}] File exists: {str(path)!r}")
+        elif exists == "replace":
             pass  # continue executing
-        elif exists == 'skip':
+        elif exists == "skip":
             return
 
     dest_dir = Path(path).parent
     try:
         if make_dirs:
             make_dir(dest_dir, create_parents=True, exists_ok=True)
         elif not dest_dir.exists():
-            raise FileNotFoundError(f'[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}')
+            raise FileNotFoundError(
+                f"[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}"
+            )
         elif not dest_dir.is_dir():
-            raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}')
+            raise NotADirectoryError(
+                f"[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}"
+            )
 
-        tmp_path = f'{path}.part'
-        with open(tmp_path, 'w', encoding=encoding) as f:
+        tmp_path = f"{path}.part"
+        with open(tmp_path, "w", encoding=encoding) as f:
             f.write(data)
 
         # You could move the atomicity code higher in the function, but then
         # you wouldn't be testing the function for the worst case scenario
         if save_text.__katalytic_test_atomicity_race_condition__:
             save_text.__katalytic_test_atomicity_race_condition__ = False
 
             # I can't use save_text('race condition', path) directly
             # It would replace the tmp_path = f'{path}.part' created above
             # and then move it to the target `path`. This function wouldn't
             # be able to find the tmp_path anymore and will throw an error
             # at the end of the function: `Path(tmp_path).rename(path)`
-            tmp_path_2 = path.replace('.txt', '.2.txt')
-            save_text('race condition', tmp_path_2)
+            tmp_path_2 = path.replace(".txt", ".2.txt")
+            save_text("race condition", tmp_path_2)
             Path(tmp_path_2).rename(path)
 
         # Checking these conditions again to make the function
         # as robust as possible against race conditions
         if Path(path).exists():
-            if exists == 'error':
-                raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
-            elif exists == 'replace':
+            if exists == "error":
+                raise FileExistsError(
+                    f"[Errno {errno.EEXIST}] File exists: {str(path)!r}"
+                )
+            elif exists == "replace":
                 pass  # continue executing
-            elif exists == 'skip':
+            elif exists == "skip":
                 return
 
         if save_text.__katalytic_test_atomicity_interrupt__:
             save_text.__katalytic_test_atomicity_interrupt__ = False
-            raise KatalyticInterrupt(f'Testing atomicity ...')
+            raise KatalyticInterrupt(f"Testing atomicity ...")
 
         Path(tmp_path).rename(path)
     except BaseException as e:
         if not isinstance(e, KatalyticInterrupt):
             raise
 
 
@@ -536,23 +581,25 @@
         TypeError:
             If <create_missing> is not a boolean value.
         OSError:
             If there is an error while deleting or creating the directory.
 
     """
     if not isinstance(create_missing, bool):
-        raise TypeError(f'<create_missing> expects False or True. Got {type(create_missing)}')
+        raise TypeError(
+            f"<create_missing> expects False or True. Got {type(create_missing)}"
+        )
 
     path = Path(path)
     delete_dir(path, missing_ok=True, non_empty_dir=True)
     if create_missing:
         make_dir(path)
 
 
-def copy_dir(src, dest, *, dir_exists='merge', file_exists='replace', make_dirs=True):
+def copy_dir(src, dest, *, dir_exists="merge", file_exists="replace", make_dirs=True):
     """
     Copy a directory from source to destination, including its contents.
 
     Args:
         src (str or Path):
             The path to the source directory.
         dest (str or Path):
@@ -591,58 +638,84 @@
             If the source or destination path is not a directory.
         FileExistsError:
             If a destination directory already exists when 'dir_exists' is set to 'error'.
         OSError:
             If there is an error while copying or deleting files/directories.
 
     """
-    if dir_exists not in ('error', 'merge', 'replace', 'skip'):
-        raise ValueError(f'<dir_exists> expects "error", "merge", "replace", "skip". Got {dir_exists!r}')
-    elif file_exists not in ('error', 'replace', 'skip'):
-        raise ValueError(f'<file_exists> expects "error", False, or True. Got {file_exists!r}')
+    if dir_exists not in ("error", "merge", "replace", "skip"):
+        raise ValueError(
+            f'<dir_exists> expects "error", "merge", "replace", "skip". Got {dir_exists!r}'
+        )
+    elif file_exists not in ("error", "replace", "skip"):
+        raise ValueError(
+            f'<file_exists> expects "error", False, or True. Got {file_exists!r}'
+        )
     elif not isinstance(make_dirs, bool):
-        raise TypeError(f'<make_dirs> expects False or True. Got {type(make_dirs)}')
+        raise TypeError(f"<make_dirs> expects False or True. Got {type(make_dirs)}")
 
     src = Path(src)
     dest = Path(dest)
 
     if not src.exists():
-        raise FileNotFoundError(f'[Errno {errno.ENOENT}] <src> directory does not exist: {str(src)!r}')
+        raise FileNotFoundError(
+            f"[Errno {errno.ENOENT}] <src> directory does not exist: {str(src)!r}"
+        )
     elif src.is_file():
-        raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Expected a directory, but <src> is a file: {str(src)!r}')
+        raise NotADirectoryError(
+            f"[Errno {errno.ENOTDIR}] Expected a directory, but <src> is a file: {str(src)!r}"
+        )
     elif dest.is_file():
-        raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Expected a directory, but <dest> is a file: {str(dest)!r}')
+        raise NotADirectoryError(
+            f"[Errno {errno.ENOTDIR}] Expected a directory, but <dest> is a file: {str(dest)!r}"
+        )
     elif dest.is_dir():
         if src.samefile(dest):
-            raise ValueError(f'<src> and <dest> are equal: {str(src)!r}')
-        elif dir_exists == 'replace':
+            raise ValueError(f"<src> and <dest> are equal: {str(src)!r}")
+        elif dir_exists == "replace":
             delete_dir(dest, non_empty_dir=True)
-        elif dir_exists == 'skip':
+        elif dir_exists == "skip":
             return
 
         for src_item in src.iterdir():
             dest_item = str(src_item).replace(str(src), str(dest))
             if src_item.is_dir():
-                if Path(dest_item).is_dir() and dir_exists == 'error':
-                    raise FileExistsError(f'[Errno {errno.EEXIST}] Directory already exists: {str(dest_item)!r}')
-
-                copy_dir(src_item, dest_item, make_dirs=make_dirs, file_exists=file_exists, dir_exists=dir_exists)
+                if Path(dest_item).is_dir() and dir_exists == "error":
+                    raise FileExistsError(
+                        f"[Errno {errno.EEXIST}] Directory already exists: {str(dest_item)!r}"
+                    )
+
+                copy_dir(
+                    src_item,
+                    dest_item,
+                    make_dirs=make_dirs,
+                    file_exists=file_exists,
+                    dir_exists=dir_exists,
+                )
             else:
                 copy_file(src_item, dest_item, exists=file_exists)
     elif make_dirs is True:
         if src.name != dest.name:
-            dest = dest/src.name
+            dest = dest / src.name
 
         make_dir(dest)
-        copy_dir(src, dest, make_dirs=make_dirs, file_exists=file_exists, dir_exists=dir_exists)
+        copy_dir(
+            src,
+            dest,
+            make_dirs=make_dirs,
+            file_exists=file_exists,
+            dir_exists=dir_exists,
+        )
     elif make_dirs is False:
-        raise FileNotFoundError(f'[Errno {errno.ENOENT}] No such directory: {str(dest)!r}')
+        raise FileNotFoundError(
+            f"[Errno {errno.ENOENT}] No such directory: {str(dest)!r}"
+        )
 
 
-def copy_file(src, dest, *, exists='replace', make_dirs=True):
+def copy_file(src, dest, *, exists="replace", make_dirs=True):
     """
     Copy a file from source to destination.
 
     Args:
         src (str or Path):
             The path to the source file.
         dest (str or Path):
@@ -673,66 +746,74 @@
             If the source path is a directory.
         FileExistsError:
             If a destination file already exists when 'exists' is set to 'error'.
         OSError:
             If there is an error while copying or deleting the file.
 
     """
-    if exists not in ('error', 'replace', 'skip'):
-        raise ValueError(f'<exists> expects "error", "replace", or "skip". Got {exists!r}')
+    if exists not in ("error", "replace", "skip"):
+        raise ValueError(
+            f'<exists> expects "error", "replace", or "skip". Got {exists!r}'
+        )
     elif not isinstance(make_dirs, bool):
-        raise TypeError(f'<make_dirs> expects False or True. Got {type(make_dirs)}')
+        raise TypeError(f"<make_dirs> expects False or True. Got {type(make_dirs)}")
 
-    ends_with_slash = str(dest).endswith('/')
     src = Path(src)
     dest = Path(dest)
 
     if src.exists() and dest.exists() and src.samefile(dest):
-        raise ValueError(f'<src> and <dest> are equal: {str(src)!r}')
+        raise ValueError(f"<src> and <dest> are equal: {str(src)!r}")
     elif not src.exists():
-        raise FileNotFoundError(f'[Errno {errno.ENOENT}] <src> file does not exist: {str(src)!r}')
+        raise FileNotFoundError(
+            f"[Errno {errno.ENOENT}] <src> file does not exist: {str(src)!r}"
+        )
     elif src.is_dir():
-        raise IsADirectoryError(f'[Errno {errno.EISDIR}] Expected a file, but <src> is a directory: {str(src)!r}')
+        raise IsADirectoryError(
+            f"[Errno {errno.EISDIR}] Expected a file, but <src> is a directory: {str(src)!r}"
+        )
 
     try:
         if dest.exists():
-            if exists == 'error':
-                raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(dest)!r}')
-            elif exists == 'replace':
+            if exists == "error":
+                raise FileExistsError(
+                    f"[Errno {errno.EEXIST}] File exists: {str(dest)!r}"
+                )
+            elif exists == "replace":
                 pass
-            elif exists == 'skip':
+            elif exists == "skip":
                 return
         elif make_dirs:
-            if ends_with_slash:
-                make_dir(dest)
-            else:
-                make_dir(dest.parent)
+            make_dir(dest.parent)
         else:
-            raise FileNotFoundError(f'[Errno {errno.ENOENT}] No such file: {str(dest)!r}')
+            raise FileNotFoundError(
+                f"[Errno {errno.ENOENT}] No such file: {str(dest)!r}"
+            )
 
         # You could move the atomicity code higher in the function, but then
         # you wouldn't be testing the function for the worst case scenario
         if copy_file.__katalytic_test_atomicity_race_condition__:
             copy_file.__katalytic_test_atomicity_race_condition__ = False
 
             # I can't use copy_file([{'race': 'condition'}], path) directly
             # It would replace the tmp_path = f'{path}.part' created above
             # and then move it to the target `path`. This function wouldn't
             # be able to find the tmp_path anymore and will throw an error
             # at the end of the function: `Path(tmp_path).rename(path)`
-            Path(dest).write_text('race condition')
+            Path(dest).write_text("race condition")
 
         # Checking these conditions again to make the function
         # as robust as possible against race conditions
         if Path(dest).exists():
-            if exists == 'error':
-                raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(dest)!r}')
-            elif exists == 'replace':
+            if exists == "error":
+                raise FileExistsError(
+                    f"[Errno {errno.EEXIST}] File exists: {str(dest)!r}"
+                )
+            elif exists == "replace":
                 pass  # continue executing
-            elif exists == 'skip':
+            elif exists == "skip":
                 return
 
         if copy_file.__katalytic_test_atomicity_interrupt__:
             copy_file.__katalytic_test_atomicity_interrupt__ = False
             raise KatalyticInterrupt()
 
         shutil.copy2(src, dest)
@@ -773,36 +854,42 @@
             If the directory doesn't exist and 'missing_ok' is set to False.
         NotADirectoryError:
             If the provided path refers to a file instead of a directory.
         OSError:
             If there is an error while deleting the directory.
 
     """
-    if path is None or path in ('', '.'):
-        raise ValueError(f'path={path!r} would delete the current dir')
+    if path is None or path in ("", "."):
+        raise ValueError(f"path={path!r} would delete the current dir")
     elif not isinstance(missing_ok, bool):
-        raise TypeError(f'<missing_ok> expects False or True. Got {type(missing_ok)}')
-    elif is_none_of(non_empty_dir, ('error', False, True)):
-        raise ValueError(f'<non_empty_dir> expects "error", False, or True. Got {non_empty_dir!r}')
+        raise TypeError(f"<missing_ok> expects False or True. Got {type(missing_ok)}")
+    elif is_none_of(non_empty_dir, ("error", False, True)):
+        raise ValueError(
+            f'<non_empty_dir> expects "error", False, or True. Got {non_empty_dir!r}'
+        )
 
     path = Path(path)
     if path.is_dir():
-        if non_empty_dir == 'error':
+        if non_empty_dir == "error":
             path.rmdir()
         elif non_empty_dir is True:
             shutil.rmtree(path)
         elif non_empty_dir is False and not is_dir_empty(path):
             pass
     elif not path.exists():
         if missing_ok:
             pass
         else:
-            raise FileNotFoundError(f'[Errno {errno.ENOENT}] No such directory: {str(path)!r}')
+            raise FileNotFoundError(
+                f"[Errno {errno.ENOENT}] No such directory: {str(path)!r}"
+            )
     elif path.is_file():
-        raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Expected a directory, but <path> is a file: {str(path)!r}')
+        raise NotADirectoryError(
+            f"[Errno {errno.ENOTDIR}] Expected a directory, but <path> is a file: {str(path)!r}"
+        )
 
 
 def delete_file(path, *, missing_ok=True):
     """
     Delete a file.
 
     Args:
@@ -825,29 +912,33 @@
         IsADirectoryError:
             If the provided path refers to a directory instead of a file.
         OSError:
             If there is an error while deleting the file.
 
     """
     if not isinstance(missing_ok, bool):
-        raise TypeError(f'<missing_ok> expects False or True. Got {type(missing_ok)}')
+        raise TypeError(f"<missing_ok> expects False or True. Got {type(missing_ok)}")
 
     path = Path(path)
     if path.is_file():
         path.unlink()
     elif not path.exists():
         if missing_ok:
             pass
         else:
-            raise FileNotFoundError(f'[Errno {errno.ENOENT}] No such file: {str(path)!r}')
+            raise FileNotFoundError(
+                f"[Errno {errno.ENOENT}] No such file: {str(path)!r}"
+            )
     elif path.is_dir():
-        raise IsADirectoryError(f'[Errno {errno.EISDIR}] Expected a file, but <path> is a directory: {str(path)!r}')
+        raise IsADirectoryError(
+            f"[Errno {errno.EISDIR}] Expected a file, but <path> is a directory: {str(path)!r}"
+        )
 
 
-def get_all(path='.', *, glob=True, iter_=False, prefix=True, recursive=False):
+def get_all(path=".", *, glob=True, iter_=False, prefix=True, recursive=False):
     """
     Retrieve all files and directories at the specified path. If `iter_` is False, they will be sorted
 
     Args:
         path (str or Path, optional):
             The path to retrieve files and directories from. Defaults to the current directory ('.').
         glob (bool, optional):
@@ -863,15 +954,15 @@
         list or iterator:
             A list of files and directories at the specified path, or an iterator if `iter_` is set to True.
 
     """
     return _get_all(path, glob=glob, iter_=iter_, prefix=prefix, recursive=recursive)
 
 
-def get_dirs(path='.', *, glob=True, iter_=False, prefix=True, recursive=False):
+def get_dirs(path=".", *, glob=True, iter_=False, prefix=True, recursive=False):
     """
     Retrieve directories at the specified path. If `iter_` is False, they will be sorted
 
     Args:
         path (str or Path, optional):
             The path to retrieve directories from. Defaults to the current directory ('.').
         glob (bool, optional):
@@ -884,18 +975,20 @@
             Specifies whether to retrieve directories recursively. Defaults to False.
 
     Returns:
         list or iterator:
             A list of directories at the specified path, or an iterator if `iter_` is set to True.
 
     """
-    return _get_all(path, glob=glob, iter_=iter_, prefix=prefix, only_dirs=True, recursive=recursive)
+    return _get_all(
+        path, glob=glob, iter_=iter_, prefix=prefix, only_dirs=True, recursive=recursive
+    )
 
 
-def get_files(path='.', *, glob=True, iter_=False, prefix=True, recursive=False):
+def get_files(path=".", *, glob=True, iter_=False, prefix=True, recursive=False):
     """
     Retrieve files at the specified path. If `iter_` is False, they will be sorted
 
     Args:
         path (str or Path, optional):
             The path to retrieve files from. Defaults to the current directory ('.').
         glob (bool, optional):
@@ -908,18 +1001,34 @@
             Specifies whether to retrieve files recursively. Defaults to False.
 
     Returns:
         list or iterator:
             A list of files at the specified path, or an iterator if `iter_` is set to True.
 
     """
-    return _get_all(path, glob=glob, iter_=iter_, prefix=prefix, only_files=True, recursive=recursive)
-
-
-def _get_all(path='.', *, glob=True, iter_=False, only_dirs=False, only_files=False, prefix=True, recursive=False):
+    return _get_all(
+        path,
+        glob=glob,
+        iter_=iter_,
+        prefix=prefix,
+        only_files=True,
+        recursive=recursive,
+    )
+
+
+def _get_all(
+    path=".",
+    *,
+    glob=True,
+    iter_=False,
+    only_dirs=False,
+    only_files=False,
+    prefix=True,
+    recursive=False,
+):
     """
     Retrieve all files and directories at the specified path. If `iter_` is False, they will be sorted
 
     Args:
         path (str or Path, optional):
             The path to retrieve files and directories from. Defaults to the current directory ('.').
         glob (bool, optional):
@@ -943,66 +1052,76 @@
         TypeError:
             If invalid values are provided for the boolean parameters.
         ValueError:
             If both 'only_dirs' and 'only_files' are set to True.
 
     """
     if not isinstance(glob, bool):
-        raise TypeError(f'<glob> expects False or True. Got {type(glob)}')
+        raise TypeError(f"<glob> expects False or True. Got {type(glob)}")
     elif not isinstance(iter_, bool):
-        raise TypeError(f'<iter_> expects False or True. Got {type(iter_)}')
+        raise TypeError(f"<iter_> expects False or True. Got {type(iter_)}")
     elif not isinstance(only_dirs, bool):
-        raise TypeError(f'<only_dirs> expects False or True. Got {type(only_dirs)}')
+        raise TypeError(f"<only_dirs> expects False or True. Got {type(only_dirs)}")
     elif not isinstance(only_files, bool):
-        raise TypeError(f'<only_files> expects False or True. Got {type(only_files)}')
+        raise TypeError(f"<only_files> expects False or True. Got {type(only_files)}")
     elif not isinstance(prefix, bool):
-        raise TypeError(f'<prefix> expects False or True. Got {type(prefix)}')
+        raise TypeError(f"<prefix> expects False or True. Got {type(prefix)}")
     elif not isinstance(recursive, bool):
-        raise TypeError(f'<recursive> expects False or True. Got {type(recursive)}')
+        raise TypeError(f"<recursive> expects False or True. Got {type(recursive)}")
     elif only_dirs and only_files:
-        raise ValueError('<only_dirs> and <only_files> can\'t be True at the same time')
+        raise ValueError("<only_dirs> and <only_files> can't be True at the same time")
 
     original_type = type(path)
-    if glob and (path is not None and '*' in str(path)):
-        path, _, pattern = str(path).partition('*')
+    if glob and (path is not None and "*" in str(path)):
+        path, _, pattern = str(path).partition("*")
         if recursive:
-            pattern = re.sub(r'^\*/', r'**/', f'*{pattern}')
+            pattern = re.sub(r"^\*/", r"**/", f"*{pattern}")
             result = Path(path).rglob(pattern)
         else:
-            result = Path(path).glob(f'*{pattern}')
+            result = Path(path).glob(f"*{pattern}")
     else:
         result = Path(path).iterdir()
         if recursive:
             result = itertools.chain.from_iterable(
-                [p] if p.is_file()
-                else itertools.chain([p], _get_all(
-                    p, glob=glob, iter_=True, only_dirs=only_dirs,
-                    only_files=only_files, prefix=True, recursive=recursive))
+                [p]
+                if p.is_file()
+                else itertools.chain(
+                    [p],
+                    _get_all(
+                        p,
+                        glob=glob,
+                        iter_=True,
+                        only_dirs=only_dirs,
+                        only_files=only_files,
+                        prefix=True,
+                        recursive=recursive,
+                    ),
+                )
                 for p in result
             )
 
     if only_dirs:
         result = (p for p in result if Path(p).is_dir())
     elif only_files:
         result = (p for p in result if Path(p).is_file())
 
     if prefix:
         result = (str(p) for p in result)
     else:
-        result = (str(p).replace(f'{path}/', '', 1) for p in result)
+        result = (str(p).replace(f"{path}/", "", 1) for p in result)
 
     result = (original_type(p) for p in result)
 
     if iter_:
         return result
     else:
         return sorted(result)
 
 
-def get_unique_path(pattern='{}'):
+def get_unique_path(pattern="{}"):
     """
     Generate a unique path based on the provided pattern.
 
     Args:
         pattern (str or Path, optional):
             The pattern for generating the unique path. Defaults to '{}'.
 
@@ -1013,40 +1132,41 @@
     Raises:
         TypeError:
             If the 'pattern' parameter is not a string or a pathlib.Path object.
         ValueError:
             If the pattern is invalid or does not contain exactly one placeholder.
     """
     if not isinstance(pattern, (str, Path)):
-        raise TypeError(f'<pattern> expects a str or pathlib.Path. Got {type(pattern)}')
+        raise TypeError(f"<pattern> expects a str or pathlib.Path. Got {type(pattern)}")
 
     original_type = type(pattern)
     pattern = str(pattern)
-    placeholders = re.findall(r'{(:((\d*)?d)?)?}', pattern)
+    placeholders = re.findall(r"{(:((\d*)?d)?)?}", pattern)
     if len(placeholders) != 1:
         raise ValueError(
-            f'Invalid pattern: {pattern!r}. You must provide exactly one placeholder, '
-            + 'optionally with an integer format. Try using "{}" or "{:03d}"')
+            f"Invalid pattern: {pattern!r}. You must provide exactly one placeholder, "
+            + 'optionally with an integer format. Try using "{}" or "{:03d}"'
+        )
 
-    if pattern.startswith('./'):
-        pattern = pattern.partition('./')[2]
+    if pattern.startswith("./"):
+        pattern = pattern.partition("./")[2]
 
-    if not pattern.startswith('/'):
+    if not pattern.startswith("/"):
         d = tempfile.mkdtemp()
-        pattern = f'{d}/{pattern}'
+        pattern = f"{d}/{pattern}"
 
     n = 0
     while True:
         n += 1
         path = pattern.format(n)
         if not Path(path).exists():
             return original_type(path)
 
 
-def is_dir_empty(path, *, missing='error'):
+def is_dir_empty(path, *, missing="error"):
     """
     Check if a directory is empty.
 
     Args:
         path (str or Path):
             The path to the directory.
         missing (bool or str, optional):
@@ -1065,32 +1185,36 @@
             If invalid values are provided for the 'missing' parameter.
         NotADirectoryError:
             If the provided path refers to a file instead of a directory.
         FileNotFoundError:
             If the directory doesn't exist and 'missing' is set to 'error'.
 
     """
-    if is_none_of(missing, (False, True, 'error')):
+    if is_none_of(missing, (False, True, "error")):
         raise ValueError(f'<missing> expects "error", False, or True. Got {missing!r}')
 
     path = Path(path)
     if path.is_dir():
         return list(path.iterdir()) == []
     elif path.is_file():
-        raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Expected a directory, but "path" is a file: {str(path)!r}')
+        raise NotADirectoryError(
+            f'[Errno {errno.ENOTDIR}] Expected a directory, but "path" is a file: {str(path)!r}'
+        )
     else:
         if missing is False:
             return False
         elif missing is True:
             return True
-        elif missing == 'error':
-            raise FileNotFoundError(f'[Errno {errno.ENOENT}] No such file or directory: {str(path)!r}')
+        elif missing == "error":
+            raise FileNotFoundError(
+                f"[Errno {errno.ENOENT}] No such file or directory: {str(path)!r}"
+            )
 
 
-def is_file_empty(path, *, missing='error'):
+def is_file_empty(path, *, missing="error"):
     """
     Check if a file is empty.
 
     Args:
         path (str or Path):
             The path to the file.
         missing (bool or str, optional):
@@ -1109,29 +1233,33 @@
             If invalid values are provided for the 'missing' parameter.
         IsADirectoryError:
             If the provided path refers to a directory instead of a file.
         FileNotFoundError:
             If the file doesn't exist and 'missing' is set to 'error'.
 
     """
-    if is_none_of(missing, (False, True, 'error')):
+    if is_none_of(missing, (False, True, "error")):
         raise ValueError(f'<missing> expects "error", False, or True. Got {missing!r}')
 
     path = Path(path)
     if path.is_file():
         return path.stat().st_size == 0
     elif path.is_dir():
-        raise IsADirectoryError(f'[Errno {errno.EISDIR}] Expected a file, but <path> is a directory: {str(path)!r}')
+        raise IsADirectoryError(
+            f"[Errno {errno.EISDIR}] Expected a file, but <path> is a directory: {str(path)!r}"
+        )
     else:
         if missing is False:
             return False
         elif missing is True:
             return True
-        elif missing == 'error':
-            raise FileNotFoundError(f'[Errno {errno.ENOENT}] No such file or directory: {str(path)!r}')
+        elif missing == "error":
+            raise FileNotFoundError(
+                f"[Errno {errno.ENOENT}] No such file or directory: {str(path)!r}"
+            )
 
 
 def make_dir(path, *, create_parents=True, exists_ok=True):
     """
     Create a directory at the specified path.
 
     Args:
@@ -1154,26 +1282,30 @@
         FileExistsError:
             If the directory already exists and 'exists_ok' is set to False.
         OSError:
             If there is an error while creating the directory.
 
     """
     if not isinstance(create_parents, bool):
-        raise TypeError(f'<create_parents> expects False or True. Got {type(create_parents)}')
+        raise TypeError(
+            f"<create_parents> expects False or True. Got {type(create_parents)}"
+        )
     elif not isinstance(exists_ok, bool):
-        raise TypeError(f'<exists_ok> expects False or True. Got {type(exists_ok)}')
+        raise TypeError(f"<exists_ok> expects False or True. Got {type(exists_ok)}")
 
     path = Path(path)
     if path.is_file():
-        raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Expected a directory, but "path" is a file: {str(path)!r}')
+        raise NotADirectoryError(
+            f'[Errno {errno.ENOTDIR}] Expected a directory, but "path" is a file: {str(path)!r}'
+        )
 
     path.mkdir(parents=create_parents, exist_ok=exists_ok)
 
 
-def move_dir(src, dest, *, dir_exists='merge', file_exists='replace', make_dirs=True):
+def move_dir(src, dest, *, dir_exists="merge", file_exists="replace", make_dirs=True):
     """
     Move a directory from source to destination.
 
     Args:
         src (str or Path):
             The path to the source directory.
         dest (str or Path):
@@ -1198,22 +1330,24 @@
             - True: Create the directory if it doesn't exist.
             - False: Raise an error if the destination directory doesn't exist.
 
     Returns:
         None
 
     """
-    if dir_exists == 'skip' and Path(dest).exists():
+    if dir_exists == "skip" and Path(dest).exists():
         return
 
-    copy_dir(src, dest, dir_exists=dir_exists, file_exists=file_exists, make_dirs=make_dirs)
+    copy_dir(
+        src, dest, dir_exists=dir_exists, file_exists=file_exists, make_dirs=make_dirs
+    )
     delete_dir(src, non_empty_dir=True)
 
 
-def move_file(src, dest, *, exists='replace', make_dirs=True):
+def move_file(src, dest, *, exists="replace", make_dirs=True):
     """
     Move a file from source to destination.
 
     Args:
         src (str or Path):
             The path to the source file.
         dest (str or Path):
@@ -1230,35 +1364,98 @@
             - True: Create the directory if it doesn't exist.
             - False: Raise an error if the destination directory doesn't exist.
 
     Returns:
         None
 
     """
-    if exists == 'skip' and Path(dest).exists():
-        return
+    if exists not in ("error", "replace", "skip"):
+        raise ValueError(
+            f'<exists> expects "error", "replace", or "skip". Got {exists!r}'
+        )
+    elif not isinstance(make_dirs, bool):
+        raise TypeError(f"<make_dirs> expects False or True. Got {type(make_dirs)}")
 
-    copy_file(src, dest, exists=exists, make_dirs=make_dirs)
-    delete_file(src)
+    src = Path(src)
+    dest = Path(dest)
+
+    if not src.exists():
+        raise FileNotFoundError(
+            f"[Errno {errno.ENOENT}] <src> file does not exist: {str(src)!r}"
+        )
+    elif src.is_dir():
+        raise IsADirectoryError(
+            f"[Errno {errno.EISDIR}] Expected a file, but <src> is a directory: {str(src)!r}"
+        )
+
+    try:
+        if dest.exists():
+            if exists == "error":
+                raise FileExistsError(
+                    f"[Errno {errno.EEXIST}] File exists: {str(dest)!r}"
+                )
+            elif exists == "replace":
+                pass
+            elif exists == "skip":
+                return
+        elif make_dirs:
+            make_dir(dest.parent)
+        else:
+            raise FileNotFoundError(
+                f"[Errno {errno.ENOENT}] No such file: {str(dest)!r}"
+            )
+
+        # You could move the atomicity code higher in the function, but then
+        # you wouldn't be testing the function for the worst case scenario
+        if move_file.__katalytic_test_atomicity_race_condition__:
+            move_file.__katalytic_test_atomicity_race_condition__ = False
+
+            # I can't use move_file([{'race': 'condition'}], path) directly
+            # It would replace the tmp_path = f'{path}.part' created above
+            # and then move it to the target `path`. This function wouldn't
+            # be able to find the tmp_path anymore and will throw an error
+            # at the end of the function: `Path(tmp_path).rename(path)`
+            Path(dest).write_text("race condition")
+
+        # Checking these conditions again to make the function
+        # as robust as possible against race conditions
+        if Path(dest).exists():
+            if exists == "error":
+                raise FileExistsError(
+                    f"[Errno {errno.EEXIST}] File exists: {str(dest)!r}"
+                )
+            elif exists == "replace":
+                pass  # continue executing
+            elif exists == "skip":
+                return
+
+        if move_file.__katalytic_test_atomicity_interrupt__:
+            move_file.__katalytic_test_atomicity_interrupt__ = False
+            raise KatalyticInterrupt()
+
+        shutil.move(str(src), str(dest))
+    except BaseException as e:
+        if not isinstance(e, KatalyticInterrupt):
+            raise
 
 
 def _find_grouped_functions(group):
     loaders = {}
     for func_name, f, groups in find_functions_marked_with(group):
         for g in groups:
-            ext = g.rpartition('::')[2]
+            ext = g.rpartition("::")[2]
             loaders[ext] = f
 
     # sort the dict with the most specific extension at the beginning
     # this makes it easier to pick ".tar.gz" over ".gz"
     return sort_dict_by_keys(loaders, condition=len, reverse=True)
 
 
-_load_funcs = _find_grouped_functions('load::*')
-_save_funcs = _find_grouped_functions('save::*')
+_load_funcs = _find_grouped_functions("load::*")
+_save_funcs = _find_grouped_functions("save::*")
 
 
 def load(path, default=_UNDEFINED, **kwargs):
     """
     Load data from a file based on the file extension.
 
     Args:
@@ -1275,21 +1472,21 @@
 
     Raises:
         RuntimeError:
             If no load function is found for the given file extension.
 
     """
     for ext, f in _load_funcs.items():
-        if path.lower().endswith(f'.{ext}'):
+        if path.lower().endswith(f".{ext}"):
             return f(path, default=default, **kwargs)
 
-    raise RuntimeError(f'No load function found for {path!r}')
+    return load_text(path, default=default, **kwargs)
 
 
-def save(data, path, *, exists='replace', make_dirs=True, **kwargs):
+def save(data, path, *, exists="replace", make_dirs=True, **kwargs):
     """
     Save data to a file based on the file extension.
 
     Args:
         data (any):
             The data to be saved.
         path (str):
@@ -1313,38 +1510,42 @@
 
     Raises:
         RuntimeError:
             If no save function is found for the given file extension.
 
     """
     for ext, f in _save_funcs.items():
-        if path.lower().endswith(f'.{ext}'):
+        if path.lower().endswith(f".{ext}"):
             f(data, path, exists=exists, make_dirs=make_dirs, **kwargs)
             return
 
-    raise RuntimeError(f'No save function found for {path!r}')
+    save_text(data, path, exists=exists, make_dirs=make_dirs, **kwargs)
 
 
 def _warn_if_another_function_should_be_used(path, group_dict):
     path = path.lower()
     for ext, f in group_dict.items():
-        if path.endswith(f'.{ext}'):
+        if path.endswith(f".{ext}"):
             file, caller, line = extract_call_stack_info(depth=1)
             if group_dict[ext] != caller:
                 warnings.warn(
                     f'Use "{group_dict[ext].__name__}" for ".{ext}" files instead of "{caller.__name__}".'
-                    f'\n(called from {file}:{line})'
+                    f"\n(called from {file}:{line})"
                 )
             break
 
 
 copy_dir.__katalytic_test_atomicity_interrupt__ = False
 copy_file.__katalytic_test_atomicity_interrupt__ = False
+move_dir.__katalytic_test_atomicity_interrupt__ = False
+move_file.__katalytic_test_atomicity_interrupt__ = False
 save_csv.__katalytic_test_atomicity_interrupt__ = False
 save_json.__katalytic_test_atomicity_interrupt__ = False
 save_text.__katalytic_test_atomicity_interrupt__ = False
 
 copy_dir.__katalytic_test_atomicity_race_condition__ = False
 copy_file.__katalytic_test_atomicity_race_condition__ = False
+move_dir.__katalytic_test_atomicity_race_condition__ = False
+move_file.__katalytic_test_atomicity_race_condition__ = False
 save_csv.__katalytic_test_atomicity_race_condition__ = False
 save_json.__katalytic_test_atomicity_race_condition__ = False
 save_text.__katalytic_test_atomicity_race_condition__ = False
```

### Comparing `katalytic-0.2.2/src/katalytic/maths/__init__.py` & `katalytic-0.3.0/src/katalytic/maths/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import math
 
+
 from katalytic.data.checks import is_number, is_sequence, is_iterable, is_iterator
 
 _UNDEFINED = object()
 
 
 def L1(a, b):
     """
@@ -22,30 +23,34 @@
             - If a and b are sequences and
                 - the sequences are empty.
                 - the sequences have different lengths.
                 - the sequences are nested (contains sub-sequences).
 
     """
     if isinstance(a, bool):
-        raise ValueError(f'Got <a> = {a!r}')
+        raise ValueError(f"Got <a> = {a!r}")
     elif isinstance(b, bool):
-        raise ValueError(f'Got <b> = {b!r}')
+        raise ValueError(f"Got <b> = {b!r}")
     elif isinstance(a, (int, float)) and isinstance(b, (int, float)):
         return abs(a - b)
     elif is_sequence(a) and is_sequence(b):
         if len(a) == 0 and len(b) == 0:
-            raise ValueError(f'Both sequences are empty')
+            raise ValueError(f"Both sequences are empty")
         elif len(a) != len(b):
-            raise ValueError(f'The sequences have different lengths: {len(a)} and {len(b)}')
+            raise ValueError(
+                f"The sequences have different lengths: {len(a)} and {len(b)}"
+            )
         elif is_sequence(a[0]) or is_sequence(b[0]):
-            raise ValueError(f'Nested sequences are not supported')
+            raise ValueError(f"Nested sequences are not supported")
         else:
             return sum(L1(ai, bi) for ai, bi in zip(a, b))
     else:
-        raise ValueError(f'Unknown format: ({type(a).__name__}) {a!r} and ({type(b).__name__}) {b!r}')
+        raise ValueError(
+            f"Unknown format: ({type(a).__name__}) {a!r} and ({type(b).__name__}) {b!r}"
+        )
 
 
 def L2(a, b):
     """
     Compute the L2 (Euclidean) distance between two values or sequences.
 
     Parameters:
@@ -61,34 +66,43 @@
             - If a and b are sequences and
                 - the sequences are empty.
                 - the sequences have different lengths.
                 - the sequences are nested (contains sub-sequences).
 
     """
     if isinstance(a, bool):
-        raise ValueError(f'Got <a> = {a!r}')
+        raise ValueError(f"Got <a> = {a!r}")
     elif isinstance(b, bool):
-        raise ValueError(f'Got <b> = {b!r}')
+        raise ValueError(f"Got <b> = {b!r}")
     elif isinstance(a, (int, float)) and isinstance(b, (int, float)):
-        return math.sqrt((a - b)**2)
+        return math.sqrt((a - b) ** 2)
     elif is_sequence(a) and is_sequence(b):
         if len(a) == 0 and len(b) == 0:
-            raise ValueError(f'Both sequences are empty')
+            raise ValueError(f"Both sequences are empty")
         elif len(a) != len(b):
-            raise ValueError(f'The sequences have different lengths: {len(a)} and {len(b)}')
+            raise ValueError(
+                f"The sequences have different lengths: {len(a)} and {len(b)}"
+            )
         elif is_sequence(a[0]) or is_sequence(b[0]):
-            raise ValueError(f'Nested sequences are not supported')
+            raise ValueError(f"Nested sequences are not supported")
         elif any(isinstance(ai, bool) or isinstance(bi, bool) for ai, bi in zip(a, b)):
-            raise ValueError(f'Got a boolean value in one of the sequences')
-        elif all(isinstance(ai, (int, float)) and isinstance(bi, (int, float)) for ai, bi in zip(a, b)):
-            return math.sqrt(sum((ai - bi)**2 for ai, bi in zip(a, b)))
+            raise ValueError(f"Got a boolean value in one of the sequences")
+        elif all(
+            isinstance(ai, (int, float)) and isinstance(bi, (int, float))
+            for ai, bi in zip(a, b)
+        ):
+            return math.sqrt(sum((ai - bi) ** 2 for ai, bi in zip(a, b)))
         else:
-            raise ValueError(f'Unknown format: ({type(a).__name__}) {a!r} and ({type(b).__name__}) {b!r}')
+            raise ValueError(
+                f"Unknown format: ({type(a).__name__}) {a!r} and ({type(b).__name__}) {b!r}"
+            )
     else:
-        raise ValueError(f'Unknown format: ({type(a).__name__}) {a!r} and ({type(b).__name__}) {b!r}')
+        raise ValueError(
+            f"Unknown format: ({type(a).__name__}) {a!r} and ({type(b).__name__}) {b!r}"
+        )
 
 
 def min_max(iterable, *, default=_UNDEFINED, key=None):
     """
     Find the minimum and maximum values from the given iterable.
 
     Parameters:
@@ -103,36 +117,38 @@
 
     Raises:
         TypeError: If the iterable is not iterable or if the key is not None or callable.
         ValueError: If the iterable is empty and no default value is provided.
 
     """
     if not is_iterable(iterable):
-        raise TypeError(f'<iterable> expected an iterable, got {type(iterable).__name__}')
+        raise TypeError(
+            f"<iterable> expected an iterable, got {type(iterable).__name__}"
+        )
     elif not (key is None or callable(key)):
-        raise TypeError(f'<key> expected a callable, got {type(key).__name__}')
+        raise TypeError(f"<key> expected a callable, got {type(key).__name__}")
 
     if key is None:
         key = lambda x: x
 
     if is_iterator(iterable):
         iterable = list(iterable)
 
     if len(iterable) == 0:
         if default is _UNDEFINED:
-            raise ValueError(f'Cannot get the min/max of an empty iterable')
+            raise ValueError(f"Cannot get the min/max of an empty iterable")
         else:
             return default
 
     min_ = min(iterable, key=key)
     max_ = max(iterable, key=key)
     return (min_, max_)
 
 
-def clip(x, min_=float('-inf'), max_=float('+inf')):
+def clip(x, min_=float("-inf"), max_=float("+inf")):
     """
     Clip the value x within the specified minimum and maximum bounds.
 
     Parameters:
         x: The value to be clipped.
         min_ (optional): The minimum bound. If not provided, negative infinity is used.
         max_ (optional): The maximum bound. If not provided, positive infinity is used.
@@ -140,14 +156,14 @@
     Returns:
         The clipped value of x, which is guaranteed to be within the specified bounds.
 
     Raises:
         TypeError: If x, min_, or max_ is not a number.
     """
     if not is_number(x):
-        raise TypeError(f'<x> expected a number, got {type(x).__name__}')
+        raise TypeError(f"<x> expected a number, got {type(x).__name__}")
     elif not is_number(min_):
-        raise TypeError(f'<min_> expected a number, got {type(min_).__name__}')
+        raise TypeError(f"<min_> expected a number, got {type(min_).__name__}")
     elif not is_number(max_):
-        raise TypeError(f'<max_> expected a number, got {type(max_).__name__}')
+        raise TypeError(f"<max_> expected a number, got {type(max_).__name__}")
 
     return min(max(x, min_), max_)
```

### Comparing `katalytic-0.2.2/src/katalytic/maths/bboxes.py` & `katalytic-0.3.0/src/katalytic/maths/bboxes.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         bbox (sequence): The bounding box whose area is to be calculated. It should be in the format specified by 'fmt'.
         fmt (str): The format of the bounding box. It could be one of the formats defined in `_FORMATS`.
 
     Returns:
         float: The area of the bounding box.
 
     """
-    bbox = convert_bbox(bbox, fmt, 'xy_wh') if fmt != 'xy_wh' else bbox
+    bbox = convert_bbox(bbox, fmt, "xy_wh") if fmt != "xy_wh" else bbox
     (_, _), (w, h) = bbox
     return w * h
 
 
 def calc_bbox_center(bbox, fmt, *, as_int=False):
     """
     Calculate the center of a bounding box.
@@ -31,15 +31,15 @@
         as_int (bool, optional): If True, the center coordinates are returned as integers. Defaults to False.
 
     Returns:
         tuple:
             The center of the bounding box as a tuple of two coordinates (x, y).
             If 'as_int' is True, the coordinates are integers, otherwise they are floats.
     """
-    (x, y), (X, Y) = convert_bbox(bbox, fmt, 'xy_XY')
+    (x, y), (X, Y) = convert_bbox(bbox, fmt, "xy_XY")
     cx, cy = (mean([x, X]), mean([y, Y]))
 
     if as_int:
         return (int(cx), int(cy))
     else:
         return (cx, cy)
 
@@ -75,16 +75,15 @@
         bbox_2 (sequence): The second bounding box, defined in the format specified by `fmt_2`.
         fmt_2 (str): The format of the second bounding box. This defines how the coordinates in `bbox_2` are interpreted.
 
     Returns:
         float: The largest IoB value between `bbox_1` and `bbox_2`.
     """
     return max(
-        calc_IoB(bbox_1, fmt_1, bbox_2, fmt_2),
-        calc_IoB(bbox_2, fmt_2, bbox_1, fmt_1)
+        calc_IoB(bbox_1, fmt_1, bbox_2, fmt_2), calc_IoB(bbox_2, fmt_2, bbox_1, fmt_1)
     )
 
 
 def calc_IoB_min(bbox_1, fmt_1, bbox_2, fmt_2):
     """
     Return the smallest of (Intersection over bbox_1) and (Intersection over bbox_2).
 
@@ -94,16 +93,15 @@
         bbox_2 (sequence): The second bounding box, defined in the format specified by `fmt_2`.
         fmt_2 (str): The format of the second bounding box. This defines how the coordinates in `bbox_2` are interpreted.
 
     Returns:
         float: The smallest IoB (Intersection over Bounding-box) value between `bbox_1` and `bbox_2`.
     """
     return min(
-        calc_IoB(bbox_1, fmt_1, bbox_2, fmt_2),
-        calc_IoB(bbox_2, fmt_2, bbox_1, fmt_1)
+        calc_IoB(bbox_1, fmt_1, bbox_2, fmt_2), calc_IoB(bbox_2, fmt_2, bbox_1, fmt_1)
     )
 
 
 def calc_IoU(bbox_1, fmt_1, bbox_2, fmt_2):
     """
     Calculate the Intersection over Union (IoU) between two bounding boxes, defined as the area of their intersection divided by the area of their union
 
@@ -143,37 +141,38 @@
         ValueError: If the format doesn't contain scores, and no `scores` argument is provided.
 
     Returns:
         list: The list of remaining bounding boxes after non-maximum suppression has been applied.
     """
     if not bboxes:
         return bboxes
-    elif not format.endswith('s'):
+    elif not format.endswith("s"):
         if scores:
-            bboxes = set_bbox_scores(bboxes, scores, format, 'xyXYs')
+            bboxes = set_bbox_scores(bboxes, scores, format, "xyXYs")
         else:
             raise ValueError(
-                'If the format doesn\'t contain scores, either change the call '
-                'to non_max_suppression(..., scores=...) or use set_bbox_scores().')
+                "If the format doesn't contain scores, either change the call "
+                "to non_max_suppression(..., scores=...) or use set_bbox_scores()."
+            )
 
-    if format.endswith('s') and format != 'xyXYs':
+    if format.endswith("s") and format != "xyXYs":
         # standardise the format to simplify the implementation
-        bboxes = [convert_bbox(bbox, format, 'xyXYs') for bbox in bboxes]
+        bboxes = [convert_bbox(bbox, format, "xyXYs") for bbox in bboxes]
 
     kept, bboxes = pop_max(bboxes, condition=lambda bbox: bbox[-1])
 
     # remove bboxes with IoU > max_IoU than the kept bbox
-    bboxes = [b for b in bboxes if calc_IoU(b, 'xyXYs', kept, 'xyXYs') < max_IoU]
+    bboxes = [b for b in bboxes if calc_IoU(b, "xyXYs", kept, "xyXYs") < max_IoU]
 
     # call recursively on the remaining bboxes
-    kept = [kept, *non_max_suppression(bboxes, 'xyXYs', max_IoU=max_IoU)]
+    kept = [kept, *non_max_suppression(bboxes, "xyXYs", max_IoU=max_IoU)]
 
-    if format != 'xyXYs':
+    if format != "xyXYs":
         # convert to the original format
-        kept = [convert_bbox(bbox, 'xyXYs', format) for bbox in kept]
+        kept = [convert_bbox(bbox, "xyXYs", format) for bbox in kept]
 
     return kept
 
 
 def set_bbox_scores(bboxes, scores, before, after):
     """
     Insert or change the existing scores of a list of bounding boxes.
@@ -187,28 +186,30 @@
     Raises:
         ValueError: If `bboxes` and `scores` don't have the same length, if the `after` format doesn't end with 's', or if any score is not within the range [0, 1].
 
     Returns:
         list: The list of bounding boxes with scores set, in the specified `after` format.
     """
     if len(bboxes) != len(scores):
-        raise ValueError('bboxes and scores must have the same length')
-    elif not after.endswith('s'):
-        raise ValueError('after format must be one of xyXYs, xyXY_s, xy_XY_s, xywhs, xywh_s, xy_wh_s')
+        raise ValueError("bboxes and scores must have the same length")
+    elif not after.endswith("s"):
+        raise ValueError(
+            "after format must be one of xyXYs, xyXY_s, xy_XY_s, xywhs, xywh_s, xy_wh_s"
+        )
     elif not all(0 <= s <= 1 for s in scores):
-        raise ValueError('scores must be in the range [0, 1]')
+        raise ValueError("scores must be in the range [0, 1]")
 
-    if before != 'xyXY':
-        bboxes = [convert_bbox(bbox, before, 'xyXY') for bbox in bboxes]
+    if before != "xyXY":
+        bboxes = [convert_bbox(bbox, before, "xyXY") for bbox in bboxes]
 
     bboxes = [(*bbox, s) for bbox, s in zip(bboxes, scores)]
-    if after == 'xyXYs':
+    if after == "xyXYs":
         return bboxes
     else:
-        return [convert_bbox(bbox, 'xyXYs', after) for bbox in bboxes]
+        return [convert_bbox(bbox, "xyXYs", after) for bbox in bboxes]
 
 
 def convert_bbox(bbox, before, after):
     """
     Convert a bounding box from one format to another.
 
     Args:
@@ -219,56 +220,76 @@
     Raises:
         ValueError: If `before` or `after` are not recognized formats, if `bbox` is not in the `before` format, if `before` and `after` are the same, or if attempting to convert to a format that includes scores from a format that does not.
 
     Returns:
         sequence: The bounding box, converted to the `after` format.
     """
     if before not in _FORMATS:
-        raise ValueError(f'Unknown before format {before!r}')
+        raise ValueError(f"Unknown before format {before!r}")
     elif after not in _FORMATS:
-        raise ValueError(f'Unknown after format {after!r}')
+        raise ValueError(f"Unknown after format {after!r}")
     elif not is_bbox(bbox, before):
-        raise ValueError(f'{bbox!r} is not in the {before!r} format')
+        raise ValueError(f"{bbox!r} is not in the {before!r} format")
     elif before == after:
         # I could just return the bbox, but I prefer to fail early
         # so the dev knows there might be a bug in his code
         # It makes the easy thing harder and the hard thing (debugging) easy
-        raise ValueError(f'before and after formats are the same: {before!r}')
-    elif after.endswith('s') and not before.endswith('s'):
-        raise ValueError(f'Cannot convert from {before} to {after}')
+        raise ValueError(f"before and after formats are the same: {before!r}")
+    elif after.endswith("s") and not before.endswith("s"):
+        raise ValueError(f"Cannot convert from {before} to {after}")
 
     x = y = X = Y = w = h = s = None
-    if before == 'xywh':      x,y,w,h = bbox
-    elif before == 'xywhs':   x,y,w,h,s = bbox
-    elif before == 'xywh_s':  (x,y,w,h), s = bbox
-    elif before == 'xy_wh':   (x,y), (w,h) = bbox
-    elif before == 'xy_wh_s': (x,y), (w,h), s = bbox
-    elif before == 'xyXY':    x,y,X,Y = bbox
-    elif before == 'xyXYs':   x,y,X,Y,s = bbox
-    elif before == 'xyXY_s':  (x,y,X,Y), s = bbox
-    elif before == 'xy_XY':   (x,y), (X,Y) = bbox
-    elif before == 'xy_XY_s': (x,y), (X,Y), s = bbox
+    if before == "xywh":
+        x, y, w, h = bbox
+    elif before == "xywhs":
+        x, y, w, h, s = bbox
+    elif before == "xywh_s":
+        (x, y, w, h), s = bbox
+    elif before == "xy_wh":
+        (x, y), (w, h) = bbox
+    elif before == "xy_wh_s":
+        (x, y), (w, h), s = bbox
+    elif before == "xyXY":
+        x, y, X, Y = bbox
+    elif before == "xyXYs":
+        x, y, X, Y, s = bbox
+    elif before == "xyXY_s":
+        (x, y, X, Y), s = bbox
+    elif before == "xy_XY":
+        (x, y), (X, Y) = bbox
+    elif before == "xy_XY_s":
+        (x, y), (X, Y), s = bbox
 
     if X is None:
         X = x + w
         Y = y + h
     elif w is None:
         w = X - x
         h = Y - y
 
-    if after == 'xywh':      return x,y,w,h
-    elif after == 'xywhs':   return x,y,w,h,s
-    elif after == 'xywh_s':  return (x,y,w,h), s
-    elif after == 'xy_wh':   return (x,y), (w,h)
-    elif after == 'xy_wh_s': return (x,y), (w,h), s
-    elif after == 'xyXY':    return x,y,X,Y
-    elif after == 'xyXYs':   return x,y,X,Y,s
-    elif after == 'xyXY_s':  return (x,y,X,Y), s
-    elif after == 'xy_XY':   return (x,y), (X,Y)
-    elif after == 'xy_XY_s': return (x,y), (X,Y), s
+    if after == "xywh":
+        return x, y, w, h
+    elif after == "xywhs":
+        return x, y, w, h, s
+    elif after == "xywh_s":
+        return (x, y, w, h), s
+    elif after == "xy_wh":
+        return (x, y), (w, h)
+    elif after == "xy_wh_s":
+        return (x, y), (w, h), s
+    elif after == "xyXY":
+        return x, y, X, Y
+    elif after == "xyXYs":
+        return x, y, X, Y, s
+    elif after == "xyXY_s":
+        return (x, y, X, Y), s
+    elif after == "xy_XY":
+        return (x, y), (X, Y)
+    elif after == "xy_XY_s":
+        return (x, y), (X, Y), s
 
 
 def intersect_bboxes(bbox_1, fmt_1, bbox_2, fmt_2):
     """
     Calculate the intersection of two bounding boxes.
 
     Args:
@@ -276,33 +297,33 @@
         fmt_1 (str): The format of the first bounding box.
         bbox_2 (sequence): The second bounding box.
         fmt_2 (str): The format of the second bounding box.
 
     Returns:
         list or None: The intersection of the two bounding boxes in the format of `fmt_1`, or `None` if the bounding boxes do not intersect.
     """
-    if fmt_1.endswith('s'):
+    if fmt_1.endswith("s"):
         s = bbox_1[-1]
 
-    bbox_1 = convert_bbox(bbox_1, fmt_1, 'xy_XY') if fmt_1 != 'xy_XY' else bbox_1
-    bbox_2 = convert_bbox(bbox_2, fmt_2, 'xy_XY') if fmt_2 != 'xy_XY' else bbox_2
+    bbox_1 = convert_bbox(bbox_1, fmt_1, "xy_XY") if fmt_1 != "xy_XY" else bbox_1
+    bbox_2 = convert_bbox(bbox_2, fmt_2, "xy_XY") if fmt_2 != "xy_XY" else bbox_2
 
     (x1, y1), (X1, Y1) = bbox_1
     (x2, y2), (X2, Y2) = bbox_2
 
     x3, y3 = max(x1, x2), max(y1, y2)
     X3, Y3 = min(X1, X2), min(Y1, Y2)
 
     if (0 <= x3 < X3) and (0 <= y3 < Y3):
         bbox_3 = [(x3, y3), (X3, Y3)]
-        if fmt_1.endswith('s'):
+        if fmt_1.endswith("s"):
             # noinspection PyUnboundLocalVariable
-            bbox_3 = convert_bbox([*bbox_3, s], 'xy_XY_s', fmt_1)
-        elif fmt_1 != 'xy_XY':
-            bbox_3 = convert_bbox(bbox_3, 'xy_XY', fmt_1)
+            bbox_3 = convert_bbox([*bbox_3, s], "xy_XY_s", fmt_1)
+        elif fmt_1 != "xy_XY":
+            bbox_3 = convert_bbox(bbox_3, "xy_XY", fmt_1)
 
         return type(bbox_1)(bbox_3)
     else:
         return None
 
 
 def is_bbox(bbox, fmt):
@@ -317,336 +338,336 @@
         bool: `True` if the bounding box is of the specified format, `False` otherwise.
 
     Raises:
         ValueError: If the specified format is not recognized.
     """
     if fmt not in _FORMATS:
         available = ", ".join(_FORMATS)
-        raise ValueError(f'Unknown format {fmt!r}. Available formats: {available}')
+        raise ValueError(f"Unknown format {fmt!r}. Available formats: {available}")
 
     return _FORMATS[fmt](bbox)
 
 
 def _is_xy_wh(bbox):
     """WARNING:
     Returns True if the bbox has the xy_XY format
     There's no way to check against that case
 
     Kept hidden to avoid cluttering the namespace
     """
     if not is_sequence(bbox):
-        raise TypeError(f'Expected a sequence, got {type(bbox)}')
+        raise TypeError(f"Expected a sequence, got {type(bbox)}")
 
     try:
         (x, y), (w, h) = bbox
         return (x >= 0) and (y >= 0) and (w > 0) and (h > 0)
     except ValueError as e:
-        if str(e).startswith('not enough values to unpack'):
+        if str(e).startswith("not enough values to unpack"):
             return False
-        elif str(e).startswith('too many values to unpack'):
+        elif str(e).startswith("too many values to unpack"):
             return False
         else:
             raise
     except TypeError as e:
-        if str(e).startswith('cannot unpack non-iterable'):
+        if str(e).startswith("cannot unpack non-iterable"):
             return False
         elif "not supported between instances of" in str(e):
             return False
-        elif 'object is not iterable' in str(e):
+        elif "object is not iterable" in str(e):
             return False
         else:
             raise
 
 
 def _is_xy_wh_s(bbox):
     """WARNING:
     Returns True if the bbox has the xy_XY format
     There's no way to check against that case
 
     Kept hidden to avoid cluttering the namespace
     """
     if not is_sequence(bbox):
-        raise TypeError(f'Expected a sequence, got {type(bbox)}')
+        raise TypeError(f"Expected a sequence, got {type(bbox)}")
 
     try:
         (x, y), (w, h), s = bbox
         return (x >= 0) and (y >= 0) and (w > 0) and (h > 0) and 0 <= s <= 1
     except ValueError as e:
-        if str(e).startswith('not enough values to unpack'):
+        if str(e).startswith("not enough values to unpack"):
             return False
-        elif str(e).startswith('too many values to unpack'):
+        elif str(e).startswith("too many values to unpack"):
             return False
         else:
             raise
     except TypeError as e:
-        if str(e).startswith('cannot unpack non-iterable'):
+        if str(e).startswith("cannot unpack non-iterable"):
             return False
         elif "not supported between instances of" in str(e):
             return False
-        elif 'object is not iterable' in str(e):
+        elif "object is not iterable" in str(e):
             return False
         else:
             raise
 
 
 def _is_xy_XY(bbox):
     """WARNING:
     Returns True if the bbox has the xy_wh format and x < w and y < h
     There's no way to check against that case
 
     Kept hidden to avoid cluttering the namespace
     """
     if not is_sequence(bbox):
-        raise TypeError(f'Expected a sequence, got {type(bbox)}')
+        raise TypeError(f"Expected a sequence, got {type(bbox)}")
 
     try:
         (x, y), (X, Y) = bbox
         return (0 <= x < X) and (0 <= y < Y)
     except ValueError as e:
-        if str(e).startswith('not enough values to unpack'):
+        if str(e).startswith("not enough values to unpack"):
             return False
-        elif str(e).startswith('too many values to unpack'):
+        elif str(e).startswith("too many values to unpack"):
             return False
         else:
             raise
     except TypeError as e:
-        if str(e).startswith('cannot unpack non-iterable'):
+        if str(e).startswith("cannot unpack non-iterable"):
             return False
         elif "not supported between instances of" in str(e):
             return False
-        elif 'object is not iterable' in str(e):
+        elif "object is not iterable" in str(e):
             return False
         else:
             raise
 
 
 def _is_xy_XY_s(bbox):
     """WARNING:
     Returns True if the bbox has the xywh format and x < w and y < h
     There's no way to check against that case
 
     Kept hidden to avoid cluttering the namespace
     """
     if not is_sequence(bbox):
-        raise TypeError(f'Expected a sequence, got {type(bbox)}')
+        raise TypeError(f"Expected a sequence, got {type(bbox)}")
 
     try:
         (x, y), (X, Y), s = bbox
         return (0 <= x < X) and (0 <= y < Y) and 0 <= s <= 1
     except ValueError as e:
-        if str(e).startswith('not enough values to unpack'):
+        if str(e).startswith("not enough values to unpack"):
             return False
-        elif str(e).startswith('too many values to unpack'):
+        elif str(e).startswith("too many values to unpack"):
             return False
         else:
             raise
     except TypeError as e:
-        if str(e).startswith('cannot unpack non-iterable'):
+        if str(e).startswith("cannot unpack non-iterable"):
             return False
         elif "not supported between instances of" in str(e):
             return False
-        elif 'object is not iterable' in str(e):
+        elif "object is not iterable" in str(e):
             return False
         else:
             raise
 
 
 def _is_xywh(bbox):
     """WARNING:
     Returns True if the bbox has the xyXY format
     There's no way to check against that case
 
     Kept hidden to avoid cluttering the namespace
     """
     if not is_sequence(bbox):
-        raise TypeError(f'Expected a sequence, got {type(bbox)}')
+        raise TypeError(f"Expected a sequence, got {type(bbox)}")
 
     try:
         (x, y, w, h) = bbox
         return (x >= 0) and (y >= 0) and (w > 0) and (h > 0)
     except ValueError as e:
-        if str(e).startswith('not enough values to unpack'):
+        if str(e).startswith("not enough values to unpack"):
             return False
-        elif str(e).startswith('too many values to unpack'):
+        elif str(e).startswith("too many values to unpack"):
             return False
         else:
             raise
     except TypeError as e:
-        if str(e).startswith('cannot unpack non-iterable'):
+        if str(e).startswith("cannot unpack non-iterable"):
             return False
         elif "not supported between instances of" in str(e):
             return False
-        elif 'object is not iterable' in str(e):
+        elif "object is not iterable" in str(e):
             return False
         else:
             raise
 
 
 def _is_xywh_s(bbox):
     """WARNING:
     Returns True if the bbox has the xyXY format
     There's no way to check against that case
 
     Kept hidden to avoid cluttering the namespace
     """
     if not is_sequence(bbox):
-        raise TypeError(f'Expected a sequence, got {type(bbox)}')
+        raise TypeError(f"Expected a sequence, got {type(bbox)}")
 
     try:
         (x, y, w, h), s = bbox
         return (x >= 0) and (y >= 0) and (w > 0) and (h > 0) and 0 <= s <= 1
     except ValueError as e:
-        if str(e).startswith('not enough values to unpack'):
+        if str(e).startswith("not enough values to unpack"):
             return False
-        elif str(e).startswith('too many values to unpack'):
+        elif str(e).startswith("too many values to unpack"):
             return False
         else:
             raise
     except TypeError as e:
-        if str(e).startswith('cannot unpack non-iterable'):
+        if str(e).startswith("cannot unpack non-iterable"):
             return False
         elif "not supported between instances of" in str(e):
             return False
-        elif 'object is not iterable' in str(e):
+        elif "object is not iterable" in str(e):
             return False
         else:
             raise
 
 
 def _is_xywhs(bbox):
     """WARNING:
     Returns True if the bbox has the xyXY format
     There's no way to check against that case
 
     Kept hidden to avoid cluttering the namespace
     """
     if not is_sequence(bbox):
-        raise TypeError(f'Expected a sequence, got {type(bbox)}')
+        raise TypeError(f"Expected a sequence, got {type(bbox)}")
 
     try:
         (x, y, w, h, s) = bbox
         return (x >= 0) and (y >= 0) and (w > 0) and (h > 0) and 0 <= s <= 1
     except ValueError as e:
-        if str(e).startswith('not enough values to unpack'):
+        if str(e).startswith("not enough values to unpack"):
             return False
-        elif str(e).startswith('too many values to unpack'):
+        elif str(e).startswith("too many values to unpack"):
             return False
         else:
             raise
     except TypeError as e:
-        if str(e).startswith('cannot unpack non-iterable'):
+        if str(e).startswith("cannot unpack non-iterable"):
             return False
         elif "not supported between instances of" in str(e):
             return False
-        elif 'object is not iterable' in str(e):
+        elif "object is not iterable" in str(e):
             return False
         else:
             raise
 
 
 def _is_xyXY(bbox):
     """WARNING:
     Returns True if the bbox has the xywh format and x < w and y < h
     There's no way to check against that case
 
     Kept hidden to avoid cluttering the namespace
     """
     if not is_sequence(bbox):
-        raise TypeError(f'Expected a sequence, got {type(bbox)}')
+        raise TypeError(f"Expected a sequence, got {type(bbox)}")
 
     try:
         (x, y, X, Y) = bbox
         return (0 <= x < X) and (0 <= y < Y)
     except ValueError as e:
-        if str(e).startswith('not enough values to unpack'):
+        if str(e).startswith("not enough values to unpack"):
             return False
-        elif str(e).startswith('too many values to unpack'):
+        elif str(e).startswith("too many values to unpack"):
             return False
         else:
             raise
     except TypeError as e:
-        if str(e).startswith('cannot unpack non-iterable'):
+        if str(e).startswith("cannot unpack non-iterable"):
             return False
         elif "not supported between instances of" in str(e):
             return False
-        elif 'object is not iterable' in str(e):
+        elif "object is not iterable" in str(e):
             return False
         else:
             raise
 
 
 def _is_xyXY_s(bbox):
     """WARNING:
     Returns True if the bbox has the xywh format and x < w and y < h
     There's no way to check against that case
 
     Kept hidden to avoid cluttering the namespace
     """
     if not is_sequence(bbox):
-        raise TypeError(f'Expected a sequence, got {type(bbox)}')
+        raise TypeError(f"Expected a sequence, got {type(bbox)}")
 
     try:
         (x, y, X, Y), s = bbox
         return (0 <= x < X) and (0 <= y < Y) and 0 <= s <= 1
     except ValueError as e:
-        if str(e).startswith('not enough values to unpack'):
+        if str(e).startswith("not enough values to unpack"):
             return False
-        elif str(e).startswith('too many values to unpack'):
+        elif str(e).startswith("too many values to unpack"):
             return False
         else:
             raise
     except TypeError as e:
-        if str(e).startswith('cannot unpack non-iterable'):
+        if str(e).startswith("cannot unpack non-iterable"):
             return False
         elif "not supported between instances of" in str(e):
             return False
-        elif 'object is not iterable' in str(e):
+        elif "object is not iterable" in str(e):
             return False
         else:
             raise
 
 
 def _is_xyXYs(bbox):
     """WARNING:
     Returns True if the bbox has the xywh format and x < w and y < h
     There's no way to check against that case
 
     Kept hidden to avoid cluttering the namespace
     """
     if not is_sequence(bbox):
-        raise TypeError(f'Expected a sequence, got {type(bbox)}')
+        raise TypeError(f"Expected a sequence, got {type(bbox)}")
 
     try:
         (x, y, X, Y, s) = bbox
         return (0 <= x < X) and (0 <= y < Y) and 0 <= s <= 1
     except ValueError as e:
-        if str(e).startswith('not enough values to unpack'):
+        if str(e).startswith("not enough values to unpack"):
             return False
-        elif str(e).startswith('too many values to unpack'):
+        elif str(e).startswith("too many values to unpack"):
             return False
         else:
             raise
     except TypeError as e:
-        if str(e).startswith('cannot unpack non-iterable'):
+        if str(e).startswith("cannot unpack non-iterable"):
             return False
         elif "not supported between instances of" in str(e):
             return False
-        elif 'object is not iterable' in str(e):
+        elif "object is not iterable" in str(e):
             return False
         else:
             raise
 
 
 # Define at the end of the file because it requires
 # the functions to be already defined
 _FORMATS = {
-    'xyXY': _is_xyXY,
-    'xyXY_s': _is_xyXY_s,
-    'xyXYs': _is_xyXYs,
-    'xy_XY': _is_xy_XY,
-    'xy_XY_s': _is_xy_XY_s,
-    'xy_wh': _is_xy_wh,
-    'xy_wh_s': _is_xy_wh_s,
-    'xywh': _is_xywh,
-    'xywh_s': _is_xywh_s,
-    'xywhs': _is_xywhs,
+    "xyXY": _is_xyXY,
+    "xyXY_s": _is_xyXY_s,
+    "xyXYs": _is_xyXYs,
+    "xy_XY": _is_xy_XY,
+    "xy_XY_s": _is_xy_XY_s,
+    "xy_wh": _is_xy_wh,
+    "xy_wh_s": _is_xy_wh_s,
+    "xywh": _is_xywh,
+    "xywh_s": _is_xywh_s,
+    "xywhs": _is_xywhs,
 }
```

### Comparing `katalytic-0.2.2/src/katalytic/meta/__init__.py` & `katalytic-0.3.0/src/katalytic/meta/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module implements meta-programming utilities.
 They should be used only when absolutely necessary.
 """
 import inspect
 
+
 from pathlib import Path
 
 
 def reference_caller_function(*, depth=1):
     """
     Returns a reference to the calling function, based on the specified depth.
 
@@ -38,22 +39,22 @@
         >>> bar()
         bar() called foo()
 
     """
     # I have to execute the preconditions both here and in extract_call_stack_info() because
     # of the depth+1 operation. Otherwise, I might do `True + 1` which python evaluates to 2
     if not isinstance(depth, int):
-        raise TypeError(f'depth must be an integer, not {type(depth).__name__}')
+        raise TypeError(f"depth must be an integer, not {type(depth).__name__}")
     elif isinstance(depth, bool):
-        raise TypeError(f'depth must be an integer, not bool')
+        raise TypeError(f"depth must be an integer, not bool")
     elif depth < 0:
-        raise ValueError(f'depth must be >= 0, not {depth}')
+        raise ValueError(f"depth must be >= 0, not {depth}")
 
     # reference_caller_function() adds an extra frame to the stack so you should use depth=depth+1
-    return extract_call_stack_info(depth=depth+1)[1]
+    return extract_call_stack_info(depth=depth + 1)[1]
 
 
 def extract_call_stack_info(*, depth=0):
     """
     Returns the file path, caller function reference, and line number, based on the specified depth.
 
     This function inspects the stack frames to retrieve the function that called it.
@@ -70,44 +71,46 @@
 
     Raises:
         TypeError: If depth is not an integer.
         ValueError: If depth is less than 0 or more than the number of available stack frames.
 
     """
     if not isinstance(depth, int):
-        raise TypeError(f'depth must be an integer, not {type(depth).__name__}')
+        raise TypeError(f"depth must be an integer, not {type(depth).__name__}")
     elif isinstance(depth, bool):
-        raise TypeError(f'depth must be an integer, not bool')
+        raise TypeError(f"depth must be an integer, not bool")
     elif depth < 0:
-        raise ValueError(f'depth must be >= 0, not {depth}')
+        raise ValueError(f"depth must be >= 0, not {depth}")
 
     stack = inspect.stack()
     if depth >= len(stack):
-        raise ValueError(f'You\'re getting ahead of yourself. There are only {len(stack)} frames in the stack, not {depth}.')
+        raise ValueError(
+            f"You're getting ahead of yourself. There are only {len(stack)} frames in the stack, not {depth}."
+        )
 
     # The stack is ordered from the most recent frame to the oldest frame
     # The most recent frame is this function, so we need to increase the depth by 1
-    frame_info = stack[depth+1]
+    frame_info = stack[depth + 1]
     caller = frame_info.frame.f_code.co_name
     func = _search(caller, frame_info.frame.f_globals, recursion_limit=1)
 
     return str(Path(frame_info.filename).resolve()), func, frame_info.lineno
 
 
 def _search(key, data, recursion_limit):
     func = data.get(key)
     if func:
         return func
 
     next_level = []
     for k, obj in data.items():
-        if k.startswith('__'):
+        if k.startswith("__"):
             continue
 
-        obj_2 = getattr(obj, '__dict__', {})
+        obj_2 = getattr(obj, "__dict__", {})
         if key in obj_2:
             return obj_2[key]
 
         if obj_2:
             next_level.append(obj_2)
 
     if recursion_limit == 0:
```

### Comparing `katalytic-0.2.2/tests/test_bboxes.py` & `katalytic-0.3.0/tests/test_bboxes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 import itertools
 
 import pytest as pytest
 
-from katalytic.data import all_types_besides
+from katalytic._pkg import all_types_besides
+
 # noinspection PyProtectedMember
 from katalytic.maths.bboxes import (
-    _FORMATS, calc_bbox_area, calc_bbox_center, calc_IoB, calc_IoB_max, calc_IoB_min,
-    calc_IoU, convert_bbox, non_max_suppression, set_bbox_scores, intersect_bboxes, is_bbox)
+    _FORMATS,
+    calc_bbox_area,
+    calc_bbox_center,
+    calc_IoB,
+    calc_IoB_max,
+    calc_IoB_min,
+    calc_IoU,
+    convert_bbox,
+    non_max_suppression,
+    set_bbox_scores,
+    intersect_bboxes,
+    is_bbox,
+)
 
 
 _EXAMPLES = {
-    'xyXY': (1,2,9,9),
-    'xyXY_s': ((1,2,9,9), 0.5),
-    'xyXYs': (1,2,9,9,0.5),
-    'xy_XY': ((1,2), (9,9)),
-    'xy_XY_s': ((1,2), (9,9), 0.5),
-    'xy_wh': ((1,2), (8,7)),
-    'xy_wh_s': ((1,2), (8,7), 0.5),
-    'xywh': (1,2,8,7),
-    'xywh_s': ((1,2,8,7), 0.5),
-    'xywhs': (1,2,8,7,0.5),
+    "xyXY": (1, 2, 9, 9),
+    "xyXY_s": ((1, 2, 9, 9), 0.5),
+    "xyXYs": (1, 2, 9, 9, 0.5),
+    "xy_XY": ((1, 2), (9, 9)),
+    "xy_XY_s": ((1, 2), (9, 9), 0.5),
+    "xy_wh": ((1, 2), (8, 7)),
+    "xy_wh_s": ((1, 2), (8, 7), 0.5),
+    "xywh": (1, 2, 8, 7),
+    "xywh_s": ((1, 2, 8, 7), 0.5),
+    "xywhs": (1, 2, 8, 7, 0.5),
 }
 
 
 def _check_all_besides(bbox, blacklist):
     formats = set(_FORMATS) - set(blacklist)
     return list(itertools.product([bbox], formats))
 
@@ -32,327 +44,373 @@
     return [bbox for fmt, bbox in _EXAMPLES.items() if fmt not in blacklist]
 
 
 def _generate_all_possible_conversions():
     all_combinations = itertools.product(_EXAMPLES.items(), _EXAMPLES.items())
     possible = []
     for (fmt_1, box_1), (fmt_2, box_2) in all_combinations:
-        if fmt_2.endswith('s') and not fmt_1.endswith('s'):
+        if fmt_2.endswith("s") and not fmt_1.endswith("s"):
             continue
         elif fmt_2 == fmt_1:
             continue
 
         possible.append((box_1, fmt_1, fmt_2, box_2))
 
     return possible
 
 
 def _generate_all_impossible_conversions():
     all_combinations = itertools.product(_EXAMPLES.items(), _EXAMPLES.items())
     impossible = []
     for (fmt_1, box_1), (fmt_2, box_2) in all_combinations:
-        if fmt_2.endswith('s') and not fmt_1.endswith('s'):
+        if fmt_2.endswith("s") and not fmt_1.endswith("s"):
             impossible.append((box_1, fmt_1, fmt_2))
 
     return impossible
 
 
 class Test_calc_area:
-    @pytest.mark.parametrize('fmt, bbox', _EXAMPLES.items())
+    @pytest.mark.parametrize("fmt, bbox", _EXAMPLES.items())
     def test_all_formats(self, fmt, bbox):
         assert calc_bbox_area(bbox, fmt) == 8 * 7
 
-    @pytest.mark.parametrize('bbox, fmt, area', [
-        ((0, 0, 5, 5), 'xyXY', 25),
-        ((0, 0, 10, 10), 'xywh', 100),
-        ((0, 0, 1, 5), 'xyXY', 5),
-        ((0, 0, 10, 1), 'xywh', 10),
-    ])
+    @pytest.mark.parametrize(
+        "bbox, fmt, area",
+        [
+            ((0, 0, 5, 5), "xyXY", 25),
+            ((0, 0, 10, 10), "xywh", 100),
+            ((0, 0, 1, 5), "xyXY", 5),
+            ((0, 0, 10, 1), "xywh", 10),
+        ],
+    )
     def test_basic(self, bbox, fmt, area):
         assert calc_bbox_area(bbox, fmt) == area
 
 
 class Test_convert_bbox:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('sequences'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("sequences"))
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
-            convert_bbox(wrong_type, 'xyXY', 'xywh')
+            convert_bbox(wrong_type, "xyXY", "xywh")
 
-    @pytest.mark.parametrize('bbox, before, after, _', _generate_all_possible_conversions())
+    @pytest.mark.parametrize(
+        "bbox, before, after, _", _generate_all_possible_conversions()
+    )
     def test_not_the_specified_format(self, bbox, before, after, _):
         # skip false positives
-        if 'wh' in before and 'XY' in after:
+        if "wh" in before and "XY" in after:
             return
-        elif 'XY' in before and 'wh' in after:
+        elif "XY" in before and "wh" in after:
             return
 
         with pytest.raises(ValueError):
             convert_bbox(bbox, after, before)
 
-    @pytest.mark.parametrize('fmt, bbox', _EXAMPLES.items())
+    @pytest.mark.parametrize("fmt, bbox", _EXAMPLES.items())
     def test_same_format(self, fmt, bbox):
         with pytest.raises(ValueError):
             convert_bbox(bbox, fmt, fmt)
 
-    @pytest.mark.parametrize('wrong_format', [1, None, 'asd', 'qwerty'])
+    @pytest.mark.parametrize("wrong_format", [1, None, "asd", "qwerty"])
     def test_wrong_format(self, wrong_format):
         with pytest.raises(ValueError):
-            convert_bbox((1,2,3,4), 'xywh', wrong_format)
+            convert_bbox((1, 2, 3, 4), "xywh", wrong_format)
 
         with pytest.raises(ValueError):
-            convert_bbox((1,2,3,4), wrong_format, 'xywh')
+            convert_bbox((1, 2, 3, 4), wrong_format, "xywh")
 
-    @pytest.mark.parametrize('bbox, before, after', _generate_all_impossible_conversions())
+    @pytest.mark.parametrize(
+        "bbox, before, after", _generate_all_impossible_conversions()
+    )
     def test_impossible(self, bbox, before, after):
         with pytest.raises(ValueError):
             convert_bbox(bbox, before, after)
 
-    @pytest.mark.parametrize('bbox, before, after, expected', _generate_all_possible_conversions())
+    @pytest.mark.parametrize(
+        "bbox, before, after, expected", _generate_all_possible_conversions()
+    )
     def test_expected(self, bbox, before, after, expected):
         assert convert_bbox(bbox, before, after) == expected
 
 
 class Test_calc_bbox_center:
-    @pytest.mark.parametrize('bbox, fmt, expected', [
-        ((0, 0, 5, 4), 'xyXY', (2.5, 2)),
-        ((0, 0, 3, 10), 'xywh', (1.5, 5.0)),
-    ])
+    @pytest.mark.parametrize(
+        "bbox, fmt, expected",
+        [
+            ((0, 0, 5, 4), "xyXY", (2.5, 2)),
+            ((0, 0, 3, 10), "xywh", (1.5, 5.0)),
+        ],
+    )
     def test_float(self, bbox, fmt, expected):
         assert calc_bbox_center(bbox, fmt) == expected
 
-    @pytest.mark.parametrize('bbox, fmt, expected', [
-        ((0, 0, 5, 4), 'xyXY', (2, 2)),
-        ((0, 0, 3, 10), 'xywh', (1, 5)),
-    ])
+    @pytest.mark.parametrize(
+        "bbox, fmt, expected",
+        [
+            ((0, 0, 5, 4), "xyXY", (2, 2)),
+            ((0, 0, 3, 10), "xywh", (1, 5)),
+        ],
+    )
     def test_int(self, bbox, fmt, expected):
         assert calc_bbox_center(bbox, fmt, as_int=True) == expected
 
 
 class Test_calc_IoU:
-    @pytest.mark.parametrize('bbox, fmt_1, bbox_2, fmt_2', [
-        ((0, 0, 5, 5), 'xyXY', (5, 5, 10, 10), 'xyXY'),
-        ((1, 1, 4, 4), 'xywh', (6, 6, 9, 9), 'xyXY'),
-    ])
+    @pytest.mark.parametrize(
+        "bbox, fmt_1, bbox_2, fmt_2",
+        [
+            ((0, 0, 5, 5), "xyXY", (5, 5, 10, 10), "xyXY"),
+            ((1, 1, 4, 4), "xywh", (6, 6, 9, 9), "xyXY"),
+        ],
+    )
     def test_no_overlap(self, bbox, fmt_1, bbox_2, fmt_2):
         assert calc_IoU(bbox, fmt_1, bbox_2, fmt_2) == 0
 
-    @pytest.mark.parametrize('bbox_1, fmt_1, bbox_2, fmt_2', [
-        ((0, 0, 5, 5), 'xyXY', (0, 0, 5, 5), 'xyXY'),
-        ((1, 1, 4, 4), 'xywh', (1, 1, 5, 5), 'xyXY'),
-        (((1, 1), (4, 4), 0.3), 'xy_wh_s', ((1, 1), (5, 5), 0.6), 'xy_XY_s'),
-    ])
+    @pytest.mark.parametrize(
+        "bbox_1, fmt_1, bbox_2, fmt_2",
+        [
+            ((0, 0, 5, 5), "xyXY", (0, 0, 5, 5), "xyXY"),
+            ((1, 1, 4, 4), "xywh", (1, 1, 5, 5), "xyXY"),
+            (((1, 1), (4, 4), 0.3), "xy_wh_s", ((1, 1), (5, 5), 0.6), "xy_XY_s"),
+        ],
+    )
     def test_perfect_overlap(self, bbox_1, fmt_1, bbox_2, fmt_2):
         assert calc_IoU(bbox_1, fmt_1, bbox_2, fmt_2) == 1
 
-    @pytest.mark.parametrize('bbox_1, fmt_1, bbox_2, fmt_2, expected', [
-        ((0, 0, 5, 5), 'xyXY', (3, 4, 7, 7), 'xyXY', 0.05714285714285714),
-        ((0, 0, 5, 5), 'xyXY', (1, 1, 6, 6), 'xyXY', 0.47058823529411764),
-        (((0, 0, 5, 5), 0.9), 'xyXY_s', (0, 1, 10, 3), 'xywh', 0.375),
-    ])
+    @pytest.mark.parametrize(
+        "bbox_1, fmt_1, bbox_2, fmt_2, expected",
+        [
+            ((0, 0, 5, 5), "xyXY", (3, 4, 7, 7), "xyXY", 0.05714285714285714),
+            ((0, 0, 5, 5), "xyXY", (1, 1, 6, 6), "xyXY", 0.47058823529411764),
+            (((0, 0, 5, 5), 0.9), "xyXY_s", (0, 1, 10, 3), "xywh", 0.375),
+        ],
+    )
     def test_partial_overlap(self, bbox_1, fmt_1, bbox_2, fmt_2, expected):
         assert calc_IoU(bbox_1, fmt_1, bbox_2, fmt_2) == expected
 
 
 class Test_calc_IoB:
-    @pytest.mark.parametrize('bbox, fmt_1, bbox_2, fmt_2', [
-        ((0, 0, 5, 5), 'xyXY', (5, 5, 10, 10), 'xyXY'),
-        ((1, 1, 4, 4), 'xywh', (6, 6, 9, 9), 'xyXY'),
-    ])
+    @pytest.mark.parametrize(
+        "bbox, fmt_1, bbox_2, fmt_2",
+        [
+            ((0, 0, 5, 5), "xyXY", (5, 5, 10, 10), "xyXY"),
+            ((1, 1, 4, 4), "xywh", (6, 6, 9, 9), "xyXY"),
+        ],
+    )
     def test_no_overlap(self, bbox, fmt_1, bbox_2, fmt_2):
         assert calc_IoB(bbox, fmt_1, bbox_2, fmt_2) == 0
 
-    @pytest.mark.parametrize('bbox_1, fmt_1, bbox_2, fmt_2', [
-        ((0, 0, 5, 5), 'xyXY', (0, 0, 5, 5), 'xyXY'),
-        ((1, 1, 4, 4), 'xywh', (1, 1, 5, 5), 'xyXY'),
-        (((1, 1), (4, 4), 0.3), 'xy_wh_s', ((1, 1), (5, 5), 0.6), 'xy_XY_s'),
-    ])
+    @pytest.mark.parametrize(
+        "bbox_1, fmt_1, bbox_2, fmt_2",
+        [
+            ((0, 0, 5, 5), "xyXY", (0, 0, 5, 5), "xyXY"),
+            ((1, 1, 4, 4), "xywh", (1, 1, 5, 5), "xyXY"),
+            (((1, 1), (4, 4), 0.3), "xy_wh_s", ((1, 1), (5, 5), 0.6), "xy_XY_s"),
+        ],
+    )
     def test_perfect_overlap(self, bbox_1, fmt_1, bbox_2, fmt_2):
         assert calc_IoB(bbox_1, fmt_1, bbox_2, fmt_2) == 1
 
-    @pytest.mark.parametrize('bbox_1, fmt_1, bbox_2, fmt_2, expected', [
-        ((0, 0, 5, 5), 'xyXY', (3, 4, 7, 7), 'xyXY', 0.08),
-        ((0, 0, 5, 5), 'xyXY', (1, 1, 6, 6), 'xyXY', 0.64),
-        (((0, 0, 5, 5), 0.9), 'xyXY_s', (0, 1, 10, 3), 'xywh', 0.6),
-    ])
+    @pytest.mark.parametrize(
+        "bbox_1, fmt_1, bbox_2, fmt_2, expected",
+        [
+            ((0, 0, 5, 5), "xyXY", (3, 4, 7, 7), "xyXY", 0.08),
+            ((0, 0, 5, 5), "xyXY", (1, 1, 6, 6), "xyXY", 0.64),
+            (((0, 0, 5, 5), 0.9), "xyXY_s", (0, 1, 10, 3), "xywh", 0.6),
+        ],
+    )
     def test_partial_overlap(self, bbox_1, fmt_1, bbox_2, fmt_2, expected):
         assert calc_IoB(bbox_1, fmt_1, bbox_2, fmt_2) == expected
 
 
 class Test_calc_IoB_min:
-    @pytest.mark.parametrize('bbox_1, fmt_1, bbox_2, fmt_2, expected', [
-        ((0, 0, 5, 5), 'xyXY', (3, 4, 7, 7), 'xyXY', 0.08),
-        ((0, 0, 5, 5), 'xyXY', (1, 1, 6, 6), 'xyXY', 0.64),
-        (((0, 0, 5, 5), 0.9), 'xyXY_s', (0, 1, 10, 3), 'xywh', 0.5),
-    ])
+    @pytest.mark.parametrize(
+        "bbox_1, fmt_1, bbox_2, fmt_2, expected",
+        [
+            ((0, 0, 5, 5), "xyXY", (3, 4, 7, 7), "xyXY", 0.08),
+            ((0, 0, 5, 5), "xyXY", (1, 1, 6, 6), "xyXY", 0.64),
+            (((0, 0, 5, 5), 0.9), "xyXY_s", (0, 1, 10, 3), "xywh", 0.5),
+        ],
+    )
     def test_partial_overlap(self, bbox_1, fmt_1, bbox_2, fmt_2, expected):
         assert calc_IoB_min(bbox_1, fmt_1, bbox_2, fmt_2) == expected
 
 
 class Test_calc_IoB_max:
-    @pytest.mark.parametrize('bbox_1, fmt_1, bbox_2, fmt_2, expected', [
-        ((0, 0, 5, 5), 'xyXY', (3, 4, 7, 7), 'xyXY', 0.16666666666666666),
-        ((0, 0, 5, 5), 'xyXY', (1, 1, 6, 6), 'xyXY', 0.64),
-        (((0, 0, 5, 5), 0.9), 'xyXY_s', (0, 1, 10, 3), 'xywh', 0.6),
-    ])
+    @pytest.mark.parametrize(
+        "bbox_1, fmt_1, bbox_2, fmt_2, expected",
+        [
+            ((0, 0, 5, 5), "xyXY", (3, 4, 7, 7), "xyXY", 0.16666666666666666),
+            ((0, 0, 5, 5), "xyXY", (1, 1, 6, 6), "xyXY", 0.64),
+            (((0, 0, 5, 5), 0.9), "xyXY_s", (0, 1, 10, 3), "xywh", 0.6),
+        ],
+    )
     def test_partial_overlap(self, bbox_1, fmt_1, bbox_2, fmt_2, expected):
         assert calc_IoB_max(bbox_1, fmt_1, bbox_2, fmt_2) == expected
 
 
 class Test_set_bbox_scores:
-    @pytest.mark.parametrize('after', ['xywh', 'xy_XY', 'xy_wh'])
+    @pytest.mark.parametrize("after", ["xywh", "xy_XY", "xy_wh"])
     def test_invalid_after_format(self, after):
         with pytest.raises(ValueError):
-            set_bbox_scores([(1,2,3,4)], [0], 'xyXY', after)
+            set_bbox_scores([(1, 2, 3, 4)], [0], "xyXY", after)
 
-    @pytest.mark.parametrize('scores', [-1, -0.1, 1.1, 2, 3.5])
+    @pytest.mark.parametrize("scores", [-1, -0.1, 1.1, 2, 3.5])
     def test_invalid_scores(self, scores):
         with pytest.raises(ValueError):
-            set_bbox_scores([(1,2,3,4)], [scores], 'xyXY', 'xyXYs')
+            set_bbox_scores([(1, 2, 3, 4)], [scores], "xyXY", "xyXYs")
 
-    @pytest.mark.parametrize('bboxes, scores', [
-        ([(1,2,3,4)], [1, 0.2]),
-        ([(1,2,3,4), (1,2,3,4)], [1]),
-    ])
+    @pytest.mark.parametrize(
+        "bboxes, scores",
+        [
+            ([(1, 2, 3, 4)], [1, 0.2]),
+            ([(1, 2, 3, 4), (1, 2, 3, 4)], [1]),
+        ],
+    )
     def test_unequal_lengths(self, bboxes, scores):
         with pytest.raises(ValueError):
-            set_bbox_scores(bboxes, scores, 'xyXY', 'xyXYs')
+            set_bbox_scores(bboxes, scores, "xyXY", "xyXYs")
 
-    @pytest.mark.parametrize('bboxes, scores, before, after, expected', [
-        (
-            [((1,2),(3,4))],
-            [1],
-            'xy_XY',
-            'xyXYs',
-            [(1,2,3,4,1)]
-        ),
-        (
-            [((1,2),(3,4)), ((2,2),(3,4))],
-            [1, 0.2],
-            'xy_XY',
-            'xyXYs',
-            [(1,2,3,4,1), (2,2,3,4,0.2)]
-        ),
-        (
-            [((1,2,3,4)), ((2,2,3,4))],
-            [1, 0.2],
-            'xyXY',
-            'xyXY_s',
-            [((1,2,3,4), 1), ((2,2,3,4), 0.2)]
-        ),
-    ])
+    @pytest.mark.parametrize(
+        "bboxes, scores, before, after, expected",
+        [
+            ([((1, 2), (3, 4))], [1], "xy_XY", "xyXYs", [(1, 2, 3, 4, 1)]),
+            (
+                [((1, 2), (3, 4)), ((2, 2), (3, 4))],
+                [1, 0.2],
+                "xy_XY",
+                "xyXYs",
+                [(1, 2, 3, 4, 1), (2, 2, 3, 4, 0.2)],
+            ),
+            (
+                [((1, 2, 3, 4)), ((2, 2, 3, 4))],
+                [1, 0.2],
+                "xyXY",
+                "xyXY_s",
+                [((1, 2, 3, 4), 1), ((2, 2, 3, 4), 0.2)],
+            ),
+        ],
+    )
     def test_ok(self, bboxes, scores, before, after, expected):
         assert set_bbox_scores(bboxes, scores, before, after) == expected
 
 
 class Test_non_max_suppression:
     def test_no_scores(self):
         with pytest.raises(ValueError):
-            non_max_suppression([(1,2,3,4)], 'xyXY')
+            non_max_suppression([(1, 2, 3, 4)], "xyXY")
 
     def test_scores(self):
-        bboxes = [(1,2,3,4), (5,6,7,8), (5,6,7,7)]
-        expected = [(1,2,3,4), (5,6,7,8)]
+        bboxes = [(1, 2, 3, 4), (5, 6, 7, 8), (5, 6, 7, 7)]
+        expected = [(1, 2, 3, 4), (5, 6, 7, 8)]
         scores = [0.9, 0.8, 0.7]
-        assert non_max_suppression(bboxes, 'xyXY', scores=scores) == expected
+        assert non_max_suppression(bboxes, "xyXY", scores=scores) == expected
 
     def test_empty(self):
-        assert non_max_suppression([], 'xyXYs') == []
+        assert non_max_suppression([], "xyXYs") == []
 
     def test_perfect_overlap(self):
         bboxes = [
             ((10, 10, 100, 100), 0.9),
             ((10, 10, 100, 100), 0.8),
-            ((10, 10, 100, 100), 0.7)
+            ((10, 10, 100, 100), 0.7),
         ]
 
-        assert non_max_suppression(bboxes, 'xyXY_s') == [((10, 10, 100, 100), 0.9)]
+        assert non_max_suppression(bboxes, "xyXY_s") == [((10, 10, 100, 100), 0.9)]
 
     def test_no_overlap(self):
-        bboxes = expected = [
-            [10, 10, 50, 50, 0.9],
-            [60, 60, 100, 100, 0.8]
-        ]
+        bboxes = expected = [[10, 10, 50, 50, 0.9], [60, 60, 100, 100, 0.8]]
 
-        assert non_max_suppression(bboxes, 'xyXYs') == expected
+        assert non_max_suppression(bboxes, "xyXYs") == expected
 
     def test_partial_overlap(self):
         bboxes = [
             [10, 10, 100, 100, 0.9],
             [100, 100, 190, 190, 0.6],
             [100, 100, 185, 185, 0.7],
             [90, 90, 190, 190, 0.7],
             [50, 50, 150, 150, 0.8],
         ]
 
-        assert non_max_suppression(bboxes, 'xyXYs') == [
+        assert non_max_suppression(bboxes, "xyXYs") == [
             [10, 10, 100, 100, 0.9],
             [50, 50, 150, 150, 0.8],
             [100, 100, 185, 185, 0.7],
         ]
 
 
 class Test_intersect_bboxes:
-    @pytest.mark.parametrize('bbox_1, fmt_1, bbox_2, fmt_2', [
-        ((0, 0, 5, 5), 'xyXY', (5, 5, 10, 10), 'xyXY'),
-        ((1, 1, 4, 4), 'xywh', (6, 6, 9, 9), 'xyXY'),
-    ])
+    @pytest.mark.parametrize(
+        "bbox_1, fmt_1, bbox_2, fmt_2",
+        [
+            ((0, 0, 5, 5), "xyXY", (5, 5, 10, 10), "xyXY"),
+            ((1, 1, 4, 4), "xywh", (6, 6, 9, 9), "xyXY"),
+        ],
+    )
     def test_no_overlap(self, bbox_1, fmt_1, bbox_2, fmt_2):
         assert intersect_bboxes(bbox_1, fmt_1, bbox_2, fmt_2) is None
 
-    @pytest.mark.parametrize('bbox_1, fmt_1, bbox_2, fmt_2', [
-        ((0, 0, 5, 5), 'xyXY', (0, 0, 5, 5), 'xyXY'),
-        ((1, 1, 4, 4), 'xywh', (1, 1, 5, 5), 'xyXY'),
-        (((1, 1), (4, 4), 0.3), 'xy_wh_s', ((1, 1), (5, 5), 0.6), 'xy_XY_s'),
-    ])
+    @pytest.mark.parametrize(
+        "bbox_1, fmt_1, bbox_2, fmt_2",
+        [
+            ((0, 0, 5, 5), "xyXY", (0, 0, 5, 5), "xyXY"),
+            ((1, 1, 4, 4), "xywh", (1, 1, 5, 5), "xyXY"),
+            (((1, 1), (4, 4), 0.3), "xy_wh_s", ((1, 1), (5, 5), 0.6), "xy_XY_s"),
+        ],
+    )
     def test_perfect_overlap(self, bbox_1, fmt_1, bbox_2, fmt_2):
         assert intersect_bboxes(bbox_1, fmt_1, bbox_2, fmt_2) == bbox_1
 
-    @pytest.mark.parametrize('bbox_1, fmt_1, bbox_2, fmt_2, expected', [
-        ((0, 0, 5, 5), 'xyXY', (3, 4, 7, 7), 'xyXY', (3, 4, 5, 5)),
-        (((0, 0, 5, 5), 0.9), 'xyXY_s', (0, 1, 10, 3), 'xywh', ((0, 1, 5, 4), 0.9)),
-    ])
+    @pytest.mark.parametrize(
+        "bbox_1, fmt_1, bbox_2, fmt_2, expected",
+        [
+            ((0, 0, 5, 5), "xyXY", (3, 4, 7, 7), "xyXY", (3, 4, 5, 5)),
+            (((0, 0, 5, 5), 0.9), "xyXY_s", (0, 1, 10, 3), "xywh", ((0, 1, 5, 4), 0.9)),
+        ],
+    )
     def test_partial_overlap(self, bbox_1, fmt_1, bbox_2, fmt_2, expected):
         assert intersect_bboxes(bbox_1, fmt_1, bbox_2, fmt_2) == expected
 
 
 class Test_is_bbox:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('sequences'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("sequences"))
     def test_wrong_format(self, wrong_type):
         with pytest.raises(TypeError):
-            is_bbox(wrong_type, 'xyXY')
+            is_bbox(wrong_type, "xyXY")
 
-    @pytest.mark.parametrize('fmt', [1, None, 'asd', 'qwerty'])
+    @pytest.mark.parametrize("fmt", [1, None, "asd", "qwerty"])
     def test_wrong_format(self, fmt):
         with pytest.raises(ValueError):
-            is_bbox((1,2,3,4), fmt)
+            is_bbox((1, 2, 3, 4), fmt)
 
-    @pytest.mark.parametrize('fmt, bbox', _EXAMPLES.items())
+    @pytest.mark.parametrize("fmt, bbox", _EXAMPLES.items())
     def test_True(self, fmt, bbox):
         assert is_bbox(bbox, fmt)
 
-    @pytest.mark.parametrize('bbox, fmt', [
-        *_check_all_besides((), []),
-        *_check_all_besides(range(1), []),
-        *_check_all_besides(range(2), []),
-        *_check_all_besides(range(3), []),
-        *_check_all_besides((*range(4), -0.1), []),
-        *_check_all_besides((*range(4), 1.1), []),
-        *_check_all_besides((*range(4), 2), []),
-        *_check_all_besides(range(6), []),
-        *_check_all_besides(((1,2),(3,4),(5,6),(7,8)), []),
-
-        *_check_all_besides(((1,2), (1,1)), ['xy_wh']),
-        *_check_all_besides(((1,2), (1,1), 0.5), ['xy_wh_s']),
-        *_check_all_besides((1,2,1,1), ['xywh']),
-        *_check_all_besides(((1,2,1,1), 0.5), ['xywh_s']),
-        *_check_all_besides((1,2,1,1,0.5), ['xywhs']),
-
-        # There's no way to check correctly against the "wh" equivalents
-        # They would return false positives and make the test fail
-        *_check_all_besides((1,2,3,4), ['xyXY', 'xywh']),
-        *_check_all_besides(((1,2,3,4), 0.5), ['xyXY_s', 'xywh_s']),
-        *_check_all_besides((1,2,3,4,0.5), ['xyXYs', 'xywhs']),
-        *_check_all_besides(((1,2), (3,4)), ['xy_XY', 'xy_wh']),
-        *_check_all_besides(((1,2), (3,4), 0.5), ['xy_XY_s', 'xy_wh_s']),
-    ])
+    @pytest.mark.parametrize(
+        "bbox, fmt",
+        [
+            *_check_all_besides((), []),
+            *_check_all_besides(range(1), []),
+            *_check_all_besides(range(2), []),
+            *_check_all_besides(range(3), []),
+            *_check_all_besides((*range(4), -0.1), []),
+            *_check_all_besides((*range(4), 1.1), []),
+            *_check_all_besides((*range(4), 2), []),
+            *_check_all_besides(range(6), []),
+            *_check_all_besides(((1, 2), (3, 4), (5, 6), (7, 8)), []),
+            *_check_all_besides(((1, 2), (1, 1)), ["xy_wh"]),
+            *_check_all_besides(((1, 2), (1, 1), 0.5), ["xy_wh_s"]),
+            *_check_all_besides((1, 2, 1, 1), ["xywh"]),
+            *_check_all_besides(((1, 2, 1, 1), 0.5), ["xywh_s"]),
+            *_check_all_besides((1, 2, 1, 1, 0.5), ["xywhs"]),
+            # There's no way to check correctly against the "wh" equivalents
+            # They would return false positives and make the test fail
+            *_check_all_besides((1, 2, 3, 4), ["xyXY", "xywh"]),
+            *_check_all_besides(((1, 2, 3, 4), 0.5), ["xyXY_s", "xywh_s"]),
+            *_check_all_besides((1, 2, 3, 4, 0.5), ["xyXYs", "xywhs"]),
+            *_check_all_besides(((1, 2), (3, 4)), ["xy_XY", "xy_wh"]),
+            *_check_all_besides(((1, 2), (3, 4), 0.5), ["xy_XY_s", "xy_wh_s"]),
+        ],
+    )
     def test_False(self, bbox, fmt):
         assert not is_bbox(bbox, fmt)
```

### Comparing `katalytic-0.2.2/tests/test_checks.py` & `katalytic-0.3.0/tests/test_checks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,545 +1,641 @@
 import pytest
 
+
 from katalytic.data.checks import (
-    contains_all_of, contains_any_of, contains_none_of, is_any_of, is_dict_of_sequences, is_generator,
-    is_generator_expression, is_generator_function, is_iterable, is_iterable_or_str, is_iterator, is_none_of, is_number,
-    is_primitive, is_sequence, is_sequence_of_dicts, is_sequence_of_sequences, is_sequence_or_str,
-    is_sequence_of_dicts_uniform, is_dict_of_sequences_uniform, is_sequence_of_sequences_uniform, dicts_share_key_order,
-    dicts_share_value_order, is_singleton, is_equal
+    contains_all_of,
+    contains_any_of,
+    contains_none_of,
+    is_any_of,
+    is_dict_of_sequences,
+    is_generator,
+    is_generator_expression,
+    is_generator_function,
+    is_iterable,
+    is_iterable_or_str,
+    is_iterator,
+    is_none_of,
+    is_number,
+    is_primitive,
+    is_sequence,
+    is_sequence_of_dicts,
+    is_sequence_of_sequences,
+    is_sequence_or_str,
+    is_sequence_of_dicts_uniform,
+    is_dict_of_sequences_uniform,
+    is_sequence_of_sequences_uniform,
+    dicts_share_key_order,
+    dicts_share_value_order,
+    is_singleton,
+    is_equal,
 )
 
-from katalytic.data import all_types, all_types_besides
+from katalytic._pkg import all_types, all_types_besides
 
 
 class Test_contains_all_of:
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_haystack_not_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             contains_all_of(wrong_type, [])
 
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_needles_not_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             contains_all_of([], wrong_type)
 
-    @pytest.mark.parametrize('haystack, needles', [
-        (range(10), {1, 3, 5}),
-        ({True, False, None}, [True, None]),
-        ({True, False, None}, [True, False]),
-        ({True, False, None}, [False, None]),
-    ])
+    @pytest.mark.parametrize(
+        "haystack, needles",
+        [
+            (range(10), {1, 3, 5}),
+            ({True, False, None}, [True, None]),
+            ({True, False, None}, [True, False]),
+            ({True, False, None}, [False, None]),
+        ],
+    )
     def test_True(self, haystack, needles):
         assert contains_all_of(haystack, needles)
 
-    @pytest.mark.parametrize('haystack, needles', [
-        (range(10), {True, 1, 3, 5}),
-        ([True], {(), 'hello', True}),
-        (range(10), [True, False]),
-        (range(10), [100, 666]),
-        ({None}, (True, False)),
-    ])
+    @pytest.mark.parametrize(
+        "haystack, needles",
+        [
+            (range(10), {True, 1, 3, 5}),
+            ([True], {(), "hello", True}),
+            (range(10), [True, False]),
+            (range(10), [100, 666]),
+            ({None}, (True, False)),
+        ],
+    )
     def test_False(self, haystack, needles):
         assert not contains_all_of(haystack, needles)
 
 
 class Test_contains_any_of:
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_haystack_not_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             contains_any_of(wrong_type, [])
 
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_needles_not_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             contains_any_of([], wrong_type)
 
-    @pytest.mark.parametrize('haystack, needles', [
-        (range(10), [True, False]),
-        (range(10), [100, 666]),
-        ({None}, (True, False)),
-    ])
+    @pytest.mark.parametrize(
+        "haystack, needles",
+        [
+            (range(10), [True, False]),
+            (range(10), [100, 666]),
+            ({None}, (True, False)),
+        ],
+    )
     def test_False(self, haystack, needles):
         assert not contains_any_of(haystack, needles)
 
-    @pytest.mark.parametrize('haystack, needles', [
-        (range(10), {True, False, 5}),
-        ([True], {(), 'hello', True}),
-    ])
+    @pytest.mark.parametrize(
+        "haystack, needles",
+        [
+            (range(10), {True, False, 5}),
+            ([True], {(), "hello", True}),
+        ],
+    )
     def test_True(self, haystack, needles):
         assert contains_any_of(haystack, needles)
 
 
 class Test_contains_none_of:
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_haystack_not_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             contains_none_of(wrong_type, [])
 
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_needles_not_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             contains_none_of([], wrong_type)
 
-    @pytest.mark.parametrize('haystack, needles', [
-        (range(10), [True, False]),
-        (range(10), [100, 666]),
-        ({None}, (True, False)),
-    ])
+    @pytest.mark.parametrize(
+        "haystack, needles",
+        [
+            (range(10), [True, False]),
+            (range(10), [100, 666]),
+            ({None}, (True, False)),
+        ],
+    )
     def test_True(self, haystack, needles):
         assert contains_none_of(haystack, needles)
 
-    @pytest.mark.parametrize('haystack, needles', [
-        (range(10), {True, False, 5}),
-        ([True], {(), 'hello', True}),
-    ])
+    @pytest.mark.parametrize(
+        "haystack, needles",
+        [
+            (range(10), {True, False, 5}),
+            ([True], {(), "hello", True}),
+        ],
+    )
     def test_False(self, haystack, needles):
         assert not contains_none_of(haystack, needles)
 
 
 # noinspection PyTypeChecker
 class Test_dicts_share_key_order:
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_not_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             dicts_share_key_order({}, {}, recursive=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), 1, 1.0, None, "string", object()]
+    )
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             dicts_share_key_order({}, wrong_type)
 
         with pytest.raises(TypeError):
             dicts_share_key_order(wrong_type, wrong_type)
 
         with pytest.raises(TypeError):
-            dicts_share_key_order({'a': {}}, {'a': wrong_type}, recursive=True)
+            dicts_share_key_order({"a": {}}, {"a": wrong_type}, recursive=True)
 
-    @pytest.mark.parametrize('wrong_type', [[], (), 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize("wrong_type", [[], (), 1, 1.0, None, "string", object()])
     def test_no_dicts(self, wrong_type):
         with pytest.raises(TypeError):
             dicts_share_key_order(wrong_type, wrong_type, recursive=False)
 
-    @pytest.mark.parametrize('wrong_type', [{}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize("wrong_type", [{}, 1, 1.0, None, "string", object()])
     def test_not_a_sequence(self, wrong_type):
         with pytest.raises(TypeError):
             dicts_share_key_order([], wrong_type, recursive=True)
 
         with pytest.raises(TypeError):
-            dicts_share_key_order({'a': []}, {'a': wrong_type}, recursive=True)
+            dicts_share_key_order({"a": []}, {"a": wrong_type}, recursive=True)
 
     def test_empty(self):
         assert dicts_share_key_order({}, {})
 
-    @pytest.mark.parametrize('dict_1, dict_2', [
-        [{'a': 1, 'b': 2}, {'a': 3, 'b': 4}],
-        [{'a': {'b': 1, 'c': 2}}, {'a': {'b': 1, 'c': 2}}],
-        [[{'a': 1, 'b': 2}], [{'a': 3, 'b': 4}]],
-    ])
+    @pytest.mark.parametrize(
+        "dict_1, dict_2",
+        [
+            [{"a": 1, "b": 2}, {"a": 3, "b": 4}],
+            [{"a": {"b": 1, "c": 2}}, {"a": {"b": 1, "c": 2}}],
+            [[{"a": 1, "b": 2}], [{"a": 3, "b": 4}]],
+        ],
+    )
     def test_True(self, dict_1, dict_2):
         assert dicts_share_key_order(dict_1, dict_2, recursive=True)
 
-    @pytest.mark.parametrize('dict_1, dict_2', [
-        [{'a': 1, 'b': 2}, {'b': 1, 'a': 2}],
-        [{'a': 1, 'b': 2}, {'a': 1, 'c': 2}],
-        [{'a': {'b': 1, 'c': 2}}, {'a': {'c': 1, 'b': 2}}],
-        [{'a': {'b': 1, 'c': 2}}, {'a': {'x': 1, 'y': 2}}],
-        [{'a': {'b': 1, 'c': 2}}, {'z': {'x': 1, 'y': 2}}],
-        [[{'a': 1, 'b': 2}], [{'b': 3, 'a': 4}]],
-        [[{'a': 1, 'b': 2}], [{'x': 3, 'y': 4}]],
-    ])
+    @pytest.mark.parametrize(
+        "dict_1, dict_2",
+        [
+            [{"a": 1, "b": 2}, {"b": 1, "a": 2}],
+            [{"a": 1, "b": 2}, {"a": 1, "c": 2}],
+            [{"a": {"b": 1, "c": 2}}, {"a": {"c": 1, "b": 2}}],
+            [{"a": {"b": 1, "c": 2}}, {"a": {"x": 1, "y": 2}}],
+            [{"a": {"b": 1, "c": 2}}, {"z": {"x": 1, "y": 2}}],
+            [[{"a": 1, "b": 2}], [{"b": 3, "a": 4}]],
+            [[{"a": 1, "b": 2}], [{"x": 3, "y": 4}]],
+        ],
+    )
     def test_False(self, dict_1, dict_2):
         assert not dicts_share_key_order(dict_1, dict_2, recursive=True)
 
 
 # noinspection PyTypeChecker
 class Test_dicts_share_value_order:
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_not_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             dicts_share_value_order({}, {}, recursive=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), 1, 1.0, None, "string", object()]
+    )
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             dicts_share_value_order({}, wrong_type)
 
         with pytest.raises(TypeError):
             dicts_share_value_order(wrong_type, wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], (), 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize("wrong_type", [[], (), 1, 1.0, None, "string", object()])
     def test_no_dicts(self, wrong_type):
         with pytest.raises(TypeError):
             dicts_share_value_order(wrong_type, wrong_type, recursive=False)
 
-    @pytest.mark.parametrize('wrong_type', [{}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize("wrong_type", [{}, 1, 1.0, None, "string", object()])
     def test_not_a_sequence(self, wrong_type):
         with pytest.raises(TypeError):
             dicts_share_value_order([], wrong_type)
 
     def test_empty(self):
         assert dicts_share_value_order({}, {})
 
-    @pytest.mark.parametrize('dict_1, dict_2', [
-        [{'a': 1, 'b': 2}, {'c': 1, 'd': 2}],
-        [{'a': {'b': 1, 'c': 2}}, {'b': {'b': 1, 'c': 2}}],
-        [[{'a': 1, 'b': 2}], [{'c': 1, 'd': 2}]],
-    ])
+    @pytest.mark.parametrize(
+        "dict_1, dict_2",
+        [
+            [{"a": 1, "b": 2}, {"c": 1, "d": 2}],
+            [{"a": {"b": 1, "c": 2}}, {"b": {"b": 1, "c": 2}}],
+            [[{"a": 1, "b": 2}], [{"c": 1, "d": 2}]],
+        ],
+    )
     def test_simple(self, dict_1, dict_2):
         assert dicts_share_value_order(dict_1, dict_2, recursive=True)
         assert dicts_share_value_order(dict_1, dict_2, recursive=True)
         assert dicts_share_value_order(dict_1, dict_2, recursive=True)
 
-    @pytest.mark.parametrize('dict_1, dict_2', [
-        [{'a': {'b': 1, 'c': 2}}, {'b': {'c': 1, 'b': 2}}],
-        [{'a': {'b': 1, 'c': 2}}, {'b': {'b': 2, 'c': 1}}],
-        [{'a': 1, 'b': 2}, {'c': 2, 'd': 1}],
-        [[{'a': 2, 'b': 1}], [{'c': 1, 'd': 2}]],
-    ])
+    @pytest.mark.parametrize(
+        "dict_1, dict_2",
+        [
+            [{"a": {"b": 1, "c": 2}}, {"b": {"c": 1, "b": 2}}],
+            [{"a": {"b": 1, "c": 2}}, {"b": {"b": 2, "c": 1}}],
+            [{"a": 1, "b": 2}, {"c": 2, "d": 1}],
+            [[{"a": 2, "b": 1}], [{"c": 1, "d": 2}]],
+        ],
+    )
     def test_recursive(self, dict_1, dict_2):
         assert not dicts_share_value_order(dict_1, dict_2, recursive=True)
 
 
 class Test_is_any_of:
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_not_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             is_any_of([], haystack=wrong_type)
 
-    @pytest.mark.parametrize('x, iterable', [
-        (0, [1, 2, 3]),
-        (4, [1, 2, 3]),
-        ('a', {'b': 'a', 'c': 'd'}),
-        ({}, [1, 2, 3]),
-        (True, {1, None, False}),
-    ])
+    @pytest.mark.parametrize(
+        "x, iterable",
+        [
+            (0, [1, 2, 3]),
+            (4, [1, 2, 3]),
+            ("a", {"b": "a", "c": "d"}),
+            ({}, [1, 2, 3]),
+            (True, {1, None, False}),
+        ],
+    )
     def test_False(self, x, iterable):
         assert not is_any_of(x, iterable)
 
-    @pytest.mark.parametrize('x, iterable', [
-        (2, [1, 2, 3]),
-        ('a', {'a': 'b', 'c': 'd'}),
-        ({}, [1, 2, {}, 3]),
-        (True, {None, True, False}),
-    ])
+    @pytest.mark.parametrize(
+        "x, iterable",
+        [
+            (2, [1, 2, 3]),
+            ("a", {"a": "b", "c": "d"}),
+            ({}, [1, 2, {}, 3]),
+            (True, {None, True, False}),
+        ],
+    )
     def test_True(self, x, iterable):
         assert is_any_of(x, iterable)
 
-    @pytest.mark.parametrize('x, iterable', [
-        (1, [True, False]),
-        (0, [True, False]),
-        (True, [0, 1]),
-        (False, [0, 1]),
-    ])
+    @pytest.mark.parametrize(
+        "x, iterable",
+        [
+            (1, [True, False]),
+            (0, [True, False]),
+            (True, [0, 1]),
+            (False, [0, 1]),
+        ],
+    )
     def test_bools_are_not_ints(self, x, iterable):
         assert not is_any_of(x, iterable)
 
 
 class Test_is_dict_of_sequences:
-    @pytest.mark.parametrize('correct_type', [{'a': []}, {'a': ()}])
+    @pytest.mark.parametrize("correct_type", [{"a": []}, {"a": ()}])
     def test_True(self, correct_type):
         assert is_dict_of_sequences(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('dict') + [{'a': {}}])
+    @pytest.mark.parametrize("wrong_type", all_types_besides("dict") + [{"a": {}}])
     def test_False(self, wrong_type):
         assert not is_dict_of_sequences(wrong_type)
 
     def test_empty_ok(self):
         assert is_dict_of_sequences({}, empty_ok=True)
         assert not is_dict_of_sequences({}, empty_ok=False)
 
-    @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+    @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
     def test_precondition_empty_ok(self, mistake):
         with pytest.raises(TypeError):
             is_dict_of_sequences([], empty_ok=mistake)
 
 
 class Test_is_dict_of_sequences_uniform:
-    @pytest.mark.parametrize('data', [
-        {'a': (), 'b': ()},
-        {'a': [1], 'b': [1]},
-        {'a': (1, 2, 3), 'b': [10, 20, 30]},
-    ])
+    @pytest.mark.parametrize(
+        "data",
+        [
+            {"a": (), "b": ()},
+            {"a": [1], "b": [1]},
+            {"a": (1, 2, 3), "b": [10, 20, 30]},
+        ],
+    )
     def test_True(self, data):
         assert is_dict_of_sequences_uniform(data)
 
-    @pytest.mark.parametrize('data', [
-        {'a': [1], 'b': []},
-        {'a': [1], 'b': [1, 2]},
-        {'a': [1], 'b': [1], 'c': [1, 2]},
-        []
-    ])
+    @pytest.mark.parametrize(
+        "data",
+        [
+            {"a": [1], "b": []},
+            {"a": [1], "b": [1, 2]},
+            {"a": [1], "b": [1], "c": [1, 2]},
+            [],
+        ],
+    )
     def test_False(self, data):
         assert not is_dict_of_sequences_uniform(data)
 
     def test_empty_ok(self):
         assert is_dict_of_sequences_uniform({}, empty_ok=True)
         assert not is_dict_of_sequences_uniform({}, empty_ok=False)
 
-    @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+    @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
     def test_precondition_empty_ok(self, mistake):
         with pytest.raises(TypeError):
             is_dict_of_sequences_uniform([], empty_ok=mistake)
 
 
 class Test_is_equal:
-    @pytest.mark.parametrize('a, b', [
-        (0, False),
-        (0, None),
-        (False, None),
-        (1, True),
-        (0, 1),
-        (1, '1'),
-    ])
+    @pytest.mark.parametrize(
+        "a, b",
+        [
+            (0, False),
+            (0, None),
+            (False, None),
+            (1, True),
+            (0, 1),
+            (1, "1"),
+        ],
+    )
     def test_False(self, a, b):
         assert not is_equal(a, b)
 
-    @pytest.mark.parametrize('a, b', [
-        (0, 0),
-        (1, 1),
-        (False, False),
-        (True, True),
-        (None, None),
-    ])
+    @pytest.mark.parametrize(
+        "a, b",
+        [
+            (0, 0),
+            (1, 1),
+            (False, False),
+            (True, True),
+            (None, None),
+        ],
+    )
     def test_True(self, a, b):
         assert is_equal(a, b)
 
 
 class Test_is_generator:
-    @pytest.mark.parametrize('correct_type', all_types('generators'))
+    @pytest.mark.parametrize("correct_type", all_types("generators"))
     def test_True(self, correct_type):
         assert is_generator(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('generators'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("generators"))
     def test_False(self, wrong_type):
         assert not is_generator(wrong_type)
 
 
 class Test_is_generator_function:
-    @pytest.mark.parametrize('correct_type', all_types('generator_function'))
+    @pytest.mark.parametrize("correct_type", all_types("generator_function"))
     def test_True(self, correct_type):
         assert is_generator_function(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('generator_function'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("generator_function"))
     def test_False(self, wrong_type):
         assert not is_generator_function(wrong_type)
 
 
 class Test_is_generator_expression:
-    @pytest.mark.parametrize('correct_type', all_types('generator_expression'))
+    @pytest.mark.parametrize("correct_type", all_types("generator_expression"))
     def test_True(self, correct_type):
         assert is_generator_expression(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('generator_expression'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("generator_expression"))
     def test_False(self, wrong_type):
         assert not is_generator_expression(wrong_type)
 
 
 class Test_is_iterable:
-    @pytest.mark.parametrize('correct_type', all_types('iterables'))
+    @pytest.mark.parametrize("correct_type", all_types("iterables"))
     def test_True(self, correct_type):
         assert is_iterable(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("iterables"))
     def test_False(self, wrong_type):
         assert not is_iterable(wrong_type)
 
 
 class Test_is_iterable_or_str:
-    @pytest.mark.parametrize('correct_type', all_types(['iterables', 'strings']))
+    @pytest.mark.parametrize("correct_type", all_types(["iterables", "strings"]))
     def test_True(self, correct_type):
         assert is_iterable_or_str(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides(['iterables', 'strings']))
+    @pytest.mark.parametrize("wrong_type", all_types_besides(["iterables", "strings"]))
     def test_False(self, wrong_type):
         assert not is_iterable_or_str(wrong_type)
 
 
 class Test_is_iterator:
-    @pytest.mark.parametrize('correct_type', all_types('iterators'))
+    @pytest.mark.parametrize("correct_type", all_types("iterators"))
     def test_True(self, correct_type):
         assert is_iterator(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('iterators'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("iterators"))
     def test_False(self, wrong_type):
         assert not is_iterator(wrong_type)
 
 
 class Test_is_none_of:
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_not_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             is_none_of([], haystack=wrong_type)
 
-    @pytest.mark.parametrize('x, iterable', [
-        (0, [1, 2, 3]),
-        (4, [1, 2, 3]),
-        ('a', {'b': 'a', 'c': 'd'}),
-        ({}, [1, 2, 3]),
-        (True, {1, None, False}),
-    ])
+    @pytest.mark.parametrize(
+        "x, iterable",
+        [
+            (0, [1, 2, 3]),
+            (4, [1, 2, 3]),
+            ("a", {"b": "a", "c": "d"}),
+            ({}, [1, 2, 3]),
+            (True, {1, None, False}),
+        ],
+    )
     def test_True(self, x, iterable):
         assert is_none_of(x, iterable)
 
-    @pytest.mark.parametrize('x, iterable', [
-        (2, [1, 2, 3]),
-        ('a', {'a': 'b', 'c': 'd'}),
-        ({}, [1, 2, {}, 3]),
-        (True, {None, True, False}),
-    ])
+    @pytest.mark.parametrize(
+        "x, iterable",
+        [
+            (2, [1, 2, 3]),
+            ("a", {"a": "b", "c": "d"}),
+            ({}, [1, 2, {}, 3]),
+            (True, {None, True, False}),
+        ],
+    )
     def test_False(self, x, iterable):
         assert not is_none_of(x, iterable)
 
-    @pytest.mark.parametrize('x, iterable', [
-        (1, [True, False]),
-        (0, [True, False]),
-        (True, [0, 1]),
-        (False, [0, 1]),
-    ])
+    @pytest.mark.parametrize(
+        "x, iterable",
+        [
+            (1, [True, False]),
+            (0, [True, False]),
+            (True, [0, 1]),
+            (False, [0, 1]),
+        ],
+    )
     def test_bools_are_not_ints(self, x, iterable):
         assert is_none_of(x, iterable)
 
 
 class Test_is_primitive:
-    @pytest.mark.parametrize('correct_type', all_types('primitives'))
+    @pytest.mark.parametrize("correct_type", all_types("primitives"))
     def test_True(self, correct_type):
         assert is_primitive(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('primitives'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("primitives"))
     def test_False(self, wrong_type):
         assert not is_primitive(wrong_type)
 
 
 class Test_is_sequence:
-    @pytest.mark.parametrize('correct_type', all_types('sequences'))
+    @pytest.mark.parametrize("correct_type", all_types("sequences"))
     def test_True(self, correct_type):
         assert is_sequence(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('sequences'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("sequences"))
     def test_False(self, wrong_type):
         assert not is_sequence(wrong_type)
 
 
 class Test_is_sequence_of_dicts:
-    @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+    @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
     def test_precondition_empty_ok(self, mistake):
         with pytest.raises(TypeError):
             is_sequence_of_dicts([], empty_ok=mistake)
 
-    @pytest.mark.parametrize('correct_type', [[{}], ({}, )])
+    @pytest.mark.parametrize("correct_type", [[{}], ({},)])
     def test_True(self, correct_type):
         assert is_sequence_of_dicts(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('sequences') + [{'a': []}])
+    @pytest.mark.parametrize("wrong_type", all_types_besides("sequences") + [{"a": []}])
     def test_False(self, wrong_type):
         assert not is_sequence_of_dicts(wrong_type)
 
     def test_empty_ok(self):
         assert is_sequence_of_dicts([], empty_ok=True)
         assert not is_sequence_of_dicts([], empty_ok=False)
 
 
 class Test_is_sequence_of_dicts_uniform:
-    @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+    @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
     def test_precondition_empty_ok(self, mistake):
         with pytest.raises(TypeError):
             is_sequence_of_dicts_uniform([], empty_ok=mistake)
 
-    @pytest.mark.parametrize('data', [
-        [{}, {}],
-        [{'a': 1}, {'a': 2}],
-        [{'b': 1, 'a': 1}, {'a': 2, 'b': 2}],
-    ])
+    @pytest.mark.parametrize(
+        "data",
+        [
+            [{}, {}],
+            [{"a": 1}, {"a": 2}],
+            [{"b": 1, "a": 1}, {"a": 2, "b": 2}],
+        ],
+    )
     def test_True(self, data):
         assert is_sequence_of_dicts_uniform(data)
 
-    @pytest.mark.parametrize('data', [
-        [{'a': 1}, {'b': 2}],
-        [{'a': 1, 'b': 1}, {'b': 2}],
-        {},
-    ])
+    @pytest.mark.parametrize(
+        "data",
+        [
+            [{"a": 1}, {"b": 2}],
+            [{"a": 1, "b": 1}, {"b": 2}],
+            {},
+        ],
+    )
     def test_False(self, data):
         assert not is_sequence_of_dicts_uniform(data)
 
     def test_empty_ok(self):
         assert is_sequence_of_dicts_uniform([], empty_ok=True)
         assert not is_sequence_of_dicts_uniform([], empty_ok=False)
 
 
 class Test_is_sequence_of_sequences:
-    @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+    @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
     def test_precondition_empty_ok(self, mistake):
         with pytest.raises(TypeError):
             is_sequence_of_sequences([], empty_ok=mistake)
 
-    @pytest.mark.parametrize('correct_type', [[[]], [()], ([], ), ((), )])
+    @pytest.mark.parametrize("correct_type", [[[]], [()], ([],), ((),)])
     def test_True(self, correct_type):
         assert is_sequence_of_sequences(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('sequences') + [{'a': []}])
+    @pytest.mark.parametrize("wrong_type", all_types_besides("sequences") + [{"a": []}])
     def test_False(self, wrong_type):
         assert not is_sequence_of_sequences(wrong_type)
 
     def test_empty_ok(self):
         assert is_sequence_of_sequences([], empty_ok=True)
         assert not is_sequence_of_sequences([], empty_ok=False)
 
 
 class Test_is_sequence_of_sequences_uniform:
-    @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+    @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
     def test_precondition_empty_ok(self, mistake):
         with pytest.raises(TypeError):
             is_sequence_of_sequences_uniform([], empty_ok=mistake)
 
-    @pytest.mark.parametrize('data', [
-        [[], []],
+    @pytest.mark.parametrize(
+        "data",
         [
-            ['a', 'b', 'c'],
-            ['x', 'y', 'z'],
-            [1, 2, 3],
-            [True, False, None]
+            [[], []],
+            [["a", "b", "c"], ["x", "y", "z"], [1, 2, 3], [True, False, None]],
         ],
-    ])
+    )
     def test_True(self, data):
         assert is_sequence_of_sequences_uniform(data)
 
-    @pytest.mark.parametrize('data', [
-        [[], [1]],
-        [['a', 'b', 'c'], ['x', 'y']],
-        {},
-    ])
+    @pytest.mark.parametrize(
+        "data",
+        [
+            [[], [1]],
+            [["a", "b", "c"], ["x", "y"]],
+            {},
+        ],
+    )
     def test_False(self, data):
         assert not is_sequence_of_sequences_uniform(data)
 
     def test_empty_ok(self):
         assert is_sequence_of_sequences_uniform([], empty_ok=True)
         assert not is_sequence_of_sequences_uniform([], empty_ok=False)
 
 
 class Test_is_sequence_or_str:
-    @pytest.mark.parametrize('correct_type', all_types(['sequences', 'strings']))
+    @pytest.mark.parametrize("correct_type", all_types(["sequences", "strings"]))
     def test_True(self, correct_type):
         assert is_sequence_or_str(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides(['sequences', 'strings']))
+    @pytest.mark.parametrize("wrong_type", all_types_besides(["sequences", "strings"]))
     def test_False(self, wrong_type):
         assert not is_sequence_or_str(wrong_type)
 
 
 class Test_is_singleton:
-    @pytest.mark.parametrize('correct_type', all_types('singletons'))
+    @pytest.mark.parametrize("correct_type", all_types("singletons"))
     def test_True(self, correct_type):
         assert is_singleton(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('singletons'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("singletons"))
     def test_False(self, wrong_type):
         assert not is_singleton(wrong_type)
 
 
 class Test_is_number:
-    @pytest.mark.parametrize('correct_type', all_types('numbers'))
+    @pytest.mark.parametrize("correct_type", all_types("numbers"))
     def test_True(self, correct_type):
         assert is_number(correct_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('numbers'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("numbers"))
     def test_False(self, wrong_type):
         assert not is_number(wrong_type)
```

### Comparing `katalytic-0.2.2/tests/test_data.py` & `katalytic-0.3.0/tests/test_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,81 @@
 from _decimal import Decimal
+
 from fractions import Fraction
 from pathlib import Path, PosixPath
 
 import pytest
 
 from katalytic.data.checks import (
-    is_generator_function, is_iterator, dicts_share_key_order, dicts_share_value_order, is_equal
+    is_generator_function,
+    is_iterator,
+    dicts_share_key_order,
+    dicts_share_value_order,
+    is_equal,
 )
+
 # noinspection PyProtectedMember
 from katalytic.data import (
-    _C, _C_obj, _callables, _collections, _dict_views, _flatten, _function, _functions, _generators, _iterables,
-    _iterators, _lambda, _numbers, _obj, _objects, _primitives, _sequences, _singletons, _strings, _types, all_types,
-    all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last,
-    last_with_idx, map_dict_keys, map_dict_values, map_recursive, one, pick_all, pick_all_besides, pick_any, pop_max,
-    pop_max_by_dict_key, pop_max_by_dict_value, pop_min, pop_min_by_dict_key, pop_min_by_dict_value, sort_dict_by_keys,
-    sort_dict_by_keys_recursive, sort_dict_by_values, sort_dict_by_values_recursive, as_dict_of_lists, sort_recursive,
-    swap_keys_and_values, xor, xor_with_idx, detect_fronts, detect_fronts_positive, detect_fronts_negative
+    as_list_of_dicts,
+    as_list_of_lists,
+    first,
+    first_with_idx,
+    flatten,
+    flatten_recursive,
+    last,
+    last_with_idx,
+    map_dict_keys,
+    map_dict_values,
+    map_recursive,
+    one,
+    pick_all,
+    pick_all_besides,
+    pick_any,
+    pop_max,
+    pop_max_by_dict_key,
+    pop_max_by_dict_value,
+    pop_min,
+    pop_min_by_dict_key,
+    pop_min_by_dict_value,
+    sort_dict_by_keys,
+    sort_dict_by_keys_recursive,
+    sort_dict_by_values,
+    sort_dict_by_values_recursive,
+    as_dict_of_lists,
+    sort_recursive,
+    swap_keys_and_values,
+    xor,
+    xor_with_idx,
+    detect_fronts,
+    detect_fronts_positive,
+    detect_fronts_negative,
+)
+from katalytic._pkg import (
+    _C,
+    _C_obj,
+    _callables,
+    _collections,
+    _dict_views,
+    _flatten,
+    _function,
+    _functions,
+    _generators,
+    _iterables,
+    _iterators,
+    _lambda,
+    _numbers,
+    _obj,
+    _objects,
+    _primitives,
+    _sequences,
+    _singletons,
+    _strings,
+    _types,
+    all_types,
+    all_types_besides,
 )
 
 
 def _is_list(x):
     return isinstance(x, list)
 
 
@@ -36,1386 +92,1833 @@
 
 
 def _is_str(x):
     return isinstance(x, str)
 
 
 class Test_all_types:
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, object()])
+    @pytest.mark.parametrize("wrong_type", [1, 1.0, True, False, object()])
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             all_types(wrong_type)
 
-    @pytest.mark.parametrize('unexpected', [
-        ['iterable', 'func', 'strong']
-    ])
+    @pytest.mark.parametrize("unexpected", [["iterable", "func", "strong"]])
     def test_unexpected(self, unexpected):
         with pytest.raises(ValueError):
             all_types(unexpected)
 
-    @pytest.mark.parametrize('whitelist, expected', [
-        ('callables', _callables),
-        ('collections', _collections),
-        ('dict_views', _dict_views),
-        ('functions', _functions),
-        ('generators', _generators),
-        ('iterators', _iterators),
-        ('numbers', _numbers),
-        ('objects', _objects),
-        ('primitives', _primitives),
-        ('sequences', _sequences),
-        ('singletons', _singletons),
-        ('strings', _strings),
-        (None, _flatten(_types.values())),
-        (['iterables', 'objects', 'path'], [*_iterables, *_objects, Path('')]),
-        (['iterables'], _iterables),
-    ])
+    @pytest.mark.parametrize(
+        "whitelist, expected",
+        [
+            ("callables", _callables),
+            ("collections", _collections),
+            ("dict_views", _dict_views),
+            ("functions", _functions),
+            ("generators", _generators),
+            ("iterators", _iterators),
+            ("numbers", _numbers),
+            ("objects", _objects),
+            ("primitives", _primitives),
+            ("sequences", _sequences),
+            ("singletons", _singletons),
+            ("strings", _strings),
+            (None, _flatten(_types.values())),
+            (["iterables", "objects", "path"], [*_iterables, *_objects, Path("")]),
+            (["iterables"], _iterables),
+        ],
+    )
     def test_all_types(self, whitelist, expected):
         assert all_types(whitelist) == expected
 
 
 class Test_all_types_besides:
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object()])
+    @pytest.mark.parametrize("wrong_type", [1, 1.0, True, False, None, object()])
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             all_types_besides(wrong_type)
 
-    @pytest.mark.parametrize('unexpected', [
-        ['iterable', 'func', 'strong']
-    ])
+    @pytest.mark.parametrize("unexpected", [["iterable", "func", "strong"]])
     def test_unexpected(self, unexpected):
         with pytest.raises(ValueError):
             all_types_besides(unexpected)
 
-    @pytest.mark.parametrize('blacklist, expected', [
-        (
-            ['iterables'],
-            [
-                True, False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0.0, Fraction(0, 1),
-                0, None, _obj, PosixPath('.'), ''
-            ]
-        ),
-        (
-            'iterables',
-            [
-                True, False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0.0, Fraction(0, 1),
-                0, None, _obj, PosixPath('.'), ''
-            ]
-        ),
-        (
-            ['iterables', 'generators', 'functions', 'objects', 'path'],
-            [True, False, bytearray(b''), b'', _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, '']
-        ),
-    ])
+    @pytest.mark.parametrize(
+        "blacklist, expected",
+        [
+            (
+                ["iterables"],
+                [
+                    True,
+                    False,
+                    bytearray(b""),
+                    b"",
+                    _function,
+                    _lambda,
+                    _C_obj,
+                    _C,
+                    0j,
+                    Decimal("0"),
+                    0.0,
+                    Fraction(0, 1),
+                    0,
+                    None,
+                    _obj,
+                    PosixPath("."),
+                    "",
+                ],
+            ),
+            (
+                "iterables",
+                [
+                    True,
+                    False,
+                    bytearray(b""),
+                    b"",
+                    _function,
+                    _lambda,
+                    _C_obj,
+                    _C,
+                    0j,
+                    Decimal("0"),
+                    0.0,
+                    Fraction(0, 1),
+                    0,
+                    None,
+                    _obj,
+                    PosixPath("."),
+                    "",
+                ],
+            ),
+            (
+                ["iterables", "generators", "functions", "objects", "path"],
+                [
+                    True,
+                    False,
+                    bytearray(b""),
+                    b"",
+                    _C,
+                    0j,
+                    Decimal("0"),
+                    0.0,
+                    Fraction(0, 1),
+                    0,
+                    None,
+                    "",
+                ],
+            ),
+        ],
+    )
     def test_all_types_besides(self, blacklist, expected):
         assert all_types_besides(blacklist) == expected
 
 
 # noinspection PyTypeChecker
 class Test_as_dict_of_lists:
-    @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+    @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
     def test_precondition_empty_ok(self, mistake):
         with pytest.raises(TypeError):
             as_dict_of_lists([], empty_ok=mistake)
 
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object(), iter([]), map(lambda x: x, [])])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [1, 1.0, True, False, None, object(), iter([]), map(lambda x: x, [])],
+    )
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             as_dict_of_lists(wrong_type)
 
-    @pytest.mark.parametrize('data, expected', [
-        # from dict of sequences
-        [
-            {'b': [3, 4], 'a': [1, 2]},
-            {'b': [3, 4], 'a': [1, 2]},
-        ],
+    @pytest.mark.parametrize(
+        "data, expected",
         [
-            {'a': (1, 2), 'b': (3, 4)},
-            {'a': [1, 2], 'b': [3, 4]},
-        ],
-        # from sequence of dicts
-        [
-            ({'a': 1, 'b': 2}, {'b': 4, 'a': 3}),
-            {'a': [1, 3], 'b': [2, 4]},
-        ],
-        [
-            [{'b': 2, 'a': 1}, {'b': 4, 'a': 3}],
-            {'b': [2, 4], 'a': [1, 3]},
-        ],
-        # from sequence of sequences
-        [
-            [['b', 'a'], [1, 2], [3, 4]],
-            {'b': [1, 3], 'a': [2, 4]},
+            # from dict of sequences
+            [
+                {"b": [3, 4], "a": [1, 2]},
+                {"b": [3, 4], "a": [1, 2]},
+            ],
+            [
+                {"a": (1, 2), "b": (3, 4)},
+                {"a": [1, 2], "b": [3, 4]},
+            ],
+            # from sequence of dicts
+            [
+                ({"a": 1, "b": 2}, {"b": 4, "a": 3}),
+                {"a": [1, 3], "b": [2, 4]},
+            ],
+            [
+                [{"b": 2, "a": 1}, {"b": 4, "a": 3}],
+                {"b": [2, 4], "a": [1, 3]},
+            ],
+            # from sequence of sequences
+            [
+                [["b", "a"], [1, 2], [3, 4]],
+                {"b": [1, 3], "a": [2, 4]},
+            ],
+            [
+                (("a", "b"), (1, 2), (3, 4)),
+                {"a": [1, 3], "b": [2, 4]},
+            ],
         ],
-        [
-            (('a', 'b'), (1, 2), (3, 4)),
-            {'a': [1, 3], 'b': [2, 4]},
-        ]
-    ])
+    )
     def test_preserves_key_order_and_converts_seq_to_list(self, data, expected):
         actual = as_dict_of_lists(data)
         assert actual == expected
         # noinspection PyUnresolvedReferences
         assert list(actual.keys()) == list(expected.keys())
 
-    @pytest.mark.parametrize('data', [[], (), {}])
+    @pytest.mark.parametrize("data", [[], (), {}])
     def test_empty_ok(self, data):
         assert as_dict_of_lists(data, empty_ok=True) == []
 
-    @pytest.mark.parametrize('data', [[], (), {}])
+    @pytest.mark.parametrize("data", [[], (), {}])
     def test_empty_ok_False(self, data):
         with pytest.raises(ValueError):
             as_dict_of_lists(data, empty_ok=False)
 
 
 # noinspection PyTypeChecker
 class Test_as_list_of_dicts:
-    @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+    @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
     def test_precondition_empty_ok(self, mistake):
         with pytest.raises(TypeError):
             as_list_of_dicts([], empty_ok=mistake)
 
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object(), iter([]), map(lambda x: x, [])])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [1, 1.0, True, False, None, object(), iter([]), map(lambda x: x, [])],
+    )
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             as_list_of_dicts(wrong_type)
 
     def test_different_keys(self):
-        data = [{'a': 1, 'b': 2}, {'c': 3, 'd': 4, 'e': 5}]
+        data = [{"a": 1, "b": 2}, {"c": 3, "d": 4, "e": 5}]
         with pytest.raises(TypeError):
             as_list_of_dicts(data)
 
-    @pytest.mark.parametrize('data, expected', [
-        # from dict of sequences
+    @pytest.mark.parametrize(
+        "data, expected",
         [
-            {'a': [1, 2], 'b': [3, 4]},
-            [{'a': 1, 'b': 3}, {'a': 2, 'b': 4}],
-        ],
-        [
-            {'b': (3, 4), 'a': (1, 2)},
-            [{'b': 3, 'a': 1}, {'b': 4, 'a': 2}],
-        ],
-        # from sequence of dicts
-        [
-            [{'b': 2, 'a': 1}, {'a': 3, 'b': 4}],
-            [{'b': 2, 'a': 1}, {'b': 4, 'a': 3}],
-        ],
-        [
-            ({'a': 1, 'b': 2}, {'a': 3, 'b': 4}),
-            [{'a': 1, 'b': 2}, {'a': 3, 'b': 4}],
-        ],
-        # from sequence of sequences
-        [
-            [['b', 'a'], [1, 2], [3, 4]],
-            [{'b': 1, 'a': 2}, {'b': 3, 'a': 4}],
-        ],
-        [
-            (['a', 'b'], [1, 2], [3, 4]),
-            [{'a': 1, 'b': 2}, {'a': 3, 'b': 4}],
+            # from dict of sequences
+            [
+                {"a": [1, 2], "b": [3, 4]},
+                [{"a": 1, "b": 3}, {"a": 2, "b": 4}],
+            ],
+            [
+                {"b": (3, 4), "a": (1, 2)},
+                [{"b": 3, "a": 1}, {"b": 4, "a": 2}],
+            ],
+            # from sequence of dicts
+            [
+                [{"b": 2, "a": 1}, {"a": 3, "b": 4}],
+                [{"b": 2, "a": 1}, {"b": 4, "a": 3}],
+            ],
+            [
+                ({"a": 1, "b": 2}, {"a": 3, "b": 4}),
+                [{"a": 1, "b": 2}, {"a": 3, "b": 4}],
+            ],
+            # from sequence of sequences
+            [
+                [["b", "a"], [1, 2], [3, 4]],
+                [{"b": 1, "a": 2}, {"b": 3, "a": 4}],
+            ],
+            [
+                (["a", "b"], [1, 2], [3, 4]),
+                [{"a": 1, "b": 2}, {"a": 3, "b": 4}],
+            ],
         ],
-    ])
+    )
     def test_preserves_key_order_and_converts_seq_to_list(self, data, expected):
         actual = as_list_of_dicts(data)
         keys = list(expected[0].keys())
         assert actual == expected
         assert all(list(d.keys()) == keys for d in actual)
 
-    @pytest.mark.parametrize('data', [[], (), {}])
+    @pytest.mark.parametrize("data", [[], (), {}])
     def test_empty_ok(self, data):
         assert as_list_of_dicts(data, empty_ok=True) == []
 
-    @pytest.mark.parametrize('data', [[], (), {}])
+    @pytest.mark.parametrize("data", [[], (), {}])
     def test_empty_ok_False(self, data):
         with pytest.raises(ValueError):
             as_list_of_dicts(data, empty_ok=False)
 
 
 # noinspection PyTypeChecker
 class Test_as_list_of_lists:
-    @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+    @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
     def test_precondition_empty_ok(self, mistake):
         with pytest.raises(TypeError):
             as_list_of_lists([], empty_ok=mistake)
 
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, object(), iter([]), map(lambda x: x, [])])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [1, 1.0, True, False, None, object(), iter([]), map(lambda x: x, [])],
+    )
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             as_list_of_lists(wrong_type)
 
-    @pytest.mark.parametrize('data, expected', [
-        # from dict of sequences
-        [
-            {'a': [1, 2], 'b': [3, 4]},
-            [['a', 'b'], [1, 3], [2, 4]],
-        ],
+    @pytest.mark.parametrize(
+        "data, expected",
         [
-            {'b': (3, 4), 'a': (1, 2)},
-            [['b', 'a'], [3, 1], [4, 2]],
-        ],
-        # from sequence of dicts
-        [
-            ({'a': 1, 'b': 2}, {'a': 3, 'b': 4}),
-            [['a', 'b'], [1, 2], [3, 4]],
-        ],
-        [
-            [{'b': 2, 'a': 1}, {'a': 3, 'b': 4}],
-            [['b', 'a'], [2, 1], [4, 3]],
-        ],
-        # from sequence of sequences
-        [
-            [['b', 'a'], [1, 2], [3, 4]],
-            [['b', 'a'], [1, 2], [3, 4]],
-        ],
-        [
-            (['a', 'b'], (1, 2), [3, 4]),
-            [['a', 'b'], [1, 2], [3, 4]],
+            # from dict of sequences
+            [
+                {"a": [1, 2], "b": [3, 4]},
+                [["a", "b"], [1, 3], [2, 4]],
+            ],
+            [
+                {"b": (3, 4), "a": (1, 2)},
+                [["b", "a"], [3, 1], [4, 2]],
+            ],
+            # from sequence of dicts
+            [
+                ({"a": 1, "b": 2}, {"a": 3, "b": 4}),
+                [["a", "b"], [1, 2], [3, 4]],
+            ],
+            [
+                [{"b": 2, "a": 1}, {"a": 3, "b": 4}],
+                [["b", "a"], [2, 1], [4, 3]],
+            ],
+            # from sequence of sequences
+            [
+                [["b", "a"], [1, 2], [3, 4]],
+                [["b", "a"], [1, 2], [3, 4]],
+            ],
+            [
+                (["a", "b"], (1, 2), [3, 4]),
+                [["a", "b"], [1, 2], [3, 4]],
+            ],
         ],
-    ])
+    )
     def test_preserves_key_order_and_converts_seq_to_list(self, data, expected):
         assert as_list_of_lists(data) == expected
 
-    @pytest.mark.parametrize('data', [[], (), {}])
+    @pytest.mark.parametrize("data", [[], (), {}])
     def test_empty_ok(self, data):
         assert as_list_of_lists(data, empty_ok=True) == []
 
-    @pytest.mark.parametrize('data', [[], (), {}])
+    @pytest.mark.parametrize("data", [[], (), {}])
     def test_empty_ok_False(self, data):
         with pytest.raises(ValueError):
             as_list_of_lists(data, empty_ok=False)
 
 
 class Test_first:
-    @pytest.mark.parametrize('wrong_type', [
-        iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''
-    ])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [
+            iter([]),
+            map(lambda x: x, []),
+            range(1),
+            object(),
+            [],
+            {},
+            (),
+            set(),
+            1,
+            True,
+            False,
+            None,
+            "",
+        ],
+    )
     def test_key_not_callable(self, wrong_type):
         with pytest.raises(TypeError):
             first([], condition=wrong_type)
 
     def test_sets_are_not_allowed(self):
         with pytest.raises(TypeError):
             first(set())
 
-    @pytest.mark.parametrize('data', [iter([]), map(lambda x: x, []), [], {}, ()])
+    @pytest.mark.parametrize("data", [iter([]), map(lambda x: x, []), [], {}, ()])
     def test_empty(self, data):
         assert first(data) is None
 
     def test_no_first_with_condition(self):
         data = range(10)
         assert first(data, condition=lambda x: x > 50) is None
 
-    @pytest.mark.parametrize('data, expected', [
-        (range(10), 0),
-        ([False, None, 5, True], False),
-        (['', 0, None, False], ''),
-        (map(lambda x: x+1, range(0, 100, 10)), 1),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            (range(10), 0),
+            ([False, None, 5, True], False),
+            (["", 0, None, False], ""),
+            (map(lambda x: x + 1, range(0, 100, 10)), 1),
+        ],
+    )
     def test_first(self, data, expected):
         assert first(data) == expected
 
 
 class Test_first_with_idx:
-    @pytest.mark.parametrize('wrong_type', [
-        iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''
-    ])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [
+            iter([]),
+            map(lambda x: x, []),
+            range(1),
+            object(),
+            [],
+            {},
+            (),
+            set(),
+            1,
+            True,
+            False,
+            None,
+            "",
+        ],
+    )
     def test_key_not_callable(self, wrong_type):
         with pytest.raises(TypeError):
             first_with_idx([], condition=wrong_type)
 
     def test_sets_are_not_allowed(self):
         with pytest.raises(TypeError):
             first_with_idx(set())
 
-    @pytest.mark.parametrize('data', [iter([]), map(lambda x: x, []), [], {}, ()])
+    @pytest.mark.parametrize("data", [iter([]), map(lambda x: x, []), [], {}, ()])
     def test_empty(self, data):
         assert first_with_idx(data) is None
 
     def test_no_first_with_condition(self):
         data = range(10)
         assert first_with_idx(data, condition=lambda x: x > 50) is None
 
     def test_first_with_key(self):
         data = range(5, 15)
         assert first_with_idx(data, condition=lambda x: x >= 10) == (5, 10)
 
-    @pytest.mark.parametrize('data, expected', [
-        (range(10), (0, 0)),
-        ([False, None, 5, True], (0, False)),
-        (['', 0, None, False], (0, '')),
-        (map(lambda x: x+1, range(0, 100, 10)), (0, 1)),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            (range(10), (0, 0)),
+            ([False, None, 5, True], (0, False)),
+            (["", 0, None, False], (0, "")),
+            (map(lambda x: x + 1, range(0, 100, 10)), (0, 1)),
+        ],
+    )
     def test_first(self, data, expected):
         assert first_with_idx(data) == expected
 
 
 class Test_last:
-    @pytest.mark.parametrize('wrong_type', [
-        iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''
-    ])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [
+            iter([]),
+            map(lambda x: x, []),
+            range(1),
+            object(),
+            [],
+            {},
+            (),
+            set(),
+            1,
+            True,
+            False,
+            None,
+            "",
+        ],
+    )
     def test_key_not_callable(self, wrong_type):
         with pytest.raises(TypeError):
             last([], condition=wrong_type)
 
     def test_sets_are_not_allowed(self):
         with pytest.raises(TypeError):
             last(set())
 
-    @pytest.mark.parametrize('data', [iter([]), map(lambda x: x, []), [], {}, ()])
+    @pytest.mark.parametrize("data", [iter([]), map(lambda x: x, []), [], {}, ()])
     def test_empty(self, data):
         assert last(data) is None
 
     def test_no_last_with_condition(self):
         data = range(10)
         assert last(data, condition=lambda x: x > 50) is None
 
-    @pytest.mark.parametrize('data, expected', [
-        (range(10), 9),
-        ([False, None, 5, True], True),
-        ([False, None, True, 5], 5),
-        (['', 0, None, False], False),
-        (map(lambda x: x+1, range(0, 100, 10)), 91),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            (range(10), 9),
+            ([False, None, 5, True], True),
+            ([False, None, True, 5], 5),
+            (["", 0, None, False], False),
+            (map(lambda x: x + 1, range(0, 100, 10)), 91),
+        ],
+    )
     def test_last(self, data, expected):
         assert last(data) == expected
 
 
 class Test_last_with_idx:
-    @pytest.mark.parametrize('wrong_type', [
-        iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''
-    ])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [
+            iter([]),
+            map(lambda x: x, []),
+            range(1),
+            object(),
+            [],
+            {},
+            (),
+            set(),
+            1,
+            True,
+            False,
+            None,
+            "",
+        ],
+    )
     def test_key_not_callable(self, wrong_type):
         with pytest.raises(TypeError):
             last_with_idx([], condition=wrong_type)
 
     def test_sets_are_not_allowed(self):
         with pytest.raises(TypeError):
             last_with_idx(set())
 
-    @pytest.mark.parametrize('data', [iter([]), map(lambda x: x, []), [], {}, ()])
+    @pytest.mark.parametrize("data", [iter([]), map(lambda x: x, []), [], {}, ()])
     def test_empty(self, data):
         assert last_with_idx(data) is None
 
     def test_no_last_with_condition(self):
         data = range(10)
         assert last_with_idx(data, condition=lambda x: x > 50) is None
 
     def test_last_with_key(self):
         data = range(5, 15)
         assert last_with_idx(data, condition=lambda x: x <= 13) == (8, 13)
 
-    @pytest.mark.parametrize('data, expected', [
-        (range(7, 10), (2, 9)),
-        ([False, None, 5, True], (3, True)),
-        (['', 0, None, False], (3, False)),
-        (map(lambda x: x+1, range(0, 100, 10)), (9, 91)),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            (range(7, 10), (2, 9)),
+            ([False, None, 5, True], (3, True)),
+            (["", 0, None, False], (3, False)),
+            (map(lambda x: x + 1, range(0, 100, 10)), (9, 91)),
+        ],
+    )
     def test_last(self, data, expected):
         assert last_with_idx(data) == expected
 
 
 class Test_flatten:
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, '', object()])
+    @pytest.mark.parametrize("wrong_type", [1, 1.0, True, False, None, "", object()])
     def test_should_be_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             flatten(wrong_type)
 
-    @pytest.mark.parametrize('empty', [[], (), {}, set(), iter([])])
+    @pytest.mark.parametrize("empty", [[], (), {}, set(), iter([])])
     def test_empty(self, empty):
         assert flatten(empty) == []
 
-    @pytest.mark.parametrize('data, expected', [
-        ([1, 2, 3], [1, 2, 3]),
-        ((1, 2, 3), [1, 2, 3]),
-        ({1, 2, 3}, [1, 2, 3]),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([1, 2, 3], [1, 2, 3]),
+            ((1, 2, 3), [1, 2, 3]),
+            ({1, 2, 3}, [1, 2, 3]),
+        ],
+    )
     def test_already_flat(self, data, expected):
         assert flatten(data) == expected
 
-    @pytest.mark.parametrize('data, expected', [
-        ((1, [(2, 3), (4, (5, 6))]), [1, (2, 3), (4, (5, 6))]),
-        ([[1, (2, 3), (4, (5, 6))]], [1, (2, 3), (4, (5, 6))]),
-        ({1, (2, 3), (4, (5, 6))}, [1, 2, 3, 4, (5, 6)]),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ((1, [(2, 3), (4, (5, 6))]), [1, (2, 3), (4, (5, 6))]),
+            ([[1, (2, 3), (4, (5, 6))]], [1, (2, 3), (4, (5, 6))]),
+            ({1, (2, 3), (4, (5, 6))}, [1, 2, 3, 4, (5, 6)]),
+        ],
+    )
     def test_flattens_only_one_level(self, data, expected):
         actual = flatten(data)
         if isinstance(data, set):
             actual = set(actual)
             expected = set(expected)
 
         assert actual == expected
 
 
 class Test_flatten_recursive:
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, '', object()])
+    @pytest.mark.parametrize("wrong_type", [1, 1.0, True, False, None, "", object()])
     def test_should_be_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             flatten_recursive(wrong_type)
 
-    @pytest.mark.parametrize('empty', [[], (), {}, set(), iter([])])
+    @pytest.mark.parametrize("empty", [[], (), {}, set(), iter([])])
     def test_empty(self, empty):
         assert flatten_recursive(empty) == []
 
-    @pytest.mark.parametrize('data, expected', [
-        ([1, 2, 3], [1, 2, 3]),
-        ((1, 2, 3), [1, 2, 3]),
-        ({1, 2, 3}, [1, 2, 3]),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([1, 2, 3], [1, 2, 3]),
+            ((1, 2, 3), [1, 2, 3]),
+            ({1, 2, 3}, [1, 2, 3]),
+        ],
+    )
     def test_already_flat(self, data, expected):
         assert flatten_recursive(data) == expected
 
-    @pytest.mark.parametrize('data, expected', [
-        ((1, [(2, 3), (4, (5, 6))]), [1, 2, 3, 4, 5, 6]),
-        ([[1, (2, 3), (4, (5, 6))]], [1, 2, 3, 4, 5, 6]),
-        ({1, (2, 3), (4, (5, 6))}, [1, 2, 3, 4, 5, 6]),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ((1, [(2, 3), (4, (5, 6))]), [1, 2, 3, 4, 5, 6]),
+            ([[1, (2, 3), (4, (5, 6))]], [1, 2, 3, 4, 5, 6]),
+            ({1, (2, 3), (4, (5, 6))}, [1, 2, 3, 4, 5, 6]),
+        ],
+    )
     def test_flattens_all_levels(self, data, expected):
         actual = flatten_recursive(data)
         if isinstance(data, set):
             actual = set(actual)
             expected = set(expected)
 
         assert actual == expected
 
 
 # noinspection PyTypeChecker
 class Test_map_dict_keys:
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, True, None, False, "string", object()]
+    )
     def test_mapping_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             map_dict_keys(wrong_type, {})
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), 1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), 1, 1.0, True, None, False, "string", object()]
+    )
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             map_dict_keys(lambda x: x, wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, True, False, "string", object()]
+    )
     def test_condition_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             map_dict_keys(lambda x: x, {}, condition=wrong_type)
 
     def test_empty(self):
         assert map_dict_keys(lambda x: x, {}) == {}
 
     def test_simple_mapping(self):
-        assert map_dict_keys(str.upper, {'a': 1, 'b': 2}) == {'A': 1, 'B': 2}
+        assert map_dict_keys(str.upper, {"a": 1, "b": 2}) == {"A": 1, "B": 2}
 
     def test_conditioned_mapping(self):
-        data = {'a': 1, (0, 1): 2}
-        expected = {'A': 1, (0, 1): 2}
+        data = {"a": 1, (0, 1): 2}
+        expected = {"A": 1, (0, 1): 2}
         assert map_dict_keys(str.upper, data, condition=_is_str) == expected
 
 
 # noinspection PyTypeChecker
 class Test_map_dict_values:
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, True, None, False, "string", object()]
+    )
     def test_mapping_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             map_dict_values(wrong_type, {})
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), 1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), 1, 1.0, True, None, False, "string", object()]
+    )
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             map_dict_values(lambda x: x, wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, True, False, "string", object()]
+    )
     def test_condition_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             map_dict_values(lambda x: x, {}, condition=wrong_type)
 
     def test_empty(self):
         assert map_dict_values(lambda x: x, {}) == {}
 
     def test_simple_mapping(self):
-        assert map_dict_values(str, {'a': 1, 'b': 2}) == {'a': '1', 'b': '2'}
+        assert map_dict_values(str, {"a": 1, "b": 2}) == {"a": "1", "b": "2"}
 
     def test_conditioned_mapping(self):
-        data = {'a': -1, (0, 1): 1}
-        expected = {'a': '-1', (0, 1): 1}
+        data = {"a": -1, (0, 1): 1}
+        expected = {"a": "-1", (0, 1): 1}
         assert map_dict_values(str, data, condition=_is_negative) == expected
 
 
 class Test_map_recursive:
-    @pytest.mark.xfail(reason='Not implemented')
+    @pytest.mark.xfail(reason="Not implemented")
     def test_condition_is_iterable(self):
         """
         1. Should run both the `if is_iterable()` and the `if condition(x)` branches.
         2. Add another param for which of the two branches to run first"""
         assert 0
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, True, None, False, "string", object()]
+    )
     def test_mapping_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             map_recursive(wrong_type, {})
 
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [1, 1.0, True, None, False, "string", object()]
+    )
     def test_not_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             map_recursive(lambda x: x, wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, True, False, "string", object()]
+    )
     def test_condition_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             map_recursive(lambda x: x, {}, condition=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_on_dict_keys_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             map_recursive(lambda x: x, {}, on_dict_keys=wrong_type)
 
-    @pytest.mark.parametrize('data', [[], (), {}, set()])
+    @pytest.mark.parametrize("data", [[], (), {}, set()])
     def test_empty(self, data):
         assert map_recursive(lambda x: x, data) == data
 
     def test_simple(self):
         assert map_recursive(lambda x: x + 1, [1, 2]) == [2, 3]
         assert map_recursive(lambda x: x + 1, (1, 2)) == (2, 3)
         assert map_recursive(lambda x: x + 1, {1, 2}) == {2, 3}
-        assert map_recursive(lambda x: x + 1, {'a': 1, 'b': 2}) == {'a': 2, 'b': 3}
+        assert map_recursive(lambda x: x + 1, {"a": 1, "b": 2}) == {"a": 2, "b": 3}
 
         actual = map_recursive(lambda x: x + 1, iter([1, 2]))
         assert is_iterator(actual)
         assert tuple(actual) == (2, 3)
 
     def test_deep(self):
-        data = [(1, {'a': 1, 'b': {1, 2}})]
-        expected = [(2, {'a': 2, 'b': {2, 3}})]
+        data = [(1, {"a": 1, "b": {1, 2}})]
+        expected = [(2, {"a": 2, "b": {2, 3}})]
         assert map_recursive(lambda x: x + 1, data) == expected
 
     def test_deep_with_condition(self):
-        data = [(1, 2, {'a': 1, 'b': 2, 'c': {1, (1, 2)}})]
-        expected = [(2, 2, {'a': 2, 'b': 2, 'c': {2, (2, 2)}})]
+        data = [(1, 2, {"a": 1, "b": 2, "c": {1, (1, 2)}})]
+        expected = [(2, 2, {"a": 2, "b": 2, "c": {2, (2, 2)}})]
         assert map_recursive(lambda x: x + 1, data, condition=_is_odd) == expected
 
     def test_deep_with_condition_2(self):
-        data = [1, 2, (1, 2, {'a': 1, 'b': [1, 2]})]
-        expected = (1, 2, (1, 2, {'a': 1, 'b': (1, 2)}))
+        data = [1, 2, (1, 2, {"a": 1, "b": [1, 2]})]
+        expected = (1, 2, (1, 2, {"a": 1, "b": (1, 2)}))
         assert map_recursive(tuple, data, condition=_is_list) == expected
 
     def test_on_dict_keys(self):
-        data = {'a': 1, 'b': {'a': 1, 'b': 2}}
-        expected = {'A': 1, 'B': {'A': 1, 'B': 2}}
-        assert map_recursive(lambda x: x.upper(), data, condition=_is_str, on_dict_keys=True) == expected
+        data = {"a": 1, "b": {"a": 1, "b": 2}}
+        expected = {"A": 1, "B": {"A": 1, "B": 2}}
+        assert (
+            map_recursive(
+                lambda x: x.upper(), data, condition=_is_str, on_dict_keys=True
+            )
+            == expected
+        )
 
     def test_on_dict_keys_iter(self):
-        data = {'a': 1, (1, 2): {'a': 1, (3, 4): 2}}
-        expected = {'a': 2, (2, 3): {'a': 2, (4, 5): 3}}
-        assert map_recursive(lambda x: x + 1, data, condition=_is_num, on_dict_keys=True) == expected
+        data = {"a": 1, (1, 2): {"a": 1, (3, 4): 2}}
+        expected = {"a": 2, (2, 3): {"a": 2, (4, 5): 3}}
+        assert (
+            map_recursive(lambda x: x + 1, data, condition=_is_num, on_dict_keys=True)
+            == expected
+        )
 
 
 class Test_one:
-    @pytest.mark.parametrize('wrong_type', [
-        iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''
-    ])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [
+            iter([]),
+            map(lambda x: x, []),
+            range(1),
+            object(),
+            [],
+            {},
+            (),
+            set(),
+            1,
+            True,
+            False,
+            None,
+            "",
+        ],
+    )
     def test_key_not_callable(self, wrong_type):
         with pytest.raises(TypeError):
             one([], condition=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_key_not_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             one(wrong_type)
 
-    @pytest.mark.parametrize('data', [iter([]), map(lambda x: x, []), [], {}, (), set()])
+    @pytest.mark.parametrize(
+        "data", [iter([]), map(lambda x: x, []), [], {}, (), set()]
+    )
     def test_empty(self, data):
         assert one(data) is None
 
-    @pytest.mark.parametrize('data', [{'', 0, None, False}, ['', 0, None, False]])
+    @pytest.mark.parametrize("data", [{"", 0, None, False}, ["", 0, None, False]])
     def test_no_one(self, data):
-        assert one(data) == ''
+        assert one(data) == ""
 
     def test_no_one_with_condition(self):
         data = range(10)
         assert one(data, condition=lambda x: x > 50) is None
 
-    @pytest.mark.parametrize('data, expected', [
-        (range(10), 0),
-        ([False, None, 5, True], False),
-        ([False, None, True, 5], False),
-        (map(lambda x: x+1, range(0, 100, 10)), 1),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            (range(10), 0),
+            ([False, None, 5, True], False),
+            ([False, None, True, 5], False),
+            (map(lambda x: x + 1, range(0, 100, 10)), 1),
+        ],
+    )
     def test_one(self, data, expected):
         assert one(data) == expected
 
-    @pytest.mark.parametrize('data', [
-        {0, 1, 2, 3},
-        {3, 2, 1, 0},
-    ])
+    @pytest.mark.parametrize(
+        "data",
+        [
+            {0, 1, 2, 3},
+            {3, 2, 1, 0},
+        ],
+    )
     def test_one_of_set(self, data):
         assert one(data) in data
 
 
 class Test_pop_min:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("iterables"))
     def test_not_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pop_min(wrong_type)
 
     def test_dict(self):
         with pytest.raises(TypeError):
             pop_min({})
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("callables"))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             pop_min([1], condition=wrong_type)
 
-    @pytest.mark.parametrize('data', all_types('iterables'))
+    @pytest.mark.parametrize("data", all_types("iterables"))
     def test_empty(self, data):
         if isinstance(data, dict):
             return
         elif is_generator_function(data):
             # noinspection PyCallingNonCallable
             data = data()
             next(data)
 
         with pytest.raises(ValueError):
             pop_min(data)
 
-    @pytest.mark.parametrize('data, expected', [
-        ([3,2,1,4], (1, [3,2,4])),
-        ((0,-1,3,4), (-1, (0,3,4))),
-        (map(float, (0,3,-4,5)), (-4, [0,3,5])),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([3, 2, 1, 4], (1, [3, 2, 4])),
+            ((0, -1, 3, 4), (-1, (0, 3, 4))),
+            (map(float, (0, 3, -4, 5)), (-4, [0, 3, 5])),
+        ],
+    )
     def test_no_key(self, data, expected):
         assert pop_min(data) == expected
 
-    @pytest.mark.parametrize('data, expected', [
-        ([3,2,1,4], (4, [3,2,1])),
-        ((0,-1,3,4), (4, (0,-1,3))),
-        (map(float, (0,3,-4,5)), (5, [0,3,-4])),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([3, 2, 1, 4], (4, [3, 2, 1])),
+            ((0, -1, 3, 4), (4, (0, -1, 3))),
+            (map(float, (0, 3, -4, 5)), (5, [0, 3, -4])),
+        ],
+    )
     def test_with_key(self, data, expected):
         assert pop_min(data, condition=lambda x: -x) == expected
 
 
 class Test_pop_max:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("iterables"))
     def test_not_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pop_max(wrong_type)
 
     def test_dict(self):
         with pytest.raises(TypeError):
             pop_max({})
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("callables"))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             pop_max([1], condition=wrong_type)
 
-    @pytest.mark.parametrize('data', all_types('iterables'))
+    @pytest.mark.parametrize("data", all_types("iterables"))
     def test_empty(self, data):
         if isinstance(data, dict):
             return
         elif is_generator_function(data):
             # noinspection PyCallingNonCallable
             data = data()
             next(data)
 
         with pytest.raises(ValueError):
             pop_max(data)
 
-    @pytest.mark.parametrize('data, expected', [
-        ([3,2,1,4], (4, [3,2,1])),
-        ((0,-1,3,4), (4, (0,-1,3))),
-        (map(float, (0,3,-4,5)), (5, [0,3,-4])),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([3, 2, 1, 4], (4, [3, 2, 1])),
+            ((0, -1, 3, 4), (4, (0, -1, 3))),
+            (map(float, (0, 3, -4, 5)), (5, [0, 3, -4])),
+        ],
+    )
     def test_no_key(self, data, expected):
         assert pop_max(data) == expected
 
-    @pytest.mark.parametrize('data, expected', [
-        ([3,2,1,4], (1, [3,2,4])),
-        ({0,-1,3,4}, (-1, {0,3,4})),
-        (map(float, (0,3,-4,5)), (-4, [0,3,5])),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([3, 2, 1, 4], (1, [3, 2, 4])),
+            ({0, -1, 3, 4}, (-1, {0, 3, 4})),
+            (map(float, (0, 3, -4, 5)), (-4, [0, 3, 5])),
+        ],
+    )
     def test_with_key(self, data, expected):
         assert pop_max(data, condition=lambda x: -x) == expected
 
 
 class Test_pop_max_by_dict_key:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("dict"))
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             pop_max_by_dict_key(wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("callables"))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            pop_max_by_dict_key({'1': 1}, condition=wrong_type)
+            pop_max_by_dict_key({"1": 1}, condition=wrong_type)
 
     def test_empty(self):
         with pytest.raises(ValueError):
             pop_max_by_dict_key({})
 
-    @pytest.mark.parametrize('data, expected', [
-        ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('d', 4), {'a': 3, 'b': 2, 'c': 1})),
-        ({'a': 0, 'b': -1, 'c': 4, 'd': 3}, (('d', 3), {'a': 0, 'b': -1, 'c': 4})),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ({"a": 3, "b": 2, "c": 1, "d": 4}, (("d", 4), {"a": 3, "b": 2, "c": 1})),
+            ({"a": 0, "b": -1, "c": 4, "d": 3}, (("d", 3), {"a": 0, "b": -1, "c": 4})),
+        ],
+    )
     def test_no_key(self, data, expected):
         assert pop_max_by_dict_key(data) == expected
 
-    @pytest.mark.parametrize('data, expected', [
-        ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((1, 'c'), {3: 'a', 2: 'b', 4: 'd'})),
-        ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((-1, 'b'), {0: 'a', 4: 'c', 3: 'd'})),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ({3: "a", 2: "b", 1: "c", 4: "d"}, ((1, "c"), {3: "a", 2: "b", 4: "d"})),
+            ({0: "a", -1: "b", 4: "c", 3: "d"}, ((-1, "b"), {0: "a", 4: "c", 3: "d"})),
+        ],
+    )
     def test_with_key(self, data, expected):
         assert pop_max_by_dict_key(data, condition=lambda x: -x) == expected
 
 
 class Test_pop_min_by_dict_key:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("dict"))
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             pop_min_by_dict_key(wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("callables"))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            pop_min_by_dict_key({'1': 1}, condition=wrong_type)
+            pop_min_by_dict_key({"1": 1}, condition=wrong_type)
 
     def test_empty(self):
         with pytest.raises(ValueError):
             pop_min_by_dict_key({})
 
-    @pytest.mark.parametrize('data, expected', [
-        ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('a', 3), {'b': 2, 'c': 1, 'd': 4})),
-        ({'a': 0, 'b': -1, 'c': 4, 'd': 3}, (('a', 0), {'b': -1, 'c': 4, 'd': 3})),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ({"a": 3, "b": 2, "c": 1, "d": 4}, (("a", 3), {"b": 2, "c": 1, "d": 4})),
+            ({"a": 0, "b": -1, "c": 4, "d": 3}, (("a", 0), {"b": -1, "c": 4, "d": 3})),
+        ],
+    )
     def test_no_key(self, data, expected):
         assert pop_min_by_dict_key(data) == expected
 
-    @pytest.mark.parametrize('data, expected', [
-        ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((4, 'd'), {3: 'a', 2: 'b', 1: 'c'})),
-        ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((4, 'c'), {0: 'a', -1: 'b', 3: 'd'})),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ({3: "a", 2: "b", 1: "c", 4: "d"}, ((4, "d"), {3: "a", 2: "b", 1: "c"})),
+            ({0: "a", -1: "b", 4: "c", 3: "d"}, ((4, "c"), {0: "a", -1: "b", 3: "d"})),
+        ],
+    )
     def test_with_key(self, data, expected):
         assert pop_min_by_dict_key(data, condition=lambda x: -x) == expected
 
 
 class Test_pop_max_by_dict_value:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("dict"))
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             pop_max_by_dict_value(wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("callables"))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            pop_max_by_dict_value({'1': 1}, condition=wrong_type)
+            pop_max_by_dict_value({"1": 1}, condition=wrong_type)
 
     def test_empty(self):
         with pytest.raises(ValueError):
             pop_max_by_dict_value({})
 
-    @pytest.mark.parametrize('data, expected', [
-        ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('d', 4), {'a': 3, 'b': 2, 'c': 1})),
-        ({'a': 0, 'b': -1, 'c': 4, 'd': 3}, (('c', 4), {'a': 0, 'b': -1, 'd': 3})),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ({"a": 3, "b": 2, "c": 1, "d": 4}, (("d", 4), {"a": 3, "b": 2, "c": 1})),
+            ({"a": 0, "b": -1, "c": 4, "d": 3}, (("c", 4), {"a": 0, "b": -1, "d": 3})),
+        ],
+    )
     def test_no_key(self, data, expected):
         assert pop_max_by_dict_value(data) == expected
 
-    @pytest.mark.parametrize('data, expected', [
-        ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((3, 'a'), {2: 'b', 1: 'c', 4: 'd'})),
-        ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((0, 'a'), {-1: 'b', 4: 'c', 3: 'd'})),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ({3: "a", 2: "b", 1: "c", 4: "d"}, ((3, "a"), {2: "b", 1: "c", 4: "d"})),
+            ({0: "a", -1: "b", 4: "c", 3: "d"}, ((0, "a"), {-1: "b", 4: "c", 3: "d"})),
+        ],
+    )
     def test_with_key(self, data, expected):
         assert pop_max_by_dict_value(data, condition=lambda x: -ord(x)) == expected
 
 
 class Test_pop_min_by_dict_value:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("dict"))
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             pop_min_by_dict_value(wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("callables"))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            pop_min_by_dict_value({'1': 1}, condition=wrong_type)
+            pop_min_by_dict_value({"1": 1}, condition=wrong_type)
 
     def test_empty(self):
         with pytest.raises(ValueError):
             pop_min_by_dict_value({})
 
-    @pytest.mark.parametrize('data, expected', [
-        ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('c', 1), {'a': 3, 'b': 2, 'd': 4})),
-        ({'a': 0, 'b': -1, 'c': 4, 'd': 3}, (('b', -1), {'a': 0, 'c': 4, 'd': 3})),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ({"a": 3, "b": 2, "c": 1, "d": 4}, (("c", 1), {"a": 3, "b": 2, "d": 4})),
+            ({"a": 0, "b": -1, "c": 4, "d": 3}, (("b", -1), {"a": 0, "c": 4, "d": 3})),
+        ],
+    )
     def test_no_key(self, data, expected):
         assert pop_min_by_dict_value(data) == expected
 
-    @pytest.mark.parametrize('data, expected', [
-        ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((4, 'd'), {3: 'a', 2: 'b', 1: 'c'})),
-        ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((3, 'd'), {0: 'a', -1: 'b', 4: 'c'})),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ({3: "a", 2: "b", 1: "c", 4: "d"}, ((4, "d"), {3: "a", 2: "b", 1: "c"})),
+            ({0: "a", -1: "b", 4: "c", 3: "d"}, ((3, "d"), {0: "a", -1: "b", 4: "c"})),
+        ],
+    )
     def test_with_key(self, data, expected):
         assert pop_min_by_dict_value(data, condition=lambda x: -ord(x)) == expected
 
 
 class Test_pick_all:
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_needles_should_be_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pick_all(wrong_type, [])
 
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_haystack_should_be_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pick_all([], wrong_type)
 
-    @pytest.mark.parametrize('needles, haystack, expected', [
-        ([], [], []),
-        ((), {}, []),
-        ((), [1], []),
-        ((1, ), [], []),
-    ])
+    @pytest.mark.parametrize(
+        "needles, haystack, expected",
+        [
+            ([], [], []),
+            ((), {}, []),
+            ((), [1], []),
+            ((1,), [], []),
+        ],
+    )
     def test_empty(self, needles, haystack, expected):
         assert pick_all(needles, haystack) == expected
 
-    @pytest.mark.parametrize('needles, haystack, expected', [
-        ([1, 2], [3, 4], []),
-        ([0, True], (1, False), []),
-    ])
+    @pytest.mark.parametrize(
+        "needles, haystack, expected",
+        [
+            ([1, 2], [3, 4], []),
+            ([0, True], (1, False), []),
+        ],
+    )
     def test_no_match(self, needles, haystack, expected):
         assert pick_all(needles, haystack) == expected
 
-    @pytest.mark.parametrize('needles, haystack, expected', [
-        ([1, 2, 3], [2, 3, 4], [2, 3]),
-        ([False, True, None], {True, None}, [True, None]),
-    ])
+    @pytest.mark.parametrize(
+        "needles, haystack, expected",
+        [
+            ([1, 2, 3], [2, 3, 4], [2, 3]),
+            ([False, True, None], {True, None}, [True, None]),
+        ],
+    )
     def test_match(self, needles, haystack, expected):
         assert pick_all(needles, haystack) == expected
 
 
 class Test_pick_all_besides:
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_needles_should_be_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pick_all_besides(wrong_type, [])
 
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_haystack_should_be_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pick_all_besides([], wrong_type)
 
-    @pytest.mark.parametrize('needles, haystack, expected', [
-        ([], [], []),
-        ((), {}, []),
-    ])
+    @pytest.mark.parametrize(
+        "needles, haystack, expected",
+        [
+            ([], [], []),
+            ((), {}, []),
+        ],
+    )
     def test_empty(self, needles, haystack, expected):
         assert pick_all_besides(needles, haystack) == expected
 
-    @pytest.mark.parametrize('needles, haystack, expected', [
-        ([1, 2, 3], [3, 4, 5], [1, 2]),
-        ([0, True, None], {1, False, None}, [0, True]),
-    ])
+    @pytest.mark.parametrize(
+        "needles, haystack, expected",
+        [
+            ([1, 2, 3], [3, 4, 5], [1, 2]),
+            ([0, True, None], {1, False, None}, [0, True]),
+        ],
+    )
     def test_match(self, needles, haystack, expected):
         assert pick_all_besides(needles, haystack) == expected
 
-    @pytest.mark.parametrize('needles, haystack, expected', [
-        ([1, 2, 3], [1, 2, 3], []),
-        ([False, True, None], {False, True, None}, []),
-    ])
+    @pytest.mark.parametrize(
+        "needles, haystack, expected",
+        [
+            ([1, 2, 3], [1, 2, 3], []),
+            ([False, True, None], {False, True, None}, []),
+        ],
+    )
     def test_no_match(self, needles, haystack, expected):
         assert pick_all_besides(needles, haystack) == expected
 
 
 class Test_pick_any:
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_needles_should_be_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pick_any(wrong_type, [])
 
-    @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
+    @pytest.mark.parametrize("wrong_type", [object(), 1, True, False, None, ""])
     def test_haystack_should_be_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pick_any([], wrong_type)
 
-    @pytest.mark.parametrize('needles, haystack, expected', [
-        ([], [], None),
-        ((), {}, None),
-        ((), [1], None),
-        ((1, ), [], None),
-    ])
+    @pytest.mark.parametrize(
+        "needles, haystack, expected",
+        [
+            ([], [], None),
+            ((), {}, None),
+            ((), [1], None),
+            ((1,), [], None),
+        ],
+    )
     def test_empty(self, needles, haystack, expected):
         assert pick_any(needles, haystack) == expected
 
-    @pytest.mark.parametrize('needles, haystack, expected', [
-        ([1, 2], [3, 4], None),
-        ([0, True], {1, False}, None),
-    ])
+    @pytest.mark.parametrize(
+        "needles, haystack, expected",
+        [
+            ([1, 2], [3, 4], None),
+            ([0, True], {1, False}, None),
+        ],
+    )
     def test_no_match(self, needles, haystack, expected):
         assert pick_any(needles, haystack) == expected
 
-    @pytest.mark.parametrize('needles, haystack, expected', [
-        ([1, 2, 3], [2, 3, 4], 2),
-        ([False, True, None], {None, True}, True),
-    ])
+    @pytest.mark.parametrize(
+        "needles, haystack, expected",
+        [
+            ([1, 2, 3], [2, 3, 4], 2),
+            ([False, True, None], {None, True}, True),
+        ],
+    )
     def test_match(self, needles, haystack, expected):
         assert pick_any(needles, haystack) == expected
 
 
 class Test_sort_dict_by_keys:
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), 1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), 1, 1.0, True, None, False, "string", object()]
+    )
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_keys(wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, True, False, "string", object()]
+    )
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_keys({}, condition=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_not_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_keys({}, reverse=wrong_type)
 
     def test_empty(self):
         assert sort_dict_by_keys({}) == {}
 
     def test_simple(self):
-        actual = sort_dict_by_keys({'b': 2, 'c': 1, 'a': 3})
-        expected = {'a': 3, 'b': 2, 'c': 1}
+        actual = sort_dict_by_keys({"b": 2, "c": 1, "a": 3})
+        expected = {"a": 3, "b": 2, "c": 1}
         assert actual == expected
         assert dicts_share_key_order(actual, expected)
 
     def test_with_key(self):
-        actual = sort_dict_by_keys({'qwerty': 1, 'x': 3, 'asd': 2}, condition=len)
-        expected = {'x': 3, 'asd': 2, 'qwerty': 1}
+        actual = sort_dict_by_keys({"qwerty": 1, "x": 3, "asd": 2}, condition=len)
+        expected = {"x": 3, "asd": 2, "qwerty": 1}
         assert actual == expected
         assert dicts_share_key_order(actual, expected)
 
     def test_reversed(self):
-        actual = sort_dict_by_keys({'b': 2, 'c': 1, 'a': 3}, reverse=True)
-        expected = {'c': 1, 'b': 2, 'a': 3}
+        actual = sort_dict_by_keys({"b": 2, "c": 1, "a": 3}, reverse=True)
+        expected = {"c": 1, "b": 2, "a": 3}
         assert actual == expected
         assert dicts_share_key_order(actual, expected)
 
     def test_with_key_and_reversed(self):
-        actual = sort_dict_by_keys({'qwerty': 1, 'x': 3, 'asd': 2}, condition=len, reverse=True)
-        expected = {'qwerty': 1, 'asd': 2, 'x': 3}
+        actual = sort_dict_by_keys(
+            {"qwerty": 1, "x": 3, "asd": 2}, condition=len, reverse=True
+        )
+        expected = {"qwerty": 1, "asd": 2, "x": 3}
         assert actual == expected
         assert dicts_share_key_order(actual, expected)
 
 
 class Test_sort_dict_by_values:
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), 1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), 1, 1.0, True, None, False, "string", object()]
+    )
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_values(wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, True, False, "string", object()]
+    )
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_values({}, condition=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_not_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_values({}, reverse=wrong_type)
 
     def test_empty(self):
         assert sort_dict_by_values({}) == {}
 
     def test_simple(self):
-        actual = sort_dict_by_values({'b': 2, 'c': 1, 'a': 3})
-        expected = {'c': 1, 'b': 2, 'a': 3}
+        actual = sort_dict_by_values({"b": 2, "c": 1, "a": 3})
+        expected = {"c": 1, "b": 2, "a": 3}
         assert actual == expected
         assert dicts_share_value_order(actual, expected)
 
     def test_with_key(self):
-        actual = sort_dict_by_values({'qwerty': 1, 'x': 3, 'asd': -2}, condition=abs)
-        expected = {'qwerty': 1, 'asd': -2, 'x': 3}
+        actual = sort_dict_by_values({"qwerty": 1, "x": 3, "asd": -2}, condition=abs)
+        expected = {"qwerty": 1, "asd": -2, "x": 3}
         assert actual == expected
         assert dicts_share_value_order(actual, expected)
 
     def test_reversed(self):
-        actual = sort_dict_by_values({'b': 2, 'c': 1, 'a': 3}, reverse=True)
-        expected = {'a': 3, 'b': 2, 'c': 1}
+        actual = sort_dict_by_values({"b": 2, "c": 1, "a": 3}, reverse=True)
+        expected = {"a": 3, "b": 2, "c": 1}
         assert actual == expected
         assert dicts_share_value_order(actual, expected)
 
     def test_with_key_and_reversed(self):
-        actual = sort_dict_by_values({'qwerty': 1, 'x': 3, 'asd': -2}, condition=abs, reverse=True)
-        expected = {'x': 3, 'asd': -2, 'qwerty': 1}
+        actual = sort_dict_by_values(
+            {"qwerty": 1, "x": 3, "asd": -2}, condition=abs, reverse=True
+        )
+        expected = {"x": 3, "asd": -2, "qwerty": 1}
         assert actual == expected
         assert dicts_share_value_order(actual, expected)
 
 
 # noinspection PyTypeChecker
 class Test_sort_dict_by_keys_recursive:
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [1, 1.0, True, None, False, "string", object()]
+    )
     def test_not_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_keys_recursive(wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, True, False, "string", object()]
+    )
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_keys_recursive({}, condition=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_not_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_keys_recursive({}, reverse=wrong_type)
 
     def test_empty(self):
         assert sort_dict_by_keys_recursive({}) == {}
 
-    @pytest.mark.parametrize('data, expected', [
-        [{'x': 1, 'a': 2}, {'a': 2, 'x': 1}],
-        [{'a': 2, 'x': 1}, {'a': 2, 'x': 1}],
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            [{"x": 1, "a": 2}, {"a": 2, "x": 1}],
+            [{"a": 2, "x": 1}, {"a": 2, "x": 1}],
+        ],
+    )
     def test_simple(self, data, expected):
         actual = sort_dict_by_keys_recursive(data)
         assert actual == expected
         assert dicts_share_key_order(actual, expected, recursive=True)
 
-    @pytest.mark.parametrize('data, expected', [
-        [
-            [{'x': 1, 'a': 2}, map(lambda x: x, (2, 1, {'x': 1, 'a': {'z': 1, 'y': 2}}))],
-            [{'a': 2, 'x': 1}, (2, 1, {'a': {'y': 2, 'z': 1}, 'x': 1})],
-        ],
+    @pytest.mark.parametrize(
+        "data, expected",
         [
-            [{'a': 2, 'x': 1}, map(lambda x: x, (2, 1, {'a': {'y': 2, 'z': 1}, 'x': 1}))],
-            [{'a': 2, 'x': 1}, (2, 1, {'a': {'y': 2, 'z': 1}, 'x': 1})],
+            [
+                [
+                    {"x": 1, "a": 2},
+                    map(lambda x: x, (2, 1, {"x": 1, "a": {"z": 1, "y": 2}})),
+                ],
+                [{"a": 2, "x": 1}, (2, 1, {"a": {"y": 2, "z": 1}, "x": 1})],
+            ],
+            [
+                [
+                    {"a": 2, "x": 1},
+                    map(lambda x: x, (2, 1, {"a": {"y": 2, "z": 1}, "x": 1})),
+                ],
+                [{"a": 2, "x": 1}, (2, 1, {"a": {"y": 2, "z": 1}, "x": 1})],
+            ],
         ],
-    ])
+    )
     def test_recursive(self, data, expected):
         actual = sort_dict_by_keys_recursive(data)
         actual[1] = tuple(actual[1])
         assert actual == expected
         assert dicts_share_key_order(actual, expected, recursive=True)
 
-    @pytest.mark.parametrize('data, expected', [
+    @pytest.mark.parametrize(
+        "data, expected",
         [
-            [{'x': 1, 'a': 2}, map(lambda x: x, (2, 1, {'x': 1, 'a': {'z': 1, 'y': 2}}))],
-            [{'x': 1, 'a': 2}, (2, 1, {'x': 1, 'a': {'y': 2, 'z': 1}})],
-        ],
-        [
-            [{'a': 2, 'x': 1}, map(lambda x: x, (2, 1, {'a': {'y': 2, 'z': 1}, 'x': 1}))],
-            [{'x': 1, 'a': 2}, (2, 1, {'x': 1, 'a': {'y': 2, 'z': 1}})],
+            [
+                [
+                    {"x": 1, "a": 2},
+                    map(lambda x: x, (2, 1, {"x": 1, "a": {"z": 1, "y": 2}})),
+                ],
+                [{"x": 1, "a": 2}, (2, 1, {"x": 1, "a": {"y": 2, "z": 1}})],
+            ],
+            [
+                [
+                    {"a": 2, "x": 1},
+                    map(lambda x: x, (2, 1, {"a": {"y": 2, "z": 1}, "x": 1})),
+                ],
+                [{"x": 1, "a": 2}, (2, 1, {"x": 1, "a": {"y": 2, "z": 1}})],
+            ],
         ],
-    ])
+    )
     def test_recursive_with_key(self, data, expected):
         def condition(k):
-            if k in ['x', 'y']:
+            if k in ["x", "y"]:
                 return 0
             else:
                 return ord(k)
 
         actual = sort_dict_by_keys_recursive(data, condition=condition)
         actual[1] = tuple(actual[1])
         assert actual == expected
         assert dicts_share_key_order(actual, expected, recursive=True)
 
-    @pytest.mark.parametrize('data, expected', [
-        [
-            [{'x': 1, 'a': 2}, map(lambda x: x, (2, 1, {'x': 1, 'a': {'z': 1, 'y': 2}}))],
-            [{'x': 1, 'a': 2}, (2, 1, {'x': 1, 'a': {'z': 1, 'y': 2}})],
-        ],
+    @pytest.mark.parametrize(
+        "data, expected",
         [
-            [{'a': 2, 'x': 1}, map(lambda x: x, (2, 1, {'a': {'y': 2, 'z': 1}, 'x': 1}))],
-            [{'x': 1, 'a': 2}, (2, 1, {'x': 1, 'a': {'z': 1, 'y': 2}})],
+            [
+                [
+                    {"x": 1, "a": 2},
+                    map(lambda x: x, (2, 1, {"x": 1, "a": {"z": 1, "y": 2}})),
+                ],
+                [{"x": 1, "a": 2}, (2, 1, {"x": 1, "a": {"z": 1, "y": 2}})],
+            ],
+            [
+                [
+                    {"a": 2, "x": 1},
+                    map(lambda x: x, (2, 1, {"a": {"y": 2, "z": 1}, "x": 1})),
+                ],
+                [{"x": 1, "a": 2}, (2, 1, {"x": 1, "a": {"z": 1, "y": 2}})],
+            ],
         ],
-    ])
+    )
     def test_recursive_reversed(self, data, expected):
         actual = sort_dict_by_keys_recursive(data, reverse=True)
         actual[1] = tuple(actual[1])
         assert actual == expected
         assert dicts_share_key_order(actual, expected, recursive=True)
 
 
 # noinspection PyTypeChecker
 class Test_sort_dict_by_values_recursive:
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [1, 1.0, True, None, False, "string", object()]
+    )
     def test_not_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_values_recursive(wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, True, False, "string", object()]
+    )
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_values_recursive({}, condition=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_not_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_values_recursive({}, reverse=wrong_type)
 
     def test_empty(self):
         assert sort_dict_by_values_recursive({}) == {}
 
     def test_simple(self):
-        actual = sort_dict_by_values_recursive({'x': 2, 'a': 1})
-        expected = {'a': 1, 'x': 2}
+        actual = sort_dict_by_values_recursive({"x": 2, "a": 1})
+        expected = {"a": 1, "x": 2}
         assert actual == expected
         assert dicts_share_value_order(actual, expected, recursive=True)
 
-    @pytest.mark.parametrize('data, expected', [
-        [
-            [{'a': 2, 'b': 1}, map(lambda x: x, (2, 1, {'a': 2, 'b': 1}))],
-            [{'b': 1, 'a': 2}, (2, 1, {'b': 1, 'a': 2})],
-        ],
+    @pytest.mark.parametrize(
+        "data, expected",
         [
-            [{'b': 1, 'a': 2}, map(lambda x: x, (2, 1, {'b': 1, 'a': 2}))],
-            [{'b': 1, 'a': 2}, (2, 1, {'b': 1, 'a': 2})],
+            [
+                [{"a": 2, "b": 1}, map(lambda x: x, (2, 1, {"a": 2, "b": 1}))],
+                [{"b": 1, "a": 2}, (2, 1, {"b": 1, "a": 2})],
+            ],
+            [
+                [{"b": 1, "a": 2}, map(lambda x: x, (2, 1, {"b": 1, "a": 2}))],
+                [{"b": 1, "a": 2}, (2, 1, {"b": 1, "a": 2})],
+            ],
         ],
-    ])
+    )
     def test_recursive(self, data, expected):
         actual = sort_dict_by_values_recursive(data)
         actual[1] = tuple(actual[1])
         assert actual == expected
         assert dicts_share_value_order(actual, expected, recursive=True)
 
 
 class Test_sort_recursive:
-    @pytest.mark.parametrize('wrong_type', [1, 1.0, True, None, False, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [1, 1.0, True, None, False, "string", object()]
+    )
     def test_data_should_be_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             sort_recursive(wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [
-        iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''
-    ])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [
+            iter([]),
+            map(lambda x: x, []),
+            range(1),
+            object(),
+            [],
+            {},
+            (),
+            set(),
+            1,
+            True,
+            False,
+            None,
+            "",
+        ],
+    )
     def test_key_should_be_callable(self, wrong_type):
         with pytest.raises(TypeError):
             sort_recursive([], condition=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_reverse_should_be_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_recursive({}, reverse=wrong_type)
 
-    @pytest.mark.parametrize('wrong_value', [[], set(), (), {}, 1, 1.0, 'string', object(), True, False])
+    @pytest.mark.parametrize(
+        "wrong_value", [[], set(), (), {}, 1, 1.0, "string", object(), True, False]
+    )
     def test_sort_dicts_by_be_keys_values_or_None(self, wrong_value):
         with pytest.raises(ValueError):
             sort_recursive({}, sort_dicts_by=wrong_value)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_sort_iters_should_be_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_recursive({}, sort_iters=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_sort_lists_should_be_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_recursive({}, sort_lists=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_sort_sets_should_be_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_recursive({}, sort_sets=wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
+    @pytest.mark.parametrize(
+        "wrong_type", [[], set(), (), {}, 1, 1.0, None, "string", object()]
+    )
     def test_sort_tuples_should_be_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_recursive({}, sort_tuples=wrong_type)
 
-    @pytest.mark.parametrize('data, expected', [
-        ([], []),
-        ((), ()),
-        ({}, {}),
-        (set(), []),
-        (iter([]), []),
-        (map(bool, []), []),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([], []),
+            ((), ()),
+            ({}, {}),
+            (set(), []),
+            (iter([]), []),
+            (map(bool, []), []),
+        ],
+    )
     def test_sort_empty(self, data, expected):
         assert sort_recursive(data) == expected
 
-    @pytest.mark.parametrize('data', [
-        [],
-        (),
-        {},
-        set(),
-        iter([]),
-        map(bool, []),
-    ])
+    @pytest.mark.parametrize(
+        "data",
+        [
+            [],
+            (),
+            {},
+            set(),
+            iter([]),
+            map(bool, []),
+        ],
+    )
     def test_returns_same_type_if_possible(self, data):
         if isinstance(data, (list, tuple, dict)):
             assert isinstance(sort_recursive(data), type(data))
         elif isinstance(data, set) or is_iterator(data):
             assert isinstance(sort_recursive(data), list)
 
-    @pytest.mark.parametrize('data, expected', [
-        ([3, 2, 1], [1, 2, 3]),
-        ((3, 2, 1), (1, 2, 3)),
-        ({3: 'x', 2: 'x', 1: 'x'}, {1: 'x', 2: 'x', 3: 'x'}),
-        ({3, 2, 1}, [1, 2, 3]),
-        (iter([3, 2, 1]), [1, 2, 3]),
-        (map(bool, [2, 0, 1]), [False, True, True]),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([3, 2, 1], [1, 2, 3]),
+            ((3, 2, 1), (1, 2, 3)),
+            ({3: "x", 2: "x", 1: "x"}, {1: "x", 2: "x", 3: "x"}),
+            ({3, 2, 1}, [1, 2, 3]),
+            (iter([3, 2, 1]), [1, 2, 3]),
+            (map(bool, [2, 0, 1]), [False, True, True]),
+        ],
+    )
     def test_sort_simple(self, data, expected):
         assert sort_recursive(data) == expected
 
-    @pytest.mark.parametrize('kwargs, expected', [
-        ({'data': [3, 2, 1], 'sort_lists': False}, [3, 2, 1]),
-        ({'data': (3, 2, 1), 'sort_tuples': False}, (3, 2, 1)),
-        ({'data': {3: 'x', 2: 'x', 1: 'x'}, 'sort_dicts_by': None}, {3: 'x', 2: 'x', 1: 'x'}),
-        ({'data': {3, 2, 1}, 'sort_sets': False}, {3, 2, 1}),
-        ({'data': iter([3, 2, 1]), 'sort_iters': False}, iter([3, 2, 1])),
-        ({'data': map(bool, [2, 0, 1]), 'sort_iters': False}, map(bool, [2, 0, 1])),
-    ])
+    @pytest.mark.parametrize(
+        "kwargs, expected",
+        [
+            ({"data": [3, 2, 1], "sort_lists": False}, [3, 2, 1]),
+            ({"data": (3, 2, 1), "sort_tuples": False}, (3, 2, 1)),
+            (
+                {"data": {3: "x", 2: "x", 1: "x"}, "sort_dicts_by": None},
+                {3: "x", 2: "x", 1: "x"},
+            ),
+            ({"data": {3, 2, 1}, "sort_sets": False}, {3, 2, 1}),
+            ({"data": iter([3, 2, 1]), "sort_iters": False}, iter([3, 2, 1])),
+            ({"data": map(bool, [2, 0, 1]), "sort_iters": False}, map(bool, [2, 0, 1])),
+        ],
+    )
     def test_type_remains_unchanged_when_not_sorting(self, kwargs, expected):
         actual = sort_recursive(**kwargs)
 
-        if is_iterator(kwargs['data']):
+        if is_iterator(kwargs["data"]):
             assert is_iterator(actual)
             assert list(actual) == list(expected)
         else:
-            assert isinstance(actual, type(kwargs['data']))
+            assert isinstance(actual, type(kwargs["data"]))
             assert actual == expected
 
-    @pytest.mark.parametrize('kwargs, expected', [
-        ({'data': [(3,5), (4,2), (6, 1)], 'sort_lists': False}, [(3, 5), (2, 4), (1, 6)]),
-        ({'data': ([3,5], [4,2], [6, 1]), 'sort_tuples': False}, ([3, 5], [2, 4], [1, 6])),
-    ])
+    @pytest.mark.parametrize(
+        "kwargs, expected",
+        [
+            (
+                {"data": [(3, 5), (4, 2), (6, 1)], "sort_lists": False},
+                [(3, 5), (2, 4), (1, 6)],
+            ),
+            (
+                {"data": ([3, 5], [4, 2], [6, 1]), "sort_tuples": False},
+                ([3, 5], [2, 4], [1, 6]),
+            ),
+        ],
+    )
     def test_sort_only_inner(self, kwargs, expected):
         actual = sort_recursive(**kwargs)
         if is_iterator(expected):
             assert list(actual) == list(expected)
         else:
             assert actual == expected
 
-    @pytest.mark.parametrize('kwargs, expected', [
-        ({'data': [(3,5), (4,2), (6, 1)]}, [(1, 6), (2, 4), (3, 5)]),
-        ({'data': ([3,5], [4,2], [6, 1])}, ([1, 6], [2, 4], [3, 5])),
-        ({'data': {'a': (2, 3), 'b': (4, 1)}, 'sort_dicts_by': 'values'}, {'b': (1, 4), 'a': (2, 3)}),
-    ])
+    @pytest.mark.parametrize(
+        "kwargs, expected",
+        [
+            ({"data": [(3, 5), (4, 2), (6, 1)]}, [(1, 6), (2, 4), (3, 5)]),
+            ({"data": ([3, 5], [4, 2], [6, 1])}, ([1, 6], [2, 4], [3, 5])),
+            (
+                {"data": {"a": (2, 3), "b": (4, 1)}, "sort_dicts_by": "values"},
+                {"b": (1, 4), "a": (2, 3)},
+            ),
+        ],
+    )
     def test_sort_recursive(self, kwargs, expected):
         if is_iterator(expected):
             assert list(sort_recursive(**kwargs)) == list(expected)
         else:
             assert sort_recursive(**kwargs) == expected
 
 
 class Test_swap_keys_and_values:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("dict"))
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             swap_keys_and_values(wrong_type)
 
-    @pytest.mark.parametrize('data, expected', [
-        ({1: 2}, {2: 1}),
-        ({1: 'a', 3: 'b'}, {'a': 1, 'b': 3}),
-        ({1: 2, 3: 2}, {2: 3}),
-        ({}, {})
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ({1: 2}, {2: 1}),
+            ({1: "a", 3: "b"}, {"a": 1, "b": 3}),
+            ({1: 2, 3: 2}, {2: 3}),
+            ({}, {}),
+        ],
+    )
     def test_simple(self, data, expected):
         assert swap_keys_and_values(data) == expected
 
 
 class Test_xor:
-    @pytest.mark.parametrize('wrong_type', [
-        iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''
-    ])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [
+            iter([]),
+            map(lambda x: x, []),
+            range(1),
+            object(),
+            [],
+            {},
+            (),
+            set(),
+            1,
+            True,
+            False,
+            None,
+            "",
+        ],
+    )
     def test_key_should_be_callable(self, wrong_type):
         with pytest.raises(TypeError):
             xor(1, 2, condition=wrong_type)
 
-    @pytest.mark.parametrize('values', [
-        [],
-        [1],
-    ])
+    @pytest.mark.parametrize(
+        "values",
+        [
+            [],
+            [1],
+        ],
+    )
     def test_at_least_2_values(self, values):
         with pytest.raises(ValueError):
             xor(*values)
 
-    @pytest.mark.parametrize('values', [
-        [0, None, False],
-        [1, 2],
-    ])
+    @pytest.mark.parametrize(
+        "values",
+        [
+            [0, None, False],
+            [1, 2],
+        ],
+    )
     def test_none(self, values):
         assert xor(*values) is None
 
-    @pytest.mark.parametrize('values, expected', [
-        ([0, None, 2, False], 2),
-        ([1, 0], 1),
-        ([0, True], True),
-    ])
+    @pytest.mark.parametrize(
+        "values, expected",
+        [
+            ([0, None, 2, False], 2),
+            ([1, 0], 1),
+            ([0, True], True),
+        ],
+    )
     def test_ok(self, values, expected):
-        assert is_equal(xor(*values),  expected)
+        assert is_equal(xor(*values), expected)
 
 
 class Test_xor_with_idx:
-    @pytest.mark.parametrize('wrong_type', [
-        iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''
-    ])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [
+            iter([]),
+            map(lambda x: x, []),
+            range(1),
+            object(),
+            [],
+            {},
+            (),
+            set(),
+            1,
+            True,
+            False,
+            None,
+            "",
+        ],
+    )
     def test_key_should_be_callable(self, wrong_type):
         with pytest.raises(TypeError):
             xor_with_idx(1, 2, condition=wrong_type)
 
-    @pytest.mark.parametrize('values', [
-        [],
-        [1],
-    ])
+    @pytest.mark.parametrize(
+        "values",
+        [
+            [],
+            [1],
+        ],
+    )
     def test_at_least_2_values(self, values):
         with pytest.raises(ValueError):
             xor_with_idx(*values)
 
-    @pytest.mark.parametrize('values', [
-        [0, None, False],
-        [1, 2],
-    ])
+    @pytest.mark.parametrize(
+        "values",
+        [
+            [0, None, False],
+            [1, 2],
+        ],
+    )
     def test_none(self, values):
         assert xor_with_idx(*values) is None
 
-    @pytest.mark.parametrize('values, expected', [
-        ([0, None, 5, False], (2, 5)),
-        ([1, 0], (0, 1)),
-        ([0, True], (1, True)),
-    ])
+    @pytest.mark.parametrize(
+        "values, expected",
+        [
+            ([0, None, 5, False], (2, 5)),
+            ([1, 0], (0, 1)),
+            ([0, True], (1, True)),
+        ],
+    )
     def test_ok(self, values, expected):
         actual = xor_with_idx(*values)
         assert is_equal(actual, expected)
 
 
 class Test_detect_fronts:
-    @pytest.mark.parametrize('wrong_type', [
-        iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), None, ''
-    ])
+    @pytest.mark.parametrize(
+        "wrong_type",
+        [
+            iter([]),
+            map(lambda x: x, []),
+            range(1),
+            object(),
+            [],
+            {},
+            (),
+            set(),
+            None,
+            "",
+        ],
+    )
     def test_key_should_be_callable(self, wrong_type):
         with pytest.raises(TypeError):
             detect_fronts([0, 1, wrong_type, True, False])
 
-    @pytest.mark.parametrize('values, expected', [
-        ([], []),
-        ([0, 0, 0], []),
-        ([1, 1, 1], []),
-    ])
+    @pytest.mark.parametrize(
+        "values, expected",
+        [
+            ([], []),
+            ([0, 0, 0], []),
+            ([1, 1, 1], []),
+        ],
+    )
     def test_none(self, values, expected):
         assert detect_fronts(values) == expected
 
     def test_from_string(self):
         expected = [
             (3, 1),
             (4, -1),
             (6, 1),
             (7, -1),
             (8, 1),
             (11, -1),
             (12, 1),
             (14, -1),
         ]
-        assert detect_fronts('000100101110110') == expected
+        assert detect_fronts("000100101110110") == expected
 
     def test_from_iter(self):
         expected = [
             (3, 1),
             (4, -1),
             (6, 1),
             (7, -1),
             (8, 1),
             (11, -1),
             (12, 1),
             (14, -1),
         ]
-        assert detect_fronts(map(int, '000100101110110')) == expected
+        assert detect_fronts(map(int, "000100101110110")) == expected
 
     def test_detect_positive_fronts(self):
         assert detect_fronts_positive([0, 1, 0, 1]) == [1, 3]
         assert detect_fronts_positive([1, 0]) == []
 
     def test_detect_negative_fronts(self):
         assert detect_fronts_negative([1, 0, 1, 0]) == [1, 3]
```

### Comparing `katalytic-0.2.2/tests/test_files.py` & `katalytic-0.3.0/tests/test_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,336 +1,393 @@
 import copy
 import itertools
+
 import shutil
 import tempfile
 import warnings
 from pathlib import Path
 
 import pytest
 
-from katalytic.data import all_types_besides, as_dict_of_lists, as_list_of_lists, is_iterable, is_iterator
+from katalytic.data import as_dict_of_lists, as_list_of_lists, is_iterable, is_iterator
+from katalytic._pkg import all_types_besides
 from katalytic.data.checks import dicts_share_key_order
+
 # noinspection PyProtectedMember
 from katalytic.files import (
-    _load_funcs, _save_funcs, _get_all, clear_dir, copy_dir, copy_file, delete_dir, delete_file, get_dirs, get_files,
-    get_unique_path, is_dir_empty, get_all, is_file_empty, load, load_csv, load_json, load_text, make_dir, move_dir,
-    move_file, save, save_csv, save_json, save_text
+    _load_funcs,
+    _save_funcs,
+    _get_all,
+    clear_dir,
+    copy_dir,
+    copy_file,
+    delete_dir,
+    delete_file,
+    get_dirs,
+    get_files,
+    get_unique_path,
+    is_dir_empty,
+    get_all,
+    is_file_empty,
+    load,
+    load_csv,
+    load_json,
+    load_text,
+    make_dir,
+    move_dir,
+    move_file,
+    save,
+    save_csv,
+    save_json,
+    save_text,
 )
 
 
 def _compute_all_mismatched_combos(group_dict):
     good_matches = group_dict.items()
     all_matches = itertools.product(group_dict.keys(), group_dict.values())
     bad_matches = (m for m in all_matches if m not in good_matches)
     return ((*m, group_dict[m[0]].__name__) for m in bad_matches)
 
 
 def _create_seq_of_dicts():
     return [
-        {'a': 1, 'b': 'x', 'c': True, 'd': -1.5, 'e': True},
-        {'a': 2, 'b': None, 'c': False, 'd': 0.0, 'e': 'z'},
-        {'a': None, 'b': 'y', 'c': '', 'd': None, 'e': 'w'},
+        {"a": 1, "b": "x", "c": True, "d": -1.5, "e": True},
+        {"a": 2, "b": None, "c": False, "d": 0.0, "e": "z"},
+        {"a": None, "b": "y", "c": "", "d": None, "e": "w"},
     ]
 
 
 def _create_seq_of_seq():
     return as_list_of_lists(_create_seq_of_dicts())
 
 
 def _create_dict_of_seq():
     return as_dict_of_lists(_create_seq_of_dicts())
 
 
 class TestGroup_save_and_load:
     # noinspection PyBroadException
     class Test_warn_if_another_function_should_be_used:
-        @pytest.mark.parametrize('ext, wrong_load, correct_load', _compute_all_mismatched_combos(_load_funcs))
-        def test_using_the_wrong_loader_should_always_warn(self, ext, wrong_load, correct_load):
+        @pytest.mark.parametrize(
+            "ext, wrong_load, correct_load", _compute_all_mismatched_combos(_load_funcs)
+        )
+        def test_using_the_wrong_loader_should_always_warn(
+            self, ext, wrong_load, correct_load
+        ):
             # The warning should be triggered regardless of whether the file exists or not.
-            with pytest.warns(UserWarning, match=f'Use "{correct_load}" for ".{ext}" files.'):
+            with pytest.warns(
+                UserWarning, match=f'Use "{correct_load}" for ".{ext}" files.'
+            ):
                 try:
-                    wrong_load(get_unique_path('{}.' + ext))
+                    wrong_load(get_unique_path("{}." + ext))
                 except Exception:
                     pass
 
-        @pytest.mark.parametrize('ext, wrong_save, correct_save', _compute_all_mismatched_combos(_save_funcs))
-        def test_using_the_wrong_saver_should_always_warn(self, ext, wrong_save, correct_save):
-            with pytest.warns(UserWarning, match=f'Use "{correct_save}" for ".{ext}" files.'):
+        @pytest.mark.parametrize(
+            "ext, wrong_save, correct_save", _compute_all_mismatched_combos(_save_funcs)
+        )
+        def test_using_the_wrong_saver_should_always_warn(
+            self, ext, wrong_save, correct_save
+        ):
+            with pytest.warns(
+                UserWarning, match=f'Use "{correct_save}" for ".{ext}" files.'
+            ):
                 try:
-                    wrong_save('', get_unique_path('{}.' + ext))
+                    wrong_save("", get_unique_path("{}." + ext))
                 except Exception:
                     pass
 
     # noinspection PyTypeChecker
     class Test_csv:
+        @pytest.mark.parametrize(
+            "data",
+            [
+                [],
+                [[]],
+                {"a": []},
+                {},
+            ],
+        )
+        def test_empty_csv(self, data):
+            p = get_unique_path("{}.csv")
+            save_csv([], p)
+            assert load_csv(p) == []
+
         def test_atomicity_interrupt(self):
-            path = get_unique_path('{}.csv')
-            data = [{'path': path}]
+            path = get_unique_path("{}.csv")
+            data = [{"path": path}]
 
             save_csv.__katalytic_test_atomicity_interrupt__ = True
             save_csv(data, path)
             assert not Path(path).exists()
 
             # make sure it's still working after the test
             # the atomicity flag is set back to False inside the function
             save_csv(data, path)
             assert load(path) == data
 
         def test_atomicity_race_condition_error(self):
-            path = get_unique_path('{}.csv')
-            data = [{'path': path}]
+            path = get_unique_path("{}.csv")
+            data = [{"path": path}]
 
             save_csv.__katalytic_test_atomicity_race_condition__ = True
             assert not Path(path).exists()
             with pytest.raises(FileExistsError):
-                save_csv(data, path, exists='error')
+                save_csv(data, path, exists="error")
 
-            assert load(path) == [{'race': 'condition'}]
+            assert load(path) == [{"race": "condition"}]
 
             # make sure it's still working after the test
             # the atomicity flag is set back to False inside the function
             delete_file(path)
             assert not Path(path).exists()
-            save_csv(data, path, exists='error')
+            save_csv(data, path, exists="error")
             assert load(path) == data
 
         def test_atomicity_race_condition_replace(self):
-            path = get_unique_path('{}.csv')
-            data = [{'path': path}]
+            path = get_unique_path("{}.csv")
+            data = [{"path": path}]
 
             save_csv.__katalytic_test_atomicity_race_condition__ = True
             assert not Path(path).exists()
-            save_csv(data, path, exists='replace')
+            save_csv(data, path, exists="replace")
             assert load(path) == data
 
             # make sure it's still working after the test
             # the atomicity flag is set back to False inside the function
             delete_file(path)
             assert not Path(path).exists()
-            save_csv(data, path, exists='replace')
+            save_csv(data, path, exists="replace")
             assert load(path) == data
 
         def test_atomicity_race_condition_skip(self):
-            path = get_unique_path('{}.csv')
-            data = [{'path': path}]
+            path = get_unique_path("{}.csv")
+            data = [{"path": path}]
 
             save_csv.__katalytic_test_atomicity_race_condition__ = True
             assert not Path(path).exists()
-            save_csv(data, path, exists='skip')
-            assert load(path) == [{'race': 'condition'}]
+            save_csv(data, path, exists="skip")
+            assert load(path) == [{"race": "condition"}]
 
             # make sure it's still working after the test
             # the atomicity flag is set back to False inside the function
             delete_file(path)
             assert not Path(path).exists()
-            save_csv(data, path, exists='skip')
+            save_csv(data, path, exists="skip")
             assert load(path) == data
 
         def test_default(self):
-            path = get_unique_path('{}.csv')
-            default = [{'a': 1, 'b': 2}]
+            path = get_unique_path("{}.csv")
+            default = [{"a": 1, "b": 2}]
             assert load_csv(path, default=default) == default
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True, 'hello'])
+        @pytest.mark.parametrize("mistake", [0, None, {}, True, "hello"])
         def test_precondition_exists(self, mistake):
-            path = get_unique_path('{}.csv')
+            path = get_unique_path("{}.csv")
             with pytest.raises(ValueError):
-                save_csv('', path, exists=mistake)
+                save_csv("", path, exists=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_make_dirs(self, mistake):
-            path = get_unique_path('{}.csv')
+            path = get_unique_path("{}.csv")
             with pytest.raises(TypeError):
-                save_csv('', path, make_dirs=mistake)
+                save_csv("", path, make_dirs=mistake)
 
         def test_make_dirs_False(self):
-            path = get_unique_path('{}/data.csv')
+            path = get_unique_path("{}/data.csv")
             with pytest.raises(FileNotFoundError):
                 save_csv(_create_seq_of_dicts(), path, make_dirs=False)
 
-            path = _setup_file('{}/data')
+            path = _setup_file("{}/data")
             with pytest.raises(NotADirectoryError):
-                save_csv(_create_seq_of_dicts(), f'{path}/x.csv', make_dirs=False)
+                save_csv(_create_seq_of_dicts(), f"{path}/x.csv", make_dirs=False)
 
         def test_exists_error(self):
-            path = _setup_file('{}.csv')
+            path = _setup_file("{}.csv")
             with pytest.raises(FileExistsError):
-                save_csv([], path, exists='error')
+                save_csv([], path, exists="error")
 
         def test_exists_replace(self):
-            path = _setup_file('{}.csv')
-            data = [{'a': 1, 'b': 2}]
-            save_csv(data, path, exists='replace')
+            path = _setup_file("{}.csv")
+            data = [{"a": 1, "b": 2}]
+            save_csv(data, path, exists="replace")
             assert load_csv(path) == data
 
         def test_exists_skip(self):
-            path = get_unique_path('{}.csv')
-            data_before = [{'a': 1, 'b': 2}]
-            data_after = [{'x': 3, 'y': 4}]
+            path = get_unique_path("{}.csv")
+            data_before = [{"a": 1, "b": 2}]
+            data_after = [{"x": 3, "y": 4}]
 
             save_csv(data_before, path)
-            save_csv(data_after, path, exists='skip')
+            save_csv(data_after, path, exists="skip")
             assert load_csv(path) == data_before
 
-        @pytest.mark.parametrize('data', [
-            _create_seq_of_seq(),
-            _create_seq_of_dicts(),
-            _create_dict_of_seq(),
-        ])
+        @pytest.mark.parametrize(
+            "data",
+            [
+                _create_seq_of_seq(),
+                _create_seq_of_dicts(),
+                _create_dict_of_seq(),
+            ],
+        )
         def test_basic(self, data):
             expected = _create_seq_of_dicts()
-            expected[0]['e'] = str(expected[0]['e'])
-            expected[2]['c'] = None
+            expected[0]["e"] = str(expected[0]["e"])
+            expected[2]["c"] = None
 
             path = _setup_path()
             save_csv(data, path)
             assert load_csv(path) == expected
 
         def test_mixed_int_with_float(self):
-            data = [{'a': 1, 'b': 2.0}, {'a': 3.0, 'b': 4}]
-            expected = [{'a': 1.0, 'b': 2}, {'a': 3.0, 'b': 4.0}]
+            data = [{"a": 1, "b": 2.0}, {"a": 3.0, "b": 4}]
+            expected = [{"a": 1.0, "b": 2}, {"a": 3.0, "b": 4.0}]
 
             path = _setup_path()
             save_csv(data, path)
             assert load_csv(path) == expected
 
-        @pytest.mark.parametrize('data', [
-            [{'a': 1, 'b': 2}, {'b': 4, 'a': 3}],
-            [{'b': 4, 'a': 3}, {'a': 1, 'b': 2}],
-        ])
+        @pytest.mark.parametrize(
+            "data",
+            [
+                [{"a": 1, "b": 2}, {"b": 4, "a": 3}],
+                [{"b": 4, "a": 3}, {"a": 1, "b": 2}],
+            ],
+        )
         def test_mixed_column_order(self, data):
             path = _setup_path()
             save_csv(data, path)
             result = load_csv(path)
 
             assert result == data
             assert dicts_share_key_order(data[0], result[0])
             assert dicts_share_key_order(data[0], result[1])
             assert not dicts_share_key_order(data[0], data[1])
 
     class Test_json:
         def test_atomicity_interrupt(self):
-            path = get_unique_path('{}.json')
-            data = [{'path': path}]
+            path = get_unique_path("{}.json")
+            data = [{"path": path}]
 
             try:
                 save_json.__katalytic_test_atomicity_interrupt__ = True
                 save_json(data, path)
                 assert not Path(path).exists()
 
                 # make sure it's still working after the test
                 # the atomicity flag is set back to False inside the function
                 save_json(data, path)
                 assert load_json(path) == data
             except:
                 raise
 
         def test_atomicity_race_condition_error(self):
-            path = get_unique_path('{}.json')
-            data = [{'path': path}]
+            path = get_unique_path("{}.json")
+            data = [{"path": path}]
 
             try:
                 save_json.__katalytic_test_atomicity_race_condition__ = True
                 assert not Path(path).exists()
                 with pytest.raises(FileExistsError):
-                    save_json(data, path, exists='error')
+                    save_json(data, path, exists="error")
 
-                assert load(path) == [{'race': 'condition'}]
+                assert load(path) == [{"race": "condition"}]
 
                 # make sure it's still working after the test
                 # the atomicity flag is set back to False inside the function
                 delete_file(path)
                 assert not Path(path).exists()
-                save_json(data, path, exists='error')
+                save_json(data, path, exists="error")
                 assert load(path) == data
             except:
                 raise
 
         def test_atomicity_race_condition_replace(self):
-            path = get_unique_path('{}.json')
-            data = [{'path': path}]
+            path = get_unique_path("{}.json")
+            data = [{"path": path}]
 
             try:
                 save_json.__katalytic_test_atomicity_race_condition__ = True
                 assert not Path(path).exists()
-                save_json(data, path, exists='replace')
+                save_json(data, path, exists="replace")
                 assert load(path) == data
 
                 # make sure it's still working after the test
                 # the atomicity flag is set back to False inside the function
                 delete_file(path)
                 assert not Path(path).exists()
-                save_json(data, path, exists='replace')
+                save_json(data, path, exists="replace")
                 assert load(path) == data
             except:
                 raise
 
         def test_atomicity_race_condition_skip(self):
-            path = get_unique_path('{}.json')
-            data = [{'path': path}]
+            path = get_unique_path("{}.json")
+            data = [{"path": path}]
 
             try:
                 save_json.__katalytic_test_atomicity_race_condition__ = True
                 assert not Path(path).exists()
-                save_json(data, path, exists='skip')
-                assert load(path) == [{'race': 'condition'}]
+                save_json(data, path, exists="skip")
+                assert load(path) == [{"race": "condition"}]
 
                 # make sure it's still working after the test
                 # the atomicity flag is set back to False inside the function
                 delete_file(path)
                 assert not Path(path).exists()
-                save_json(data, path, exists='skip')
+                save_json(data, path, exists="skip")
                 assert load(path) == data
             except:
                 raise
 
         def test_default(self):
-            path = get_unique_path('{}.json')
-            default = [{'a': 1, 'b': 2}]
+            path = get_unique_path("{}.json")
+            default = [{"a": 1, "b": 2}]
             assert load_json(path, default=default) == default
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True, 'hello'])
+        @pytest.mark.parametrize("mistake", [0, None, {}, True, "hello"])
         def test_precondition_exists(self, mistake):
-            path = get_unique_path('{}.json')
+            path = get_unique_path("{}.json")
             with pytest.raises(ValueError):
                 save_json([], path, exists=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_make_dirs(self, mistake):
-            path = get_unique_path('{}.json')
+            path = get_unique_path("{}.json")
             with pytest.raises(TypeError):
                 save_json([], path, make_dirs=mistake)
 
         def test_make_dirs_False(self):
-            path = get_unique_path('{}/data.json')
+            path = get_unique_path("{}/data.json")
             with pytest.raises(FileNotFoundError):
                 save_json(_create_seq_of_dicts(), path, make_dirs=False)
 
-            path = _setup_file('{}/data')
+            path = _setup_file("{}/data")
             with pytest.raises(NotADirectoryError):
-                save_json(_create_seq_of_dicts(), f'{path}/x.json', make_dirs=False)
+                save_json(_create_seq_of_dicts(), f"{path}/x.json", make_dirs=False)
 
         def test_exists_error(self):
-            path = _setup_file('{}.json')
+            path = _setup_file("{}.json")
             with pytest.raises(FileExistsError):
-                save_json([], path, exists='error')
+                save_json([], path, exists="error")
 
         def test_exists_replace(self):
-            path = _setup_file('{}.json')
-            data = [{'a': 1, 'b': 2}]
-            save_json(data, path, exists='replace')
+            path = _setup_file("{}.json")
+            data = [{"a": 1, "b": 2}]
+            save_json(data, path, exists="replace")
             assert load_json(path) == data
 
         def test_exists_skip(self):
-            path = get_unique_path('{}.json')
-            data_before = [{'a': 1, 'b': 2}]
-            data_after = [{'x': 3, 'y': 4}]
+            path = get_unique_path("{}.json")
+            data_before = [{"a": 1, "b": 2}]
+            data_after = [{"x": 3, "y": 4}]
 
             save_json(data_before, path)
-            save_json(data_after, path, exists='skip')
+            save_json(data_after, path, exists="skip")
             assert load_json(path) == data_before
 
         def test_indent_0(self):
             data = self.create_json_data()
             path = _setup_path()
             save_json(data, path, indent=0)
             assert load_json(path) == data
@@ -350,15 +407,15 @@
         def test_indent_as_float(self):
             data = self.create_json_data()
             path = _setup_path()
 
             save_json(data, path, indent=1.0)
             assert load_json(path) == data
 
-        @pytest.mark.parametrize('mistake', all_types_besides('int'))
+        @pytest.mark.parametrize("mistake", all_types_besides("int"))
         def test_indent_of_wrong_type(self, mistake):
             data = self.create_json_data()
             path = _setup_path()
             with pytest.raises(TypeError):
                 save_json(data, path, indent=mistake)
 
         def test_save_sort_keys(self):
@@ -383,494 +440,505 @@
                 return all(self.are_keys_sorted_recursive(item) for item in data)
             else:
                 return True
 
         @staticmethod
         def create_json_data():
             """The keys are shuffled on purpose."""
-            return {'e': 0, 'a': 1, 'b': 2.0, 'c': 3.5, 'd': [{'y': None, 'f': True, 'g': {'x': 'i', 'j': [False]}}]}
+            return {
+                "e": 0,
+                "a": 1,
+                "b": 2.0,
+                "c": 3.5,
+                "d": [{"y": None, "f": True, "g": {"x": "i", "j": [False]}}],
+            }
 
     class Test_text:
         def test_atomicity_interrupt(self):
-            path = get_unique_path('{}.txt')
+            path = get_unique_path("{}.txt")
 
             try:
                 save_text.__katalytic_test_atomicity_interrupt__ = True
                 save_text(path, path)
                 assert not Path(path).exists()
 
                 # make sure it's still working after the test
                 # the atomicity flag is set back to False inside the function
                 save_text(path, path)
                 assert load(path) == path
             except:
                 raise
 
         def test_atomicity_race_condition_error(self):
-            path = get_unique_path('{}.txt')
-            data = f'path = {path!r}'
+            path = get_unique_path("{}.txt")
+            data = f"path = {path!r}"
 
             try:
                 save_text.__katalytic_test_atomicity_race_condition__ = True
                 assert not Path(path).exists()
                 with pytest.raises(FileExistsError):
-                    save_text(data, path, exists='error')
+                    save_text(data, path, exists="error")
 
-                assert load(path) == 'race condition'
+                assert load(path) == "race condition"
 
                 # make sure it's still working after the test
                 # the atomicity flag is set back to False inside the function
                 delete_file(path)
                 assert not Path(path).exists()
-                save_text(data, path, exists='error')
+                save_text(data, path, exists="error")
                 assert load(path) == data
             except:
                 raise
 
         def test_atomicity_race_condition_replace(self):
-            path = get_unique_path('{}.txt')
-            data = f'path = {path!r}'
+            path = get_unique_path("{}.txt")
+            data = f"path = {path!r}"
 
             try:
                 save_text.__katalytic_test_atomicity_race_condition__ = True
                 assert not Path(path).exists()
-                save_text(data, path, exists='replace')
+                save_text(data, path, exists="replace")
                 assert load(path) == data
 
                 # make sure it's still working after the test
                 # the atomicity flag is set back to False inside the function
                 delete_file(path)
                 assert not Path(path).exists()
-                save_text(data, path, exists='replace')
+                save_text(data, path, exists="replace")
                 assert load(path) == data
             except:
                 raise
 
         def test_atomicity_race_condition_skip(self):
-            path = get_unique_path('{}.txt')
-            data = f'path = {path!r}'
+            path = get_unique_path("{}.txt")
+            data = f"path = {path!r}"
 
             try:
                 save_text.__katalytic_test_atomicity_race_condition__ = True
                 assert not Path(path).exists()
-                save_text(data, path, exists='skip')
-                assert load(path) == 'race condition'
+                save_text(data, path, exists="skip")
+                assert load(path) == "race condition"
 
                 # make sure it's still working after the test
                 # the atomicity flag is set back to False inside the function
                 delete_file(path)
                 assert not Path(path).exists()
-                save_text(data, path, exists='skip')
+                save_text(data, path, exists="skip")
                 assert load(path) == data
             except:
                 raise
 
         def test_default(self):
-            path = get_unique_path('{}.txt')
-            assert load_text(path, default='hello') == 'hello'
+            path = get_unique_path("{}.txt")
+            assert load_text(path, default="hello") == "hello"
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True, 'hello'])
+        @pytest.mark.parametrize("mistake", [0, None, {}, True, "hello"])
         def test_precondition_exists(self, mistake):
-            path = get_unique_path('{}.txt')
+            path = get_unique_path("{}.txt")
             with pytest.raises(ValueError):
-                save_text('', path, exists=mistake)
+                save_text("", path, exists=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_make_dirs(self, mistake):
-            path = get_unique_path('{}.txt')
+            path = get_unique_path("{}.txt")
             with pytest.raises(TypeError):
-                save_text('', path, make_dirs=mistake)
+                save_text("", path, make_dirs=mistake)
 
         def test_make_dirs_False(self):
-            path = get_unique_path('{}/data.txt')
+            path = get_unique_path("{}/data.txt")
             with pytest.raises(FileNotFoundError):
-                save_text('hello', path, make_dirs=False)
+                save_text("hello", path, make_dirs=False)
 
-            path = _setup_file('{}/data')
+            path = _setup_file("{}/data")
             with pytest.raises(NotADirectoryError):
-                save_text('hello', f'{path}/x.txt', make_dirs=False)
+                save_text("hello", f"{path}/x.txt", make_dirs=False)
 
         def test_exists_error(self):
-            path = _setup_file('{}.txt')
+            path = _setup_file("{}.txt")
             with pytest.raises(FileExistsError):
-                save_text('data', path, exists='error')
+                save_text("data", path, exists="error")
 
         def test_exists_replace(self):
-            path = _setup_file('{}.txt')
-            save_text('data', path, exists='replace')
-            assert load_text(path) == 'data'
+            path = _setup_file("{}.txt")
+            save_text("data", path, exists="replace")
+            assert load_text(path) == "data"
 
         def test_exists_skip(self):
-            path = get_unique_path('{}.txt')
-            save_text('before', path)
-            save_text('after', path, exists='skip')
-            assert load_text(path) == 'before'
+            path = get_unique_path("{}.txt")
+            save_text("before", path)
+            save_text("after", path, exists="skip")
+            assert load_text(path) == "before"
 
         def test_basic(self):
-            data = 'some text\nwith newlines'
+            data = "some text\nwith newlines"
             path = _setup_path()
             save_text(data, path)
             assert load_text(path) == data
 
     # noinspection PyTypeChecker
     class Test_universal_load_and_save:
-        @pytest.mark.parametrize('pattern, default', [
-            ('{}.csv', _create_seq_of_dicts()),
-            ('{}.json', _create_dict_of_seq()),
-            ('{}.txt', 'hello'),
-        ])
+        @pytest.mark.parametrize(
+            "pattern, default",
+            [
+                ("{}.csv", _create_seq_of_dicts()),
+                ("{}.json", _create_dict_of_seq()),
+                ("{}.txt", "hello"),
+            ],
+        )
         def test_default(self, pattern, default):
             path = get_unique_path(pattern)
             assert load(path, default=default) == default
 
         def test_unknown(self):
-            with pytest.raises(RuntimeError):
-                load('data.unknown')
-
-            with pytest.raises(RuntimeError):
-                save('', 'data.unknown')
+            path = get_unique_path("{}.unknown")
+            save("hello world", path)
+            assert load(path) == "hello world"
 
         def test_txt(self):
-            data = 'Hello, World!\nThis is not a drill'
-            path = _setup_path('{}.txt')
+            data = "Hello, World!\nThis is not a drill"
+            path = _setup_path("{}.txt")
             save(data, path)
 
             assert load(path) == load_text(path) == data
 
         def test_csv(self):
             data = _create_seq_of_dicts()
-            path = _setup_path('{}.CSV')
+            path = _setup_path("{}.CSV")
             save(data, path)
 
             expected_csv = copy.deepcopy(data)
-            expected_csv[0]['e'] = str(expected_csv[0]['e'])
-            expected_csv[2]['c'] = None
+            expected_csv[0]["e"] = str(expected_csv[0]["e"])
+            expected_csv[2]["c"] = None
 
-            expected_text = '\n'.join([
-                '"a","b","c","d","e"',
-                '"1","x","True","-1.5","True"',
-                '"2","","False","0.0","z"',
-                '"","y","","","w"',
-            ])
+            expected_text = "\n".join(
+                [
+                    '"a","b","c","d","e"',
+                    '"1","x","True","-1.5","True"',
+                    '"2","","False","0.0","z"',
+                    '"","y","","","w"',
+                ]
+            )
 
             assert load(path) == expected_csv
 
             with warnings.catch_warnings():
-                warnings.simplefilter('ignore')
+                warnings.simplefilter("ignore")
                 assert load_text(path).strip() == expected_text
 
         def test_json(self):
-            data = {'a': 1, 'b': [2, True, None, {}]}
-            path = _setup_path('{}.json')
+            data = {"a": 1, "b": [2, True, None, {}]}
+            path = _setup_path("{}.json")
             save(data, path)
 
-            expected_text = '\n'.join([
-                '{',
-                '    "a": 1,',
-                '    "b": [',
-                '        2,',
-                '        true,',
-                '        null,',
-                '        {}',
-                '    ]',
-                '}',
-            ])
+            expected_text = "\n".join(
+                [
+                    "{",
+                    '    "a": 1,',
+                    '    "b": [',
+                    "        2,",
+                    "        true,",
+                    "        null,",
+                    "        {}",
+                    "    ]",
+                    "}",
+                ]
+            )
 
             assert load(path) == data
 
             with warnings.catch_warnings():
-                warnings.simplefilter('ignore')
+                warnings.simplefilter("ignore")
                 assert load_text(path).strip() == expected_text
 
 
 class TestGroup_copy:
     # noinspection PyTypeChecker
     class Test_copy_dir:
         def test_dest_is_dir(self):
-            src = Path(_setup_tree('{}_src'))
+            src = Path(_setup_tree("{}_src"))
 
-            dest = Path(get_unique_path('{}_dest'))
+            dest = Path(get_unique_path("{}_dest"))
             copy_dir(src, dest)
-            _check_tree(src, dest/src.name)
+            _check_tree(src, dest / src.name)
 
-            dest_2 = Path(get_unique_path('{}_dest_2'))
-            copy_dir(src, dest_2/src.name)
-            _check_tree(src, dest_2/src.name)
+            dest_2 = Path(get_unique_path("{}_dest_2"))
+            copy_dir(src, dest_2 / src.name)
+            _check_tree(src, dest_2 / src.name)
 
         def test_dest_is_file(self):
             with pytest.raises(NotADirectoryError):
                 src = _setup_dir()
                 dest = _setup_file()
                 copy_dir(src, dest)
 
         def test_dir_exists_error(self):
             with pytest.raises(FileExistsError):
                 src = _setup_tree()
                 dest = _setup_tree()
-                copy_dir(src, dest, dir_exists='error', file_exists='skip')
+                copy_dir(src, dest, dir_exists="error", file_exists="skip")
 
         def test_dir_exists_merge(self):
             src, src_file = _setup_dir_and_file()
-            _setup_tree(src + '/{}')
+            _setup_tree(src + "/{}")
 
             dest = _setup_tree()
-            copy_dir(src, dest, dir_exists='merge', file_exists='skip')
+            copy_dir(src, dest, dir_exists="merge", file_exists="skip")
 
             src_dirs = get_dirs(src, prefix=False, recursive=True)
             dest_dirs = get_dirs(dest, prefix=False, recursive=True)
             assert set(src_dirs).difference(dest_dirs) == set()
             assert set(dest_dirs).difference(src_dirs) != set()
 
         def test_dir_exists_replace(self):
             src, src_file = _setup_dir_and_file()
             dest = _setup_tree()
-            copy_dir(src, dest, dir_exists='replace', file_exists='skip')
+            copy_dir(src, dest, dir_exists="replace", file_exists="skip")
 
             src_tree = get_all(src, prefix=False, recursive=True)
             dest_tree = get_all(dest, prefix=False, recursive=True)
             assert src_tree == dest_tree
 
             src_tree = set(get_all(src, recursive=True))
             dest_tree = set(get_all(dest, recursive=True))
             pairs = {(fn, fn.replace(src, dest)) for fn in src_tree | dest_tree}
             pairs = {(Path(s), Path(d)) for s, d in pairs if Path(s).is_file()}
             assert all((s.read_text() == d.read_text()) for s, d in pairs)
 
         def test_dir_exists_skip(self):
             src, src_file = _setup_dir_and_file()
             dest, dest_file = _setup_dir_and_file()
-            make_dir(f'{dest}/subdir')
+            make_dir(f"{dest}/subdir")
 
-            copy_dir(src, dest, dir_exists='skip', file_exists='replace')
+            copy_dir(src, dest, dir_exists="skip", file_exists="replace")
             assert Path(dest_file).read_text() != Path(src_file).read_text()
-            assert Path(f'{dest}/subdir').is_dir()
+            assert Path(f"{dest}/subdir").is_dir()
 
         def test_file_exists_error(self):
             with pytest.raises(FileExistsError):
                 src = _setup_tree()
                 dest = _setup_tree()
-                copy_dir(src, dest, dir_exists='merge', file_exists='error')
+                copy_dir(src, dest, dir_exists="merge", file_exists="error")
 
         def test_file_exists_replace(self):
             src, src_file = _setup_dir_and_file()
             dest, dest_file = _setup_dir_and_file()
 
-            copy_dir(src, dest, dir_exists='merge', file_exists='replace')
+            copy_dir(src, dest, dir_exists="merge", file_exists="replace")
             assert Path(dest_file).read_text() == Path(src_file).read_text()
 
         def test_file_exists_skip(self):
             src, src_file = _setup_dir_and_file()
             dest, dest_file = _setup_dir_and_file()
 
             original = Path(dest_file).read_text()
-            copy_dir(src, dest, dir_exists='merge', file_exists='skip')
+            copy_dir(src, dest, dir_exists="merge", file_exists="skip")
             assert Path(dest_file).read_text() != Path(src_file).read_text()
             assert Path(dest_file).read_text() == original
 
         def test_make_dirs_false(self):
             with pytest.raises(FileNotFoundError):
                 with tempfile.TemporaryDirectory() as d:
-                    src = get_unique_path(d + '/{}_src')
-                    dest = get_unique_path(d + '/{}_dest')
+                    src = get_unique_path(d + "/{}_src")
+                    dest = get_unique_path(d + "/{}_dest")
                     make_dir(src)
                     copy_dir(src, dest, make_dirs=False)
 
         def test_make_dirs_true(self):
             with tempfile.TemporaryDirectory() as d:
                 src = _setup_tree()
                 src_name = Path(src).name
 
-                dest = get_unique_path(d + '/{}_dest')
+                dest = get_unique_path(d + "/{}_dest")
                 copy_dir(src, dest, make_dirs=True)
-                _check_tree(src, f'{dest}/{src_name}')
+                _check_tree(src, f"{dest}/{src_name}")
 
-                dest_2 = get_unique_path(d + '/{}_dest_2')
-                copy_dir(src, f'{dest_2}/{src_name}', make_dirs=True)
-                _check_tree(src, f'{dest_2}/{src_name}')
+                dest_2 = get_unique_path(d + "/{}_dest_2")
+                copy_dir(src, f"{dest_2}/{src_name}", make_dirs=True)
+                _check_tree(src, f"{dest_2}/{src_name}")
 
         def test_same_path(self):
             with pytest.raises(ValueError):
                 src = _setup_dir()
                 copy_dir(src, src)
 
         def test_src_is_file(self):
             with pytest.raises(NotADirectoryError):
                 src = _setup_file()
-                dest = get_unique_path('{}_new')
+                dest = get_unique_path("{}_new")
                 copy_dir(src, dest)
 
         def test_src_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 src = get_unique_path()
-                copy_dir(src, f'{src}_copy')
+                copy_dir(src, f"{src}_copy")
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_dest(self, mistake):
             with pytest.raises(TypeError):
-                copy_dir('src', mistake)
+                copy_dir("src", mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True, 'hello'])
+        @pytest.mark.parametrize("mistake", [0, None, {}, True, "hello"])
         def test_precondition_dir_exists(self, mistake):
             with pytest.raises(ValueError):
-                copy_dir('src', 'dest', dir_exists=mistake)
+                copy_dir("src", "dest", dir_exists=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, 'hello'])
+        @pytest.mark.parametrize("mistake", [0, None, {}, "hello"])
         def test_precondition_file_exists(self, mistake):
             with pytest.raises(ValueError):
-                copy_dir('src', 'dest', file_exists=mistake)
+                copy_dir("src", "dest", file_exists=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_make_dirs(self, mistake):
             with pytest.raises(TypeError):
                 src, dest = _setup_dir(n=2)
                 copy_dir(src, dest, make_dirs=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_src(self, mistake):
             with pytest.raises(TypeError):
-                copy_dir(mistake, 'dest')
+                copy_dir(mistake, "dest")
 
     # noinspection PyTypeChecker
     class Test_copy_file:
         def test_atomicity_interrupt(self):
-            src = _setup_file('{}.txt')
-            dest = get_unique_path('{}.txt')
+            src = _setup_file("{}.txt")
+            dest = get_unique_path("{}.txt")
 
             copy_file.__katalytic_test_atomicity_interrupt__ = True
             copy_file(src, dest)
             assert not Path(dest).exists()
 
             # make sure it's still working after the test
             # the atomicity flag is set back to False inside the function
             copy_file(src, dest)
             assert load(dest) == src
 
         def test_atomicity_race_condition_error(self):
-            src = _setup_file('{}.txt')
-            dest = get_unique_path('{}.txt')
+            src = _setup_file("{}.txt")
+            dest = get_unique_path("{}.txt")
 
             copy_file.__katalytic_test_atomicity_race_condition__ = True
             assert not Path(dest).exists()
             with pytest.raises(FileExistsError):
-                copy_file(src, dest, exists='error')
+                copy_file(src, dest, exists="error")
 
-            assert load(dest) == 'race condition'
+            assert load(dest) == "race condition"
 
             # make sure it's still working after the test
             # the atomicity flag is set back to False inside the function
             delete_file(dest)
             assert not Path(dest).exists()
-            copy_file(src, dest, exists='error')
+            copy_file(src, dest, exists="error")
             assert load(dest) == src
 
         def test_atomicity_race_condition_replace(self):
-            src = _setup_file('{}.txt')
-            dest = get_unique_path('{}.txt')
+            src = _setup_file("{}.txt")
+            dest = get_unique_path("{}.txt")
 
             copy_file.__katalytic_test_atomicity_race_condition__ = True
             assert not Path(dest).exists()
-            copy_file(src, dest, exists='replace')
+            copy_file(src, dest, exists="replace")
             assert load(dest) == src
 
             # make sure it's still working after the test
             # the atomicity flag is set back to False inside the function
             delete_file(dest)
             assert not Path(dest).exists()
-            copy_file(src, dest, exists='replace')
+            copy_file(src, dest, exists="replace")
             assert load(dest) == src
 
         def test_atomicity_race_condition_skip(self):
-            src = _setup_file('{}.txt')
-            dest = get_unique_path('{}.txt')
+            src = _setup_file("{}.txt")
+            dest = get_unique_path("{}.txt")
 
             copy_file.__katalytic_test_atomicity_race_condition__ = True
             assert not Path(dest).exists()
-            copy_file(src, dest, exists='skip')
-            assert load(dest) == 'race condition'
+            copy_file(src, dest, exists="skip")
+            assert load(dest) == "race condition"
 
             # make sure it's still working after the test
             # the atomicity flag is set back to False inside the function
             delete_file(dest)
             assert not Path(dest).exists()
-            copy_file(src, dest, exists='skip')
+            copy_file(src, dest, exists="skip")
             assert load(dest) == src
 
         def test_dir(self):
             with pytest.raises(IsADirectoryError):
                 src = _setup_dir()
                 dest = get_unique_path()
                 copy_file(src, dest)
 
         def test_exists_error(self):
             with pytest.raises(FileExistsError):
                 src, dest = _setup_file(n=2)
-                copy_file(src, dest, exists='error')
+                copy_file(src, dest, exists="error")
 
         def test_exists_replace(self):
             src, dest = _setup_file(n=2)
-            copy_file(src, dest, exists='replace')
+            copy_file(src, dest, exists="replace")
 
             text = Path(dest).read_text()
             assert text == Path(src).read_text()
             assert text != dest
 
         def test_exists_skip(self):
             src, dest = _setup_file(n=2)
-            copy_file(src, dest, exists='skip')
+            copy_file(src, dest, exists="skip")
 
             text = Path(dest).read_text()
             assert text != Path(src).read_text()
             assert text == dest
 
         def test_missing(self):
             dest = _setup_file()
             src = get_unique_path()
             with pytest.raises(FileNotFoundError):
                 copy_file(src, dest)
 
         def test_ends_with_slash(self):
             src = _setup_file()
             root = get_unique_path()
-            dest = root + '/1/2/3/'
+            dest = root + "/1/2/3/"
             copy_file(src, dest)
 
         def test_make_dirs_false(self):
             with pytest.raises(FileNotFoundError):
                 src = _setup_file()
-                dest = get_unique_path('{}/a/b/c/')
+                dest = get_unique_path("{}/a/b/c/")
                 copy_file(src, dest, make_dirs=False)
 
         def test_make_dirs_true(self):
             src = _setup_file()
             dest = _setup_path()
             copy_file(src, dest, make_dirs=True)
             assert Path(dest).read_text() == src
 
         def test_same_path(self):
             with pytest.raises(ValueError):
                 src = _setup_file()
                 copy_file(src, src)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_src(self, mistake):
             with pytest.raises(TypeError):
-                copy_file(mistake, 'a')
+                copy_file(mistake, "a")
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_dest(self, mistake):
             with pytest.raises(TypeError):
-                copy_file('a', mistake)
+                copy_file("a", mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_make_dirs(self, mistake):
             with pytest.raises(TypeError):
                 src, dest = _setup_file(n=2)
                 copy_file(src, dest, make_dirs=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, 'hello'])
+        @pytest.mark.parametrize("mistake", [0, None, {}, "hello"])
         def test_precondition_exists(self, mistake):
             src, dest = _setup_file(n=2)
             with pytest.raises(ValueError):
                 copy_file(src, dest, exists=mistake)
 
 
 class TestGroup_delete:
@@ -900,37 +968,37 @@
             path, _ = _setup_dir_and_file()
             delete_dir(path, non_empty_dir=False)
             assert Path(path).is_dir()
 
         def test_non_empty_dir_error(self):
             with pytest.raises(OSError):
                 path, _ = _setup_dir_and_file()
-                delete_dir(path, non_empty_dir='error')
+                delete_dir(path, non_empty_dir="error")
 
         def test_non_empty_dir_true(self):
             path, _ = _setup_dir_and_file()
             delete_dir(path, non_empty_dir=True)
             assert not Path(path).exists()
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_missing_ok(self, mistake):
             with pytest.raises(TypeError):
                 delete_dir(get_unique_path(), missing_ok=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_non_empty_dir(self, mistake):
             with pytest.raises(ValueError):
                 delete_dir(get_unique_path(), non_empty_dir=mistake)
 
-        @pytest.mark.parametrize('mistake', [None, '', '.'])
+        @pytest.mark.parametrize("mistake", [None, "", "."])
         def test_precondition_path_current_dir(self, mistake):
             with pytest.raises(ValueError):
                 delete_dir(mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['none', 'str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["none", "str", "path"]))
         def test_precondition_path_type(self, mistake):
             with pytest.raises(TypeError):
                 delete_dir(mistake)
 
     # noinspection PyTypeChecker
     class Test_delete_file:
         def test_dir(self):
@@ -949,337 +1017,342 @@
                 delete_file(path, missing_ok=False)
 
         def test_missing_ok_true(self):
             path = get_unique_path()
             delete_file(path, missing_ok=True)
             assert not Path(path).exists()
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 delete_file(mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_missing_ok(self, mistake):
             with pytest.raises(TypeError):
                 delete_file(get_unique_path(), missing_ok=mistake)
 
 
 class TestGroup_get:
     class Test_get_all:
         def test_prefix_false(self):
             path = _setup_tree()
-            expected = ['1.txt', 'a', 'a/2.txt', 'b', 'b/3.txt', 'b/c', 'b/c/4.txt']
+            expected = ["1.txt", "a", "a/2.txt", "b", "b/3.txt", "b/c", "b/c/4.txt"]
             assert get_all(path, prefix=False, recursive=True) == expected
 
         def test_prefix_true(self):
             path = _setup_tree()
             expected = [
-                f'{path}/1.txt',
-                f'{path}/a',
-                f'{path}/a/2.txt',
-                f'{path}/b',
-                f'{path}/b/3.txt',
-                f'{path}/b/c',
-                f'{path}/b/c/4.txt'
+                f"{path}/1.txt",
+                f"{path}/a",
+                f"{path}/a/2.txt",
+                f"{path}/b",
+                f"{path}/b/3.txt",
+                f"{path}/b/c",
+                f"{path}/b/c/4.txt",
             ]
             assert get_all(path, prefix=True, recursive=True) == expected
 
         def test_path_is_file(self):
             with pytest.raises(NotADirectoryError):
                 path = _setup_file()
                 get_all(path)
 
         def test_path_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 get_all(get_unique_path())
 
         def test_iter(self):
-            r = get_all('', iter_=True)
+            r = get_all("", iter_=True)
             assert is_iterator(r)
 
         def test_glob(self):
             path = _setup_tree_2()
-            assert get_all(f'{path}/*/a/*') == [f'{path}/a/a/6.py', f'{path}/b/a/5.py']
+            assert get_all(f"{path}/*/a/*") == [f"{path}/a/a/6.py", f"{path}/b/a/5.py"]
 
         def test_glob_recursive(self):
             path = _setup_tree_2()
-            expected = sorted(map(str, Path(path).glob('**/a/*')))
-            assert get_all(f'{path}/**/a/*') == expected
-            assert get_all(f'{path}/*/a/*', recursive=True) == expected
-
-            expected = sorted(map(str, Path(path).glob('**/a/**')))
-            assert get_all(f'{path}/**/a/**') == expected
-            assert get_all(f'{path}/**/a/**', recursive=True) == expected
+            expected = sorted(map(str, Path(path).glob("**/a/*")))
+            assert get_all(f"{path}/**/a/*") == expected
+            assert get_all(f"{path}/*/a/*", recursive=True) == expected
+
+            expected = sorted(map(str, Path(path).glob("**/a/**")))
+            assert get_all(f"{path}/**/a/**") == expected
+            assert get_all(f"{path}/**/a/**", recursive=True) == expected
 
         def test_only_dirs(self):
             path = _setup_tree()
-            assert _get_all(path, only_dirs=True, prefix=False) == ['a', 'b']
+            assert _get_all(path, only_dirs=True, prefix=False) == ["a", "b"]
 
         def test_only_files(self):
             path = _setup_tree()
-            assert _get_all(path, only_files=True, prefix=False) == ['1.txt']
+            assert _get_all(path, only_files=True, prefix=False) == ["1.txt"]
 
         def test_only_conflict(self):
             with pytest.raises(ValueError):
-                _get_all('', only_files=True, only_dirs=True)
+                _get_all("", only_files=True, only_dirs=True)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_glob(self, mistake):
             with pytest.raises(TypeError):
-                get_all('', glob=mistake)
+                get_all("", glob=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_iter_(self, mistake):
             with pytest.raises(TypeError):
-                get_all('', iter_=mistake)
+                get_all("", iter_=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_only_dirs(self, mistake):
             with pytest.raises(TypeError):
-                _get_all('', only_dirs=mistake)
+                _get_all("", only_dirs=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_only_files(self, mistake):
             with pytest.raises(TypeError):
-                _get_all('', only_files=mistake)
+                _get_all("", only_files=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize("mistake", [0, None, {}, True])
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 get_all(mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_prefix(self, mistake):
             with pytest.raises(TypeError):
-                get_all('', prefix=mistake)
+                get_all("", prefix=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_recursive(self, mistake):
             with pytest.raises(TypeError):
-                get_all('', recursive=mistake)
+                get_all("", recursive=mistake)
 
         def test_recursive(self):
             path = _setup_tree()
             assert get_all(path, recursive=True) == [
-                f'{path}/1.txt',
-                f'{path}/a',
-                f'{path}/a/2.txt',
-                f'{path}/b',
-                f'{path}/b/3.txt',
-                f'{path}/b/c',
-                f'{path}/b/c/4.txt',
+                f"{path}/1.txt",
+                f"{path}/a",
+                f"{path}/a/2.txt",
+                f"{path}/b",
+                f"{path}/b/3.txt",
+                f"{path}/b/c",
+                f"{path}/b/c/4.txt",
             ]
 
         def test_sorted(self):
             path = _setup_tree()
-            _ = _setup_tree(path + '/b/{}')
+            _ = _setup_tree(path + "/b/{}")
             assert get_all(path, iter_=False, recursive=True) == [
-                f'{path}/1.txt',
-                f'{path}/a',
-                f'{path}/a/2.txt',
-                f'{path}/b',
-                f'{path}/b/1',
-                f'{path}/b/1/1.txt',
-                f'{path}/b/1/a',
-                f'{path}/b/1/a/2.txt',
-                f'{path}/b/1/b',
-                f'{path}/b/1/b/3.txt',
-                f'{path}/b/1/b/c',
-                f'{path}/b/1/b/c/4.txt',
-                f'{path}/b/3.txt',
-                f'{path}/b/c',
-                f'{path}/b/c/4.txt',
+                f"{path}/1.txt",
+                f"{path}/a",
+                f"{path}/a/2.txt",
+                f"{path}/b",
+                f"{path}/b/1",
+                f"{path}/b/1/1.txt",
+                f"{path}/b/1/a",
+                f"{path}/b/1/a/2.txt",
+                f"{path}/b/1/b",
+                f"{path}/b/1/b/3.txt",
+                f"{path}/b/1/b/c",
+                f"{path}/b/1/b/c/4.txt",
+                f"{path}/b/3.txt",
+                f"{path}/b/c",
+                f"{path}/b/c/4.txt",
             ]
 
         def test_returns_same_type_as_input(self):
             path = _setup_tree()
             result = get_all(path, recursive=True)
             assert all(isinstance(p, str) for p in result)
 
             path = Path(_setup_tree())
             result = get_all(path, recursive=True)
             assert all(isinstance(p, Path) for p in result)
 
     class Test_get_dirs:
         def test_prefix_false(self):
             path = _setup_tree()
-            assert get_dirs(path, prefix=False, recursive=True) == ['a', 'b', 'b/c']
+            assert get_dirs(path, prefix=False, recursive=True) == ["a", "b", "b/c"]
 
         def test_prefix_true(self):
             path = _setup_tree()
-            expected = [f'{path}/a', f'{path}/b', f'{path}/b/c']
+            expected = [f"{path}/a", f"{path}/b", f"{path}/b/c"]
             assert get_dirs(path, prefix=True, recursive=True) == expected
 
         def test_path_is_file(self):
             with pytest.raises(NotADirectoryError):
                 path = _setup_file()
                 get_dirs(path)
 
         def test_path_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 get_dirs(get_unique_path())
 
         def test_iter(self):
-            r = get_dirs('', iter_=True)
+            r = get_dirs("", iter_=True)
             assert is_iterator(r)
 
         def test_glob(self):
             path = _setup_tree_2()
-            assert get_dirs(f'{path}/*/a') == [f'{path}/a/a', f'{path}/b/a']
+            assert get_dirs(f"{path}/*/a") == [f"{path}/a/a", f"{path}/b/a"]
 
         def test_glob_recursive(self):
             path = _setup_tree_2()
-            expected = [f'{path}/a', f'{path}/a/a', f'{path}/b/a', f'{path}/b/c/a']
-            assert get_dirs(f'{path}/**/a') == expected
-            assert get_dirs(f'{path}/*/a', recursive=True) == expected
+            expected = [f"{path}/a", f"{path}/a/a", f"{path}/b/a", f"{path}/b/c/a"]
+            assert get_dirs(f"{path}/**/a") == expected
+            assert get_dirs(f"{path}/*/a", recursive=True) == expected
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_prefix(self, mistake):
             with pytest.raises(TypeError):
-                get_dirs('', prefix=mistake)
+                get_dirs("", prefix=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_glob(self, mistake):
             with pytest.raises(TypeError):
-                get_dirs('', glob=mistake)
+                get_dirs("", glob=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_iter_(self, mistake):
             with pytest.raises(TypeError):
-                get_dirs('', iter_=mistake)
+                get_dirs("", iter_=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 get_dirs(mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_recursive(self, mistake):
             with pytest.raises(TypeError):
-                get_dirs('', recursive=mistake)
+                get_dirs("", recursive=mistake)
 
         def test_recursive(self):
             path = _setup_tree()
             assert get_dirs(path, recursive=True) == [
-                f'{path}/a',
-                f'{path}/b',
-                f'{path}/b/c',
+                f"{path}/a",
+                f"{path}/b",
+                f"{path}/b/c",
             ]
 
         def test_sorted(self):
             path = _setup_tree()
-            _ = _setup_tree(path + '/b/{}')
+            _ = _setup_tree(path + "/b/{}")
             assert get_dirs(path, iter_=False, recursive=True) == [
-                f'{path}/a',
-                f'{path}/b',
-                f'{path}/b/1',
-                f'{path}/b/1/a',
-                f'{path}/b/1/b',
-                f'{path}/b/1/b/c',
-                f'{path}/b/c',
+                f"{path}/a",
+                f"{path}/b",
+                f"{path}/b/1",
+                f"{path}/b/1/a",
+                f"{path}/b/1/b",
+                f"{path}/b/1/b/c",
+                f"{path}/b/c",
             ]
 
         def test_returns_same_type_as_input(self):
             path = _setup_tree()
             result = get_dirs(path, recursive=True)
             assert all(isinstance(p, str) for p in result)
 
             path = Path(_setup_tree())
             result = get_dirs(path, recursive=True)
             assert all(isinstance(p, Path) for p in result)
 
     class Test_get_files:
         def test_prefix_false(self):
             path = _setup_tree()
-            expected = ['1.txt', 'a/2.txt', 'b/3.txt', 'b/c/4.txt']
+            expected = ["1.txt", "a/2.txt", "b/3.txt", "b/c/4.txt"]
             assert get_files(path, prefix=False, recursive=True) == expected
 
         def test_prefix_true(self):
             path = _setup_tree()
             expected = [
-                f'{path}/1.txt',
-                f'{path}/a/2.txt',
-                f'{path}/b/3.txt',
-                f'{path}/b/c/4.txt'
+                f"{path}/1.txt",
+                f"{path}/a/2.txt",
+                f"{path}/b/3.txt",
+                f"{path}/b/c/4.txt",
             ]
             assert get_files(path, prefix=True, recursive=True) == expected
 
         def test_path_is_file(self):
             with pytest.raises(NotADirectoryError):
                 path = _setup_file()
                 get_files(path)
 
         def test_path_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 get_files(get_unique_path())
 
         def test_iter(self):
-            r = get_files('', iter_=True)
+            r = get_files("", iter_=True)
             assert is_iterator(r)
 
         def test_glob(self):
             path = _setup_tree_2()
-            assert get_files(f'{path}/*.py') == [f'{path}/1.py']
+            assert get_files(f"{path}/*.py") == [f"{path}/1.py"]
 
         def test_glob_recursive(self):
             path = _setup_tree_2()
-            expected = [f'{path}/1.py', f'{path}/a/2.py', f'{path}/a/a/6.py', f'{path}/b/a/5.py']
-            assert get_files(f'{path}/**/*.py') == expected
+            expected = [
+                f"{path}/1.py",
+                f"{path}/a/2.py",
+                f"{path}/a/a/6.py",
+                f"{path}/b/a/5.py",
+            ]
+            assert get_files(f"{path}/**/*.py") == expected
 
         def test_only_conflict(self):
             with pytest.raises(ValueError):
-                _get_all('', only_files=True, only_dirs=True)
+                _get_all("", only_files=True, only_dirs=True)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_prefix(self, mistake):
             with pytest.raises(TypeError):
-                get_files('', prefix=mistake)
+                get_files("", prefix=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_glob(self, mistake):
             with pytest.raises(TypeError):
-                get_files('', glob=mistake)
+                get_files("", glob=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_iter_(self, mistake):
             with pytest.raises(TypeError):
-                get_files('', iter_=mistake)
+                get_files("", iter_=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 get_files(mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_recursive(self, mistake):
             with pytest.raises(TypeError):
-                get_files('', recursive=mistake)
+                get_files("", recursive=mistake)
 
         def test_recursive(self):
             path = _setup_tree()
             assert get_files(path, recursive=True) == [
-                f'{path}/1.txt',
-                f'{path}/a/2.txt',
-                f'{path}/b/3.txt',
-                f'{path}/b/c/4.txt',
+                f"{path}/1.txt",
+                f"{path}/a/2.txt",
+                f"{path}/b/3.txt",
+                f"{path}/b/c/4.txt",
             ]
 
         def test_sorted(self):
             path = _setup_tree()
-            _ = _setup_tree(path + '/b/{}')
+            _ = _setup_tree(path + "/b/{}")
             assert get_files(path, iter_=False, recursive=True) == [
-                f'{path}/1.txt',
-                f'{path}/a/2.txt',
-                f'{path}/b/1/1.txt',
-                f'{path}/b/1/a/2.txt',
-                f'{path}/b/1/b/3.txt',
-                f'{path}/b/1/b/c/4.txt',
-                f'{path}/b/3.txt',
-                f'{path}/b/c/4.txt',
+                f"{path}/1.txt",
+                f"{path}/a/2.txt",
+                f"{path}/b/1/1.txt",
+                f"{path}/b/1/a/2.txt",
+                f"{path}/b/1/b/3.txt",
+                f"{path}/b/1/b/c/4.txt",
+                f"{path}/b/3.txt",
+                f"{path}/b/c/4.txt",
             ]
 
         def test_returns_same_type_as_input(self):
             path = _setup_tree()
             result = get_files(path, recursive=True)
             assert all(isinstance(p, str) for p in result)
 
@@ -1313,21 +1386,21 @@
             assert is_dir_empty(path)
 
         def test_is_file(self):
             with pytest.raises(NotADirectoryError):
                 file = _setup_file()
                 clear_dir(file)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_create_missing(self, mistake):
             path = get_unique_path()
             with pytest.raises(TypeError):
                 clear_dir(path, create_missing=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 clear_dir(mistake)
 
     # noinspection PyTypeChecker
     class Test_is_dir_empty:
         def test_empty(self):
@@ -1337,46 +1410,46 @@
         def test_is_file(self):
             with pytest.raises(NotADirectoryError):
                 path = _setup_file()
                 is_dir_empty(path)
 
         def test_missing_error(self):
             with pytest.raises(FileNotFoundError):
-                is_dir_empty(get_unique_path(), missing='error')
+                is_dir_empty(get_unique_path(), missing="error")
 
         def test_missing_false(self):
             path = get_unique_path()
             assert is_dir_empty(path, missing=False) is False
 
         def test_missing_true(self):
             path = get_unique_path()
             assert is_dir_empty(path, missing=True) is True
 
         def test_non_empty(self):
             path, _ = _setup_dir_and_file()
             assert not is_dir_empty(path)
 
-        @pytest.mark.parametrize('mistake', [[], '', 0, None])
+        @pytest.mark.parametrize("mistake", [[], "", 0, None])
         def test_precondition_missing(self, mistake):
             with pytest.raises(ValueError):
                 path = get_unique_path()
                 is_dir_empty(path, missing=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 is_dir_empty(mistake)
 
     # noinspection PyTypeChecker
     class Test_mkdir:
         def test_create(self):
             path = _setup_dir()
             assert Path(path).is_dir()
 
-            path = _setup_dir('a/{}/b')
+            path = _setup_dir("a/{}/b")
             assert Path(path).is_dir()
 
         def test_exists_error(self):
             with pytest.raises(FileExistsError):
                 path = _setup_dir()
                 make_dir(path, exists_ok=False)
 
@@ -1393,43 +1466,43 @@
         def test_is_file(self):
             with pytest.raises(NotADirectoryError):
                 path = _setup_file()
                 make_dir(path)
 
         def test_no_parents(self):
             with pytest.raises(FileNotFoundError):
-                d = get_unique_path('parent/{}/child')
+                d = get_unique_path("parent/{}/child")
                 make_dir(d, create_parents=False)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_create_parents(self, mistake):
             with pytest.raises(TypeError):
                 make_dir(get_unique_path(), create_parents=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_exists_ok(self, mistake):
             with pytest.raises(TypeError):
                 make_dir(get_unique_path(), exists_ok=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 make_dir(mistake)
 
 
 class TestGroup_misc_file:
     # noinspection PyTypeChecker
     class Test_is_file_empty:
         def test_is_dir(self):
             with pytest.raises(IsADirectoryError):
                 is_file_empty(_setup_dir())
 
         def test_missing_error(self):
             with pytest.raises(FileNotFoundError):
-                is_file_empty(get_unique_path(), missing='error')
+                is_file_empty(get_unique_path(), missing="error")
 
         def test_missing_false(self):
             path = get_unique_path()
             assert is_file_empty(path, missing=False) is False
 
         def test_missing_true(self):
             path = get_unique_path()
@@ -1438,296 +1511,298 @@
         def test_empty(self):
             path = get_unique_path()
             Path(path).touch()
             assert is_file_empty(path)
 
         def test_non_empty(self):
             path = get_unique_path()
-            Path(path).write_text('hello')
+            Path(path).write_text("hello")
             assert not is_file_empty(path)
 
-        @pytest.mark.parametrize('mistake', [[], '', 0, None])
+        @pytest.mark.parametrize("mistake", [[], "", 0, None])
         def test_precondition_missing(self, mistake):
             with pytest.raises(ValueError):
                 path = get_unique_path()
                 is_file_empty(path, missing=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 is_file_empty(mistake)
 
 
 class TestGroup_move:
     # noinspection PyTypeChecker
     class Test_move_dir:
         def test_dest_is_dir(self):
-            src = Path(_setup_tree('{}_src'))
-            src_copy = Path(get_unique_path('{}_src_copy'))
+            src = Path(_setup_tree("{}_src"))
+            src_copy = Path(get_unique_path("{}_src_copy"))
             copy_dir(src, src_copy)
 
-            dest = get_unique_path('{}_dest')
+            dest = get_unique_path("{}_dest")
             move_dir(src, dest)
             _check_tree(src_copy, dest)
             assert not src.exists()
 
-            src = Path(_setup_tree('{}_src'))
-            src_copy = Path(get_unique_path('{}_src_copy'))
+            src = Path(_setup_tree("{}_src"))
+            src_copy = Path(get_unique_path("{}_src_copy"))
             copy_dir(src, src_copy)
 
-            dest = Path(get_unique_path('{}_dest'))
-            move_dir(src, dest/src.name)
-            _check_tree(src_copy/src.name, dest/src.name)
+            dest = Path(get_unique_path("{}_dest"))
+            move_dir(src, dest / src.name)
+            _check_tree(src_copy / src.name, dest / src.name)
             assert not src.exists()
 
         def test_dest_is_file(self):
             with pytest.raises(NotADirectoryError):
                 src = _setup_dir()
                 dest = _setup_file()
                 move_dir(src, dest)
 
         def test_dir_exists_error(self):
             with pytest.raises(FileExistsError):
                 src = _setup_tree()
                 dest = _setup_tree()
-                move_dir(src, dest, dir_exists='error', file_exists='skip')
+                move_dir(src, dest, dir_exists="error", file_exists="skip")
 
         def test_dir_exists_merge(self):
             src, src_file = _setup_dir_and_file()
-            _setup_tree(src + '/{}')
+            _setup_tree(src + "/{}")
             src_dirs = get_dirs(src, prefix=False, recursive=True)
 
             dest = _setup_tree()
-            move_dir(src, dest, dir_exists='merge', file_exists='skip')
+            move_dir(src, dest, dir_exists="merge", file_exists="skip")
 
             dest_dirs = get_dirs(dest, prefix=False, recursive=True)
             assert set(src_dirs).difference(dest_dirs) == set()
             assert set(dest_dirs).difference(src_dirs) != set()
 
         def test_dir_exists_replace(self):
             src, src_file = _setup_dir_and_file()
             src_tree = get_all(src, prefix=False, recursive=True)
             src_tree_2 = set(get_all(src, recursive=True))
 
             dest = _setup_tree()
-            move_dir(src, dest, dir_exists='replace', file_exists='skip')
+            move_dir(src, dest, dir_exists="replace", file_exists="skip")
 
             dest_tree = get_all(dest, prefix=False, recursive=True)
             assert src_tree == dest_tree
 
             dest_tree = set(get_all(dest, recursive=True))
             pairs = {(fn, fn.replace(src, dest)) for fn in src_tree_2 | dest_tree}
             pairs = {(Path(s), Path(d)) for s, d in pairs if Path(s).is_file()}
             assert all((s.read_text() == d.read_text()) for s, d in pairs)
 
         def test_dir_exists_skip(self):
             src, src_file = _setup_dir_and_file()
             dest, dest_file = _setup_dir_and_file()
-            make_dir(f'{dest}/subdir')
+            make_dir(f"{dest}/subdir")
 
-            move_dir(src, dest, dir_exists='skip', file_exists='replace')
+            move_dir(src, dest, dir_exists="skip", file_exists="replace")
             assert Path(dest_file).read_text() != Path(src_file).read_text()
-            assert Path(f'{dest}/subdir').is_dir()
+            assert Path(f"{dest}/subdir").is_dir()
 
         def test_file_exists_error(self):
             with pytest.raises(FileExistsError):
                 src = _setup_tree()
                 dest = _setup_tree()
-                move_dir(src, dest, dir_exists='merge', file_exists='error')
+                move_dir(src, dest, dir_exists="merge", file_exists="error")
 
         def test_file_exists_replace(self):
             src, src_file = _setup_dir_and_file()
             dest, dest_file = _setup_dir_and_file()
             src_file_text = Path(src_file).read_text()
 
-            move_dir(src, dest, dir_exists='merge', file_exists='replace')
+            move_dir(src, dest, dir_exists="merge", file_exists="replace")
             assert Path(dest_file).read_text() == src_file_text
 
         def test_file_exists_skip(self):
             src, src_file = _setup_dir_and_file()
             dest, dest_file = _setup_dir_and_file()
 
             src_file_text = Path(src_file).read_text()
             original = Path(dest_file).read_text()
 
-            move_dir(src, dest, dir_exists='merge', file_exists='skip')
+            move_dir(src, dest, dir_exists="merge", file_exists="skip")
             assert Path(dest_file).read_text() != src_file_text
             assert Path(dest_file).read_text() == original
 
         def test_make_dirs_false(self):
             with pytest.raises(FileNotFoundError):
                 with tempfile.TemporaryDirectory() as d:
-                    src = get_unique_path(d + '/{}_src')
-                    dest = get_unique_path(d + '/{}_dest')
+                    src = get_unique_path(d + "/{}_src")
+                    dest = get_unique_path(d + "/{}_dest")
                     make_dir(src)
                     move_dir(src, dest, make_dirs=False)
 
         def test_make_dirs_true(self):
             with tempfile.TemporaryDirectory() as d:
                 src = _setup_tree()
                 src_name = Path(src).name
-                src_copy = Path(get_unique_path('{}_src_copy'))
+                src_copy = Path(get_unique_path("{}_src_copy"))
                 copy_dir(src, src_copy)
 
-                dest = get_unique_path(d + '/{}_dest')
+                dest = get_unique_path(d + "/{}_dest")
                 move_dir(src, dest, make_dirs=True)
-                _check_tree(src_copy/src_name, f'{dest}/{src_name}')
+                _check_tree(src_copy / src_name, f"{dest}/{src_name}")
 
                 src = _setup_tree()
                 src_name = Path(src).name
-                src_copy = Path(get_unique_path('{}_src_copy'))
+                src_copy = Path(get_unique_path("{}_src_copy"))
                 copy_dir(src, src_copy)
 
-                dest_2 = get_unique_path(d + '/{}_dest_2')
-                move_dir(src, f'{dest_2}/{src_name}', make_dirs=True)
-                _check_tree(src_copy/src_name, f'{dest_2}/{src_name}')
+                dest_2 = get_unique_path(d + "/{}_dest_2")
+                move_dir(src, f"{dest_2}/{src_name}", make_dirs=True)
+                _check_tree(src_copy / src_name, f"{dest_2}/{src_name}")
 
         def test_same_path(self):
             with pytest.raises(ValueError):
                 src = _setup_dir()
                 move_dir(src, src)
 
         def test_src_is_file(self):
             with pytest.raises(NotADirectoryError):
                 src = _setup_file()
-                dest = get_unique_path('{}_new')
+                dest = get_unique_path("{}_new")
                 move_dir(src, dest)
 
         def test_src_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 src = get_unique_path()
-                move_dir(src, f'{src}_copy')
+                move_dir(src, f"{src}_copy")
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_dest(self, mistake):
             with pytest.raises(TypeError):
-                move_dir('src', mistake)
+                move_dir("src", mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True, 'hello'])
+        @pytest.mark.parametrize("mistake", [0, None, {}, True, "hello"])
         def test_precondition_dir_exists(self, mistake):
             with pytest.raises(ValueError):
-                move_dir('src', 'dest', dir_exists=mistake)
+                move_dir("src", "dest", dir_exists=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, 'hello'])
+        @pytest.mark.parametrize("mistake", [0, None, {}, "hello"])
         def test_precondition_file_exists(self, mistake):
             with pytest.raises(ValueError):
-                move_dir('src', 'dest', file_exists=mistake)
+                move_dir("src", "dest", file_exists=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_make_dirs(self, mistake):
             with pytest.raises(TypeError):
                 src, dest = _setup_dir(n=2)
                 move_dir(src, dest, make_dirs=mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_src(self, mistake):
             with pytest.raises(TypeError):
                 # noinspection PyTypeChecker
-                move_dir(mistake, 'dest')
+                move_dir(mistake, "dest")
 
     # noinspection PyTypeChecker
     class Test_move_file:
         def test_dir(self):
             with pytest.raises(IsADirectoryError):
                 src = _setup_dir()
                 dest = get_unique_path()
                 move_file(src, dest)
 
         def test_exists_error(self):
             with pytest.raises(FileExistsError):
                 src, dest = _setup_file(n=2)
-                move_file(src, dest, exists='error')
+                move_file(src, dest, exists="error")
 
         def test_exists_replace(self):
             src, dest = _setup_file(n=2)
             expected_text = Path(src).read_text()
-            move_file(src, dest, exists='replace')
+            move_file(src, dest, exists="replace")
 
             text = Path(dest).read_text()
             assert text == expected_text
             assert text != dest
             assert not Path(src).exists()
 
         def test_exists_skip(self):
             src, dest = _setup_file(n=2)
-            move_file(src, dest, exists='skip')
+            move_file(src, dest, exists="skip")
 
             text = Path(dest).read_text()
             assert text != Path(src).read_text()
             assert text == dest
             assert Path(src).exists()
 
         def test_make_dirs_false(self):
             with pytest.raises(FileNotFoundError):
                 src = _setup_file()
-                dest = get_unique_path('{}/a/b/c/')
+                dest = get_unique_path("{}/a/b/c/")
                 move_file(src, dest, make_dirs=False)
 
         def test_make_dirs_true(self):
             src = _setup_file()
             dest = _setup_path()
             move_file(src, dest, make_dirs=True)
             assert Path(dest).read_text() == src
             assert not Path(src).exists()
 
         def test_same_path(self):
             with pytest.raises(ValueError):
                 src = _setup_file()
                 move_file(src, src)
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_src(self, mistake):
             with pytest.raises(TypeError):
-                move_file(mistake, 'a')
+                move_file(mistake, "a")
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_precondition_dest(self, mistake):
             with pytest.raises(TypeError):
-                move_file('a', mistake)
+                move_file("a", mistake)
 
-        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
+        @pytest.mark.parametrize("mistake", all_types_besides("booleans"))
         def test_precondition_make_dirs(self, mistake):
             with pytest.raises(TypeError):
                 src, dest = _setup_file(n=2)
                 move_file(src, dest, make_dirs=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, 'hello'])
+        @pytest.mark.parametrize("mistake", [0, None, {}, "hello"])
         def test_precondition_exists(self, mistake):
             src, dest = _setup_file(n=2)
             with pytest.raises(ValueError):
                 move_file(src, dest, exists=mistake)
 
 
 class TestGroup_paths:
     class Test_get_unique_path:
         def test_consecutive_values(self):
             root = Path(_setup_dir())
             for i in range(1, 11):
-                file = get_unique_path(root/'{}')
-                assert file == Path(f'{root}/{i}')
+                file = get_unique_path(root / "{}")
+                assert file == Path(f"{root}/{i}")
                 Path(file).touch()
 
-        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
+        @pytest.mark.parametrize("mistake", all_types_besides(["str", "path"]))
         def test_invalid_pattern_type(self, mistake):
             with pytest.raises(TypeError):
                 get_unique_path(mistake)
 
-        @pytest.mark.parametrize('mistake', ['', '{0}', '{a}', '{:f}'])
+        @pytest.mark.parametrize("mistake", ["", "{0}", "{a}", "{:f}"])
         def test_invalid_placeholder(self, mistake):
             with pytest.raises(ValueError):
                 get_unique_path(mistake)
 
         def test_keeps_slash_at_the_end(self):
-            assert get_unique_path('{}/').endswith('/')
+            assert get_unique_path("{}/").endswith("/")
 
         def test_returns_same_type_as_input(self):
-            assert isinstance(get_unique_path('{}'), str)
-            assert isinstance(get_unique_path(Path('{}')), Path)
+            assert isinstance(get_unique_path("{}"), str)
+            assert isinstance(get_unique_path(Path("{}")), Path)
 
-        @pytest.mark.parametrize('mistake', ['hello_{}', '{}', './{}', '/a/{}', '/{}/a', '{:06d}'])
+        @pytest.mark.parametrize(
+            "mistake", ["hello_{}", "{}", "./{}", "/a/{}", "/{}/a", "{:06d}"]
+        )
         def test_not_exists(self, mistake):
             path = get_unique_path(mistake)
             assert not Path(path).exists()
 
 
 def _check_tree(src, dest):
     for src_item in Path(src).iterdir():
@@ -1740,45 +1815,50 @@
         else:
             assert dest_item.is_file()
 
 
 def _setup_tree(path=None):
     path = _setup_path(path)
 
-    for d in [path, f'{path}/a', f'{path}/b', f'{path}/b/c']:
+    for d in [path, f"{path}/a", f"{path}/b", f"{path}/b/c"]:
         _setup_dir(d)
 
-    for f in [f'{path}/1.txt', f'{path}/a/2.txt', f'{path}/b/3.txt', f'{path}/b/c/4.txt']:
+    for f in [
+        f"{path}/1.txt",
+        f"{path}/a/2.txt",
+        f"{path}/b/3.txt",
+        f"{path}/b/c/4.txt",
+    ]:
         _setup_file(f)
 
     return str(path)
 
 
 def _setup_tree_2(path=None):
     path = _setup_tree(path)
 
-    make_dir(f'{path}/a/a')
-    make_dir(f'{path}/b/a')
-    make_dir(f'{path}/b/c/a')
-    make_dir(f'{path}/b/c/a/d')
-
-    Path(f'{path}/1.py').touch()
-    Path(f'{path}/a/2.py').touch()
-    Path(f'{path}/b/a/5.py').touch()
-    Path(f'{path}/a/a/6.py').touch()
+    make_dir(f"{path}/a/a")
+    make_dir(f"{path}/b/a")
+    make_dir(f"{path}/b/c/a")
+    make_dir(f"{path}/b/c/a/d")
+
+    Path(f"{path}/1.py").touch()
+    Path(f"{path}/a/2.py").touch()
+    Path(f"{path}/b/a/5.py").touch()
+    Path(f"{path}/a/a/6.py").touch()
 
     return path
 
 
 def _setup_dir_and_file(path_dir=None, filename=None):
     if filename is None:
-        filename = 'file'
+        filename = "file"
 
     dir_ = _setup_dir(path_dir)
-    file = _setup_file(Path(dir_)/filename)
+    file = _setup_file(Path(dir_) / filename)
     return dir_, file
 
 
 def _setup_file(path=None, n=1):
     files = []
     for _ in range(n):
         file = _setup_path(path)
@@ -1805,11 +1885,11 @@
     else:
         return dirs
 
 
 def _setup_path(path=None):
     if path is None:
         return get_unique_path()
-    elif '{}' in str(path):
+    elif "{}" in str(path):
         return get_unique_path(path)
     else:
         return str(path)
```

### Comparing `katalytic-0.2.2/tests/test_maths.py` & `katalytic-0.3.0/tests/test_maths.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,138 +1,157 @@
 import pytest
-from katalytic.data import all_types_besides
+
+from katalytic._pkg import all_types_besides
 from katalytic.maths import clip, L1, L2, min_max
 
 
 class Test_L1:
-    @pytest.mark.parametrize('x', all_types_besides(['int', 'float']))
+    @pytest.mark.parametrize("x", all_types_besides(["int", "float"]))
     def test_wrong_value(self, x):
         with pytest.raises(ValueError):
             L1(x, 1)
 
         with pytest.raises(ValueError):
             L1(1, x)
 
-    @pytest.mark.parametrize('a, b', [
-        ([], []),
-        ([], [1]),
-        ([1, 2], [1]),
-        ([[1]], [1])
-    ])
+    @pytest.mark.parametrize("a, b", [([], []), ([], [1]), ([1, 2], [1]), ([[1]], [1])])
     def test_wrong_format(self, a, b):
         with pytest.raises(ValueError):
             L1(a, b)
 
-    @pytest.mark.parametrize('a, b, expected', [
-        (1, 1, 0),
-        (1, 5, 4),
-        (-5, 1, 6),
-        ([1], [3], 2),
-        ([3], [1], 2),
-        ([1, 2], [3, 4], 4),
-        ([1.1, 2], [3, 3.5], 3.4),
-        ([1, 10, 1], (10, 10, 10), 18),
-    ])
+    @pytest.mark.parametrize(
+        "a, b, expected",
+        [
+            (1, 1, 0),
+            (1, 5, 4),
+            (-5, 1, 6),
+            ([1], [3], 2),
+            ([3], [1], 2),
+            ([1, 2], [3, 4], 4),
+            ([1.1, 2], [3, 3.5], 3.4),
+            ([1, 10, 1], (10, 10, 10), 18),
+        ],
+    )
     def test_ok(self, a, b, expected):
         assert L1(a, b) == expected
 
 
 class Test_L2:
-    @pytest.mark.parametrize('x', all_types_besides(['int', 'float']))
+    @pytest.mark.parametrize("x", all_types_besides(["int", "float"]))
     def test_wrong_value(self, x):
         with pytest.raises(ValueError):
             L2(x, 1)
 
         with pytest.raises(ValueError):
             L2(1, x)
 
-    @pytest.mark.parametrize('a, b', [
-        ([], []),
-        ([], [1]),
-        ([1, 2], [1]),
-        ([[1]], [1]),
-        (['1'], [1]),
-        ([True], [1]),
-    ])
+    @pytest.mark.parametrize(
+        "a, b",
+        [
+            ([], []),
+            ([], [1]),
+            ([1, 2], [1]),
+            ([[1]], [1]),
+            (["1"], [1]),
+            ([True], [1]),
+        ],
+    )
     def test_wrong_value_2(self, a, b):
         with pytest.raises(ValueError):
             L2(a, b)
 
-    @pytest.mark.parametrize('a, b, expected', [
-        (1, 1, 0),
-        (1, 5, 4),
-        (-5, 1, 6),
-        ([1], [3], 2),
-        ([3], [1], 2),
-        ([1, 2], [5, 6], 5.656854),
-        ([1, 10, 1], (10, 10, 10), 12.727922),
-    ])
+    @pytest.mark.parametrize(
+        "a, b, expected",
+        [
+            (1, 1, 0),
+            (1, 5, 4),
+            (-5, 1, 6),
+            ([1], [3], 2),
+            ([3], [1], 2),
+            ([1, 2], [5, 6], 5.656854),
+            ([1, 10, 1], (10, 10, 10), 12.727922),
+        ],
+    )
     def test_ok(self, a, b, expected):
         assert round(L2(a, b), 6) == expected
 
 
 class Test_min_max:
-    @pytest.mark.parametrize('wrong_type', all_types_besides(['iterables']))
+    @pytest.mark.parametrize("wrong_type", all_types_besides(["iterables"]))
     def test_not_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             min_max(wrong_type)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides(['callables', 'none']))
+    @pytest.mark.parametrize("wrong_type", all_types_besides(["callables", "none"]))
     def test_not_a_callable(self, wrong_type):
         with pytest.raises(TypeError):
             min_max([], key=wrong_type)
 
-    @pytest.mark.parametrize('data', [
-        [],
-        (),
-        iter([]),
-    ])
+    @pytest.mark.parametrize(
+        "data",
+        [
+            [],
+            (),
+            iter([]),
+        ],
+    )
     def test_empty_without_default(self, data):
         with pytest.raises(ValueError):
             min_max(data)
 
-    @pytest.mark.parametrize('data, default', [
-        ([], 'default_1'),
-        ((), 'default_2'),
-        (iter([]), 'default_3'),
-    ])
+    @pytest.mark.parametrize(
+        "data, default",
+        [
+            ([], "default_1"),
+            ((), "default_2"),
+            (iter([]), "default_3"),
+        ],
+    )
     def test_empty_with_default(self, data, default):
         assert min_max(data, default=default) == default
 
-
-    @pytest.mark.parametrize('data, expected', [
-        ({3,2,1}, (1, 3)),
-        ([3, 2, -1, 100], (-1, 100)),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ({3, 2, 1}, (1, 3)),
+            ([3, 2, -1, 100], (-1, 100)),
+        ],
+    )
     def test_happy_path(self, data, expected):
         assert min_max(data) == expected
 
 
 class Test_clip:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('numbers'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("numbers"))
     def test_wrong_type_x(self, wrong_type):
         with pytest.raises(TypeError):
             clip(wrong_type, 1, 2)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('numbers'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("numbers"))
     def test_wrong_type_min(self, wrong_type):
         with pytest.raises(TypeError):
             clip(1, wrong_type, 2)
 
-    @pytest.mark.parametrize('wrong_type', all_types_besides('numbers'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("numbers"))
     def test_wrong_type_max(self, wrong_type):
         with pytest.raises(TypeError):
             clip(1, 2, wrong_type)
 
-    @pytest.mark.parametrize('args, expected', [
-        ((2, 1, 3), 2),
-        ((2.5, 2, 3), 2.5),
-    ])
+    @pytest.mark.parametrize(
+        "args, expected",
+        [
+            ((2, 1, 3), 2),
+            ((2.5, 2, 3), 2.5),
+        ],
+    )
     def test_within_bounds(self, args, expected):
         assert clip(*args) == expected
 
-    @pytest.mark.parametrize('args, expected', [
-        ((20, 1, 3), 3),
-        ((0.5, 2, 3), 2),
-    ])
+    @pytest.mark.parametrize(
+        "args, expected",
+        [
+            ((20, 1, 3), 3),
+            ((0.5, 2, 3), 2),
+        ],
+    )
     def test_outside_bounds(self, args, expected):
         assert clip(*args) == expected
```

### Comparing `katalytic-0.2.2/tests/test_meta.py` & `katalytic-0.3.0/tests/test_meta.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,79 @@
 from pathlib import Path
 
+
 import pytest as pytest
-from katalytic.data import all_types_besides
+from katalytic._pkg import all_types_besides
 from katalytic.meta import extract_call_stack_info, reference_caller_function
 
 
-def _f0(depth): return reference_caller_function(depth=depth)
-def _f1(depth): return _f0(depth)
-def _f2(depth): return _f1(depth)
+def _f0(depth):
+    return reference_caller_function(depth=depth)
+
+
+def _f1(depth):
+    return _f0(depth)
+
+
+def _f2(depth):
+    return _f1(depth)
+
 
+def _g0(depth):
+    return extract_call_stack_info(depth=depth)
 
-def _g0(depth): return extract_call_stack_info(depth=depth)
-def _g1(depth): return _g0(depth)
-def _g2(depth): return _g1(depth)
+
+def _g1(depth):
+    return _g0(depth)
+
+
+def _g2(depth):
+    return _g1(depth)
 
 
 class _Nested_0:
     class Nested_1:
-        def f0(depth): return extract_call_stack_info(depth=depth)
-        def f1(depth): return _Nested_0.Nested_1.f0(depth)
-        def f2(depth): return _Nested_0.Nested_1.f1(depth)
+        def f0(depth):
+            return extract_call_stack_info(depth=depth)
+
+        def f1(depth):
+            return _Nested_0.Nested_1.f0(depth)
+
+        def f2(depth):
+            return _Nested_0.Nested_1.f1(depth)
 
 
 class Test_extract_call_stack_info:
-    @pytest.mark.parametrize('caller, depth, expected', [
-        (_Nested_0.Nested_1.f1, 0, _Nested_0.Nested_1.f0),
-        (_Nested_0.Nested_1.f1, 1, _Nested_0.Nested_1.f1),
-        (_Nested_0.Nested_1.f2, 0, _Nested_0.Nested_1.f0),
-        (_Nested_0.Nested_1.f2, 1, _Nested_0.Nested_1.f1),
-        (_Nested_0.Nested_1.f2, 2, _Nested_0.Nested_1.f2),
-    ])
+    @pytest.mark.parametrize(
+        "caller, depth, expected",
+        [
+            (_Nested_0.Nested_1.f1, 0, _Nested_0.Nested_1.f0),
+            (_Nested_0.Nested_1.f1, 1, _Nested_0.Nested_1.f1),
+            (_Nested_0.Nested_1.f2, 0, _Nested_0.Nested_1.f0),
+            (_Nested_0.Nested_1.f2, 1, _Nested_0.Nested_1.f1),
+            (_Nested_0.Nested_1.f2, 2, _Nested_0.Nested_1.f2),
+        ],
+    )
     def test_depth_ok_nested(self, caller, depth, expected):
         path, func, line = caller(depth=depth)
 
         assert path == str(Path(__file__).resolve())
         assert func == expected
         assert isinstance(line, int) and line > 0
 
-    @pytest.mark.parametrize('caller, depth, expected', [
-        (_g1, 0, _g0),
-        (_g1, 1, _g1),
-        (_g2, 0, _g0),
-        (_g2, 1, _g1),
-        (_g2, 2, _g2),
-    ])
+    @pytest.mark.parametrize(
+        "caller, depth, expected",
+        [
+            (_g1, 0, _g0),
+            (_g1, 1, _g1),
+            (_g2, 0, _g0),
+            (_g2, 1, _g1),
+            (_g2, 2, _g2),
+        ],
+    )
     def test_depth_ok(self, caller, depth, expected):
         path, func, line = caller(depth=depth)
 
         assert path == str(Path(__file__).resolve())
         assert func == expected
         assert isinstance(line, int) and line > 0
 
@@ -56,37 +82,40 @@
             _g1(-1)
 
     def test_depth_should_not_be_larger_than_the_stack(self):
         with pytest.raises(ValueError):
             # Use a large number because of the pytest internal calls
             _g1(100)
 
-    @pytest.mark.parametrize('depth', all_types_besides('int'))
+    @pytest.mark.parametrize("depth", all_types_besides("int"))
     def test_precondition_depth_should_be_an_integer(self, depth):
         with pytest.raises(TypeError):
             _g1(depth)
 
 
 class Test_reference_caller_function:
-    @pytest.mark.parametrize('caller, depth, expected', [
-        (_f1, 0, _f0),
-        (_f1, 1, _f1),
-        (_f2, 0, _f0),
-        (_f2, 1, _f1),
-        (_f2, 2, _f2),
-    ])
+    @pytest.mark.parametrize(
+        "caller, depth, expected",
+        [
+            (_f1, 0, _f0),
+            (_f1, 1, _f1),
+            (_f2, 0, _f0),
+            (_f2, 1, _f1),
+            (_f2, 2, _f2),
+        ],
+    )
     def test_depth_ok(self, caller, depth, expected):
         assert caller(depth=depth) == expected
 
     def test_precondition_depth_should_be_positive(self):
         with pytest.raises(ValueError):
             _f1(-1)
 
     def test_depth_should_not_be_larger_than_the_stack(self):
         with pytest.raises(ValueError):
             # Use a large number because of the pytest internal calls
             _f1(100)
 
-    @pytest.mark.parametrize('depth', all_types_besides('int'))
+    @pytest.mark.parametrize("depth", all_types_besides("int"))
     def test_precondition_depth_should_be_an_integer(self, depth):
         with pytest.raises(TypeError):
             _f1(depth)
```

### Comparing `katalytic-0.2.2/tests/test_pkg.py` & `katalytic-0.3.0/tests/test_pkg.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,105 @@
 import pytest
 
+
 # noinspection PyProtectedMember
-from katalytic._pkg import _check, find_functions_marked_with, get_modules, get_version, mark
+from katalytic._pkg import (
+    _check,
+    find_functions_marked_with,
+    get_modules,
+    get_version,
+    mark,
+)
 from katalytic.katalytic import __version__
 
 
 class Test_check:
     def test_all(self):
-        assert _check(None, '') is False
-        assert _check('load', 'save') is False
-        assert _check('load', 'save::*') is False
-        assert _check('save::txt', 'load::*') is False
-        assert _check('load::txt', 'load::') is False
-
-        assert _check('load::txt', 'load::txt') is True
-        assert _check('load::txt', 'load::*') is True
-        assert _check('load::image::png', 'load::*') is True
+        assert _check(None, "") is False
+        assert _check("load", "save") is False
+        assert _check("load", "save::*") is False
+        assert _check("save::txt", "load::*") is False
+        assert _check("load::txt", "load::") is False
+
+        assert _check("load::txt", "load::txt") is True
+        assert _check("load::txt", "load::*") is True
+        assert _check("load::image::png", "load::*") is True
 
 
 class Test_mark:
     def test_internals(self):
-        def f1(): pass
-
-        @mark('_test_group-1')
-        def f2(): pass
-
-        @mark('_test_group-2')
-        @mark('_test_group-1')
-        def f3(): pass
+        def f1():
+            pass
 
-        assert not hasattr(f1, '__katalytic_marks__')
-        assert f2.__katalytic_marks__ == ('_test_group-1', )
-        assert f3.__katalytic_marks__ == ('_test_group-2', '_test_group-1')
+        @mark("_test_group-1")
+        def f2():
+            pass
+
+        @mark("_test_group-2")
+        @mark("_test_group-1")
+        def f3():
+            pass
+
+        assert not hasattr(f1, "__katalytic_marks__")
+        assert f2.__katalytic_marks__ == ("_test_group-1",)
+        assert f3.__katalytic_marks__ == ("_test_group-2", "_test_group-1")
 
-    @pytest.mark.parametrize('group', [0, None, {}, True])
+    @pytest.mark.parametrize("group", [0, None, {}, True])
     def test_TypeError(self, group):
         with pytest.raises(TypeError):
             # noinspection PyTypeChecker
             @mark(group)
-            def f1(): pass
+            def f1():
+                pass
 
-    @pytest.mark.parametrize('group', ['', ' ', ' \n ', '\t \t', 'no \t tabs', 'no \n newlines'])
+    @pytest.mark.parametrize(
+        "group", ["", " ", " \n ", "\t \t", "no \t tabs", "no \n newlines"]
+    )
     def test_ValueError(self, group):
         with pytest.raises(ValueError):
+
             @mark(group)
-            def f1(): pass
+            def f1():
+                pass
 
 
 class Test_get_functions_in_group:
     def test_empty(self):
-        assert find_functions_marked_with('__not-used') == []
-        assert find_functions_marked_with('__test_3') == []
+        assert find_functions_marked_with("__not-used") == []
+        assert find_functions_marked_with("__test_3") == []
 
     def test_pattern(self):
-        found = find_functions_marked_with('__test_3*')
+        found = find_functions_marked_with("__test_3*")
         found = [(name, groups) for name, _, groups in found]
         assert found == [
-            ('__test', ['__test_300']),
-            ('__test_2', ['__test_3::a', '__test_3::b'])
+            ("__test", ["__test_300"]),
+            ("__test_2", ["__test_3::a", "__test_3::b"]),
         ]
 
     def test_exact(self):
-        found = find_functions_marked_with('__test_1')
+        found = find_functions_marked_with("__test_1")
         found = [(name, groups) for name, _, groups in found]
-        assert found == [('__test', ['__test_1'])]
+        assert found == [("__test", ["__test_1"])]
 
-        found = find_functions_marked_with('__test_2')
+        found = find_functions_marked_with("__test_2")
         found = [(name, groups) for name, _, groups in found]
-        assert found == [
-            ('__test', ['__test_2']),
-            ('__test_2', ['__test_2'])
-        ]
+        assert found == [("__test", ["__test_2"]), ("__test_2", ["__test_2"])]
 
 
 class Test_get_modules:
     def test_all(self):
         modules = get_modules()
-        modules = [m.__name__.replace('.__init__', '') for m in modules]
-        assert 'katalytic._pkg' in modules
-        assert all(m.startswith('katalytic') for m in modules)
+        modules = [m.__name__.replace(".__init__", "") for m in modules]
+        assert "katalytic._pkg" in modules
+        assert all(m.startswith("katalytic") for m in modules)
 
 
 class Test_version:
     def test_is_ok(self):
-        v, v_info = get_version('katalytic')
+        v, v_info = get_version("katalytic")
 
         assert v is not None
         assert v_info is not None
         assert v == __version__
 
-        v2 = v.replace('+editable', '.editable')
-        assert v2 == '.'.join(str(i) for i in v_info)
+        v2 = v.replace("+editable", ".editable")
+        assert v2 == ".".join(str(i) for i in v_info)
```

### Comparing `katalytic-0.2.2/PKG-INFO` & `katalytic-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic
-Version: 0.2.2
+Version: 0.3.0
 Summary: We'll take care of the boilerplate, so you can focus on your problems.
 Keywords: automation high-level metaprogramming
 Author-Email: Valentin Neagu <vali19th@protonmail.com>
 License: Copyright 2023 - present, Valentin Neagu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

