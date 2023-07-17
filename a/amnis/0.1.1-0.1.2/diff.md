# Comparing `tmp/amnis-0.1.1.tar.gz` & `tmp/amnis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amnis-0.1.1.tar", last modified: Mon Jul 17 14:37:30 2023, max compression
+gzip compressed data, was "amnis-0.1.2.tar", last modified: Mon Jul 17 16:34:52 2023, max compression
```

## Comparing `amnis-0.1.1.tar` & `amnis-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 14:37:30.298782 amnis-0.1.1/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     1063 2021-09-26 12:41:19.000000 amnis-0.1.1/LICENSE
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       15 2021-09-26 12:44:27.000000 amnis-0.1.1/MANIFEST.in
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     7844 2023-07-17 14:37:30.298782 amnis-0.1.1/PKG-INFO
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     7445 2023-07-17 14:32:48.000000 amnis-0.1.1/README.md
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 14:37:30.298782 amnis-0.1.1/amnis/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       36 2022-09-11 14:43:08.000000 amnis-0.1.1/amnis/__init__.py
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     5502 2022-09-11 15:38:51.000000 amnis-0.1.1/amnis/stream.py
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 14:37:30.298782 amnis-0.1.1/amnis.egg-info/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     7844 2023-07-17 14:37:30.000000 amnis-0.1.1/amnis.egg-info/PKG-INFO
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      188 2023-07-17 14:37:30.000000 amnis-0.1.1/amnis.egg-info/SOURCES.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)        1 2023-07-17 14:37:30.000000 amnis-0.1.1/amnis.egg-info/dependency_links.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)        6 2023-07-17 14:37:30.000000 amnis-0.1.1/amnis.egg-info/top_level.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       38 2023-07-17 14:37:30.298782 amnis-0.1.1/setup.cfg
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      885 2023-07-17 14:33:03.000000 amnis-0.1.1/setup.py
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 16:34:52.864887 amnis-0.1.2/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     1063 2021-09-26 12:41:19.000000 amnis-0.1.2/LICENSE
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       15 2021-09-26 12:44:27.000000 amnis-0.1.2/MANIFEST.in
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     7844 2023-07-17 16:34:52.864887 amnis-0.1.2/PKG-INFO
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     7445 2023-07-17 14:32:48.000000 amnis-0.1.2/README.md
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 16:34:52.864887 amnis-0.1.2/amnis/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       36 2022-09-11 14:43:08.000000 amnis-0.1.2/amnis/__init__.py
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     5639 2023-07-17 16:31:23.000000 amnis-0.1.2/amnis/stream.py
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 16:34:52.864887 amnis-0.1.2/amnis.egg-info/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     7844 2023-07-17 16:34:52.000000 amnis-0.1.2/amnis.egg-info/PKG-INFO
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      188 2023-07-17 16:34:52.000000 amnis-0.1.2/amnis.egg-info/SOURCES.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)        1 2023-07-17 16:34:52.000000 amnis-0.1.2/amnis.egg-info/dependency_links.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)        6 2023-07-17 16:34:52.000000 amnis-0.1.2/amnis.egg-info/top_level.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       38 2023-07-17 16:34:52.864887 amnis-0.1.2/setup.cfg
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      885 2023-07-17 16:33:19.000000 amnis-0.1.2/setup.py
```

### Comparing `amnis-0.1.1/LICENSE` & `amnis-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amnis-0.1.1/PKG-INFO` & `amnis-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amnis
-Version: 0.1.1
+Version: 0.1.2
 Summary: Java like Stream Api for Python
 Home-page: https://github.com/zahash/amnis
 Author: zahash
 Author-email: zahash.z@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `amnis-0.1.1/README.md` & `amnis-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `amnis-0.1.1/amnis/stream.py` & `amnis-0.1.2/amnis/stream.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,30 @@
     "Grouper",
     [
         ("collection", Any),
         ("grouper_fn", Callable[[Any, Any], Any])
     ]
 )
 
+T = TypeVar("T")
+U = TypeVar("U")
+V = TypeVar("V")
 
-class Stream:
-    def __init__(self, iterable: Iterable):
-        self._iterator = iter(iterable)
 
-    def __iter__(self):
+class Stream(Generic[T]):
+    def __init__(self, iterable: Iterable[T]):
+        self._iterator: Iterator[T] = iter(iterable)
+
+    def __iter__(self) -> Iterator[T]:
         return self._iterator
 
-    def __next__(self):
+    def __next__(self) -> T:
         return next(self._iterator)
 
-    def apply(self, fn: Callable[[Iterable], Iterable]) -> "Stream":
+    def apply(self, fn: Callable[[Iterable[T]], Iterable[U]]) -> "Stream[U]":
         return Stream(fn(self))
 
     def catch(self, handler: Callable[["Exception"], Any], err_type=Exception) -> "Stream":
         def _catch(iterable: Iterable) -> Iterable:
             while True:
                 try:
                     yield next(iter(iterable))
@@ -35,138 +39,138 @@
                 except err_type as ex:
                     return_val = handler(ex)
                     if return_val is not None:
                         yield return_val
 
         return self.apply(_catch)
 
-    def map(self, fn: Callable[[Any], Any]) -> "Stream":
+    def map(self, fn: Callable[[T], U]) -> "Stream[U]":
         return self.apply(partial(map, fn))
 
-    def filter(self, fn: Callable[[Any], bool]) -> "Stream":
+    def filter(self, fn: Callable[[T], bool]) -> "Stream[T]":
         return self.apply(partial(filter, fn))
 
-    def flatten(self) -> "Stream":
-        def _flatten(nested_iterable: Iterable) -> Iterable:
+    def flatten(self) -> "Stream[Iterable[T]]":
+        def _flatten(nested_iterable: Iterable[Iterable[T]]) -> Iterable[T]:
             for iterable in nested_iterable:
                 yield from iterable
 
         return self.apply(_flatten)
 
-    def flatmap(self, fn: Callable[[Any], Iterable]) -> "Stream":
+    def flatmap(self, fn: Callable[[T], Iterable[U]]) -> "Stream[U]":
         return self.map(fn).flatten()
 
-    def distinct(self) -> "Stream":
-        def _distinct(iterable: Iterable) -> Iterable:
+    def distinct(self) -> "Stream[T]":
+        def _distinct(iterable: Iterable[T]) -> Iterable[T]:
             seen = set()
             for item in iterable:
                 if item not in seen:
                     yield item
                     seen.add(item)
 
         return self.apply(_distinct)
 
-    def sorted(self) -> "Stream":
+    def sorted(self) -> "Stream[T]":
         return self.apply(sorted)
 
-    def limit(self, n: int) -> "Stream":
-        def _limit(iterable: Iterable, n: int) -> Iterable:
+    def limit(self, n: int) -> "Stream[T]":
+        def _limit(iterable: Iterable[T], n: int) -> Iterable[T]:
             for item in iterable:
                 if n == 0:
                     break
                 yield item
                 n -= 1
 
         return self.apply(partial(_limit, n=max(n, 0)))
 
-    def skip(self, n: int) -> "Stream":
-        def _skip(iterable: Iterable, n: int) -> Iterable:
+    def skip(self, n: int) -> "Stream[T]":
+        def _skip(iterable: Iterable[T], n: int) -> Iterable[T]:
             for item in iterable:
                 if n == 0:
                     yield item
                     break
                 n -= 1
             yield from iterable
 
         return self.apply(partial(_skip, n=max(n, 0)))
 
-    def takeuntil(self, fn: Callable[[Any], bool]) -> "Stream":
-        def _takeuntil(iterable: Iterable) -> Iterable:
+    def takeuntil(self, fn: Callable[[T], bool]) -> "Stream[T]":
+        def _takeuntil(iterable: Iterable[T]) -> Iterable[T]:
             for item in iterable:
                 if not fn(item):
                     break
                 yield item
 
         return self.apply(_takeuntil)
 
-    def skipuntil(self, fn: Callable[[Any], bool]) -> "Stream":
-        def _skipuntil(iterable: Iterable) -> Iterable:
+    def skipuntil(self, fn: Callable[[T], bool]) -> "Stream[T]":
+        def _skipuntil(iterable: Iterable[T]) -> Iterable[T]:
             for item in iterable:
                 if not fn(item):
                     yield item
                     break
 
             yield from iterable
 
         return self.apply(_skipuntil)
 
-    def first(self) -> Optional[Any]:
+    def first(self) -> Optional[T]:
         return self.nth(0)
 
-    def nth(self, n: int) -> Optional[Any]:
+    def nth(self, n: int) -> Optional[T]:
         for item in self:
             if n == 0:
                 return item
             n -= 1
 
-    def last(self) -> Optional[Any]:
+    def last(self) -> Optional[T]:
         last_item = None
         for item in self:
             last_item = item
         return last_item
 
     def collect(self, collector: Callable[[Iterable], Iterable] = iter) -> Union[Sequence, Iterable, AbstractSet]:
         return collector(self)
 
-    def reduce(self, fn: Callable[[Any, Any], Any], initial=None) -> Optional[Any]:
+    def reduce(self, fn: Callable[[T, T], T], initial=None) -> Optional[T]:
         with suppress(TypeError):  # thrown when stream is empty without initial value
             return reduce(fn, self, initial) if initial is not None else reduce(fn, self)
 
-    def max(self, key: Callable[[Any], Any] = lambda x: x) -> Optional[Any]:
+    def max(self, key: Callable[[T], U] = lambda x: x) -> Optional[T]:
         with suppress(ValueError):  # thrown when stream is empty
             return max(self, key=key)
 
-    def min(self, key: Callable[[Any], Any] = lambda x: x) -> Optional[Any]:
+    def min(self, key: Callable[[T], U] = lambda x: x) -> Optional[T]:
         with suppress(ValueError):  # thrown when stream is empty
             return min(self, key=key)
 
-    def find(self, fn: Callable[[Any], bool]) -> Optional[Any]:
+    def find(self, fn: Callable[[T], bool]) -> Optional[T]:
         return self.filter(fn).first()
 
-    def foreach(self, fn: Callable[[Iterable], None]) -> None:
+    def foreach(self, fn: Callable[[T], None]) -> None:
         for item in self:
             fn(item)
 
-    def group(self, key_fn: Callable[[Any], Any], val_fn: Callable[[Any], Any], grouper: Grouper) -> dict:
+    def group(self, key_fn: Callable[[T], U], val_fn: Callable[[T], V], grouper: Grouper) -> dict:
         d = defaultdict(grouper.collection)
         for item in self:
             key, val = key_fn(item), val_fn(item)
             return_val = grouper.grouper_fn(d[key], val)
             # if there is no return value then it is assumed that the operation is performed inplace
             # eg: appending item to a list
             # but if there is a return value then it is assumed not inplace
             # eg: concatenating strings
             if return_val is not None:
                 d[key] = return_val
         return dict(d)
 
-    def allmatch(self, fn: Callable[[Any], bool]) -> bool:
+    def allmatch(self, fn: Callable[[T], bool]) -> bool:
         return all(fn(item) for item in self)
 
-    def anymatch(self, fn: Callable[[Any], bool]) -> bool:
+    def anymatch(self, fn: Callable[[T], bool]) -> bool:
         return any(fn(item) for item in self)
 
     def count(self) -> int:
         size = 0
         for _ in self:
             size += 1
         return size
```

### Comparing `amnis-0.1.1/amnis.egg-info/PKG-INFO` & `amnis-0.1.2/amnis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amnis
-Version: 0.1.1
+Version: 0.1.2
 Summary: Java like Stream Api for Python
 Home-page: https://github.com/zahash/amnis
 Author: zahash
 Author-email: zahash.z@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `amnis-0.1.1/setup.py` & `amnis-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 README = (HERE / "README.md").read_text()
 
 with (HERE / "requirements.txt").open() as f:
     requirements = f.read().splitlines()
 
 setup(
     name="amnis",
-    version="0.1.1",
+    version="0.1.2",
     description="Java like Stream Api for Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/zahash/amnis",
     author="zahash",
     author_email="zahash.z@gmail.com",
     license="MIT",
```

