# Comparing `tmp/magic-filter-1.0.8.tar.gz` & `tmp/magic-filter-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic-filter-1.0.8.tar", max compression
+gzip compressed data, was "magic-filter-1.0.9.tar", max compression
```

## Comparing `magic-filter-1.0.8.tar` & `magic-filter-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       85 2022-07-03 14:08:02.917658 magic-filter-1.0.8/README.md
--rw-r--r--   0        0        0      310 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/__init__.py
--rw-r--r--   0        0        0      368 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/attrdict.py
--rw-r--r--   0        0        0      306 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/exceptions.py
--rw-r--r--   0        0        0      291 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/helper.py
--rw-r--r--   0        0        0    10059 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/magic.py
--rw-r--r--   0        0        0      632 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/operations/__init__.py
--rw-r--r--   0        0        0      231 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/operations/base.py
--rw-r--r--   0        0        0      527 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/operations/call.py
--rw-r--r--   0        0        0      446 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/operations/cast.py
--rw-r--r--   0        0        0     1005 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/operations/combination.py
--rw-r--r--   0        0        0      522 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/operations/comparator.py
--rw-r--r--   0        0        0      751 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/operations/function.py
--rw-r--r--   0        0        0      466 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/operations/getattr.py
--rw-r--r--   0        0        0      736 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/operations/getitem.py
--rw-r--r--   0        0        0      504 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/operations/selector.py
--rw-r--r--   0        0        0        0 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/py.typed
--rw-r--r--   0        0        0      437 2022-07-03 14:08:02.917658 magic-filter-1.0.8/magic_filter/util.py
--rw-r--r--   0        0        0     1396 2022-07-03 14:08:02.917658 magic-filter-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      728 2022-07-03 14:08:14.273760 magic-filter-1.0.8/setup.py
--rw-r--r--   0        0        0      967 2022-07-03 14:08:14.274017 magic-filter-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0       85 2022-09-11 14:28:10.204648 magic-filter-1.0.9/README.md
+-rw-r--r--   0        0        0      310 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/__init__.py
+-rw-r--r--   0        0        0      368 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/attrdict.py
+-rw-r--r--   0        0        0      306 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/exceptions.py
+-rw-r--r--   0        0        0      291 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/helper.py
+-rw-r--r--   0        0        0    10260 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/magic.py
+-rw-r--r--   0        0        0      632 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/operations/__init__.py
+-rw-r--r--   0        0        0      231 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/operations/base.py
+-rw-r--r--   0        0        0      527 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/operations/call.py
+-rw-r--r--   0        0        0      446 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/operations/cast.py
+-rw-r--r--   0        0        0     1005 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/operations/combination.py
+-rw-r--r--   0        0        0      522 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/operations/comparator.py
+-rw-r--r--   0        0        0      751 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/operations/function.py
+-rw-r--r--   0        0        0      466 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/operations/getattr.py
+-rw-r--r--   0        0        0      736 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/operations/getitem.py
+-rw-r--r--   0        0        0      504 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/operations/selector.py
+-rw-r--r--   0        0        0        0 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/py.typed
+-rw-r--r--   0        0        0      437 2022-09-11 14:28:10.204648 magic-filter-1.0.9/magic_filter/util.py
+-rw-r--r--   0        0        0     1318 2022-09-11 14:28:10.204648 magic-filter-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 magic-filter-1.0.9/setup.py
+-rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 magic-filter-1.0.9/PKG-INFO
```

### Comparing `magic-filter-1.0.8/magic_filter/magic.py` & `magic-filter-1.0.9/magic_filter/magic.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
 class MagicFilter:
     __slots__ = ("_operations",)
 
     def __init__(self, operations: Tuple[BaseOperation, ...] = ()) -> None:
         self._operations = operations
 
+    # An instance of MagicFilter cannot be used as an iterable object because objects
+    # with a __getitem__ method can be endlessly iterated, which is not the desired behavior.
+    __iter__ = None
+
     @classmethod
     def ilter(cls, magic: "MagicFilter") -> Callable[[Any], Any]:
         @wraps(magic.resolve)
         def wrapper(value: Any) -> Any:
             return magic.resolve(value)
 
         return wrapper
```

### Comparing `magic-filter-1.0.8/magic_filter/operations/__init__.py` & `magic-filter-1.0.9/magic_filter/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `magic-filter-1.0.8/magic_filter/operations/call.py` & `magic-filter-1.0.9/magic_filter/operations/call.py`

 * *Files identical despite different names*

### Comparing `magic-filter-1.0.8/magic_filter/operations/combination.py` & `magic-filter-1.0.9/magic_filter/operations/combination.py`

 * *Files identical despite different names*

### Comparing `magic-filter-1.0.8/magic_filter/operations/comparator.py` & `magic-filter-1.0.9/magic_filter/operations/comparator.py`

 * *Files identical despite different names*

### Comparing `magic-filter-1.0.8/magic_filter/operations/function.py` & `magic-filter-1.0.9/magic_filter/operations/function.py`

 * *Files identical despite different names*

### Comparing `magic-filter-1.0.8/magic_filter/operations/getitem.py` & `magic-filter-1.0.9/magic_filter/operations/getitem.py`

 * *Files identical despite different names*

### Comparing `magic-filter-1.0.8/pyproject.toml` & `magic-filter-1.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 [tool.poetry]
 name = "magic-filter"
-version = "1.0.8"
+version = "1.0.9"
 description = "This package provides magic filter based on dynamic attribute getter"
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aiogram/magic-filter/"
 authors = ["Alex Root Junior <pypi@aiogram.dev>"]
 classifiers = [
 	"Development Status :: 3 - Alpha",
 	"License :: OSI Approved :: MIT License",
-	"Programming Language :: Python :: 3.6",
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Topic :: Utilities",
 	"Typing :: Typed",
 ]
 keywords = [
 	"magic",
 	"filter",
 	"validation"
 ]
-include = [
-	"magic_filter/py.typed"
-]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.7"
 
-[tool.poetry.dev-dependencies]
-pre-commit = "^2.17.0"
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^2.20.0"
+pytest = "^7.1.3"
 pytest-cov = "^3.0.0"
 pytest-html = "^3.1.1"
-pytest = "^7.0.1"
-mypy = "^0.961"
-black = "^22.6.0"
-flake8 = "^4.0.1"
+flake8 = "^5.0.4"
+mypy = "^0.971"
+black = "^22.8.0"
 isort = "^5.10.1"
-types-setuptools = "^57.4.18"
+types-setuptools = "^65.3.0"
 
 [tool.black]
 line-length = 99
 target-version = ['py37', 'py38', 'py39', 'py310']
 exclude = '''
 (
     \.eggs
```

### Comparing `magic-filter-1.0.8/PKG-INFO` & `magic-filter-1.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: magic-filter
-Version: 1.0.8
+Version: 1.0.9
 Summary: This package provides magic filter based on dynamic attribute getter
 Home-page: https://github.com/aiogram/magic-filter/
 License: MIT
 Keywords: magic,filter,validation
 Author: Alex Root Junior
 Author-email: pypi@aiogram.dev
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/aiogram/magic-filter/
 Description-Content-Type: text/markdown
```

