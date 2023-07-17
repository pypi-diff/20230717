# Comparing `tmp/scrape_schema-0.3.6.tar.gz` & `tmp/scrape_schema-0.3.7.tar.gz`

## Comparing `scrape_schema-0.3.6.tar` & `scrape_schema-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/_logger.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/_protocols.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/_typing.py
--rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/base.py
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/field.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/nested.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/type_caster.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/special_methods/__init__.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/special_methods/base.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/special_methods/methods.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/LICENSE
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/README.md
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    12494 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/_logger.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/_protocols.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/_typing.py
+-rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/base.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/field.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/nested.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/type_caster.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/special_methods/__init__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/special_methods/base.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/scrape_schema/special_methods/methods.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/LICENSE
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/README.md
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 scrape_schema-0.3.7/PKG-INFO
```

### Comparing `scrape_schema-0.3.6/scrape_schema/_protocols.py` & `scrape_schema-0.3.7/scrape_schema/_protocols.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.6/scrape_schema/_typing.py` & `scrape_schema-0.3.7/scrape_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.6/scrape_schema/base.py` & `scrape_schema-0.3.7/scrape_schema/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,30 +66,36 @@
             return getattr(markup, method.METHOD_NAME)(*method.args, **method.kwargs)
         raise TypeError(  # pragma: no cover
             f"`{type(markup).__name__}` is not contains `{method.METHOD_NAME}`"
         )
 
     def _call_stack_methods(self, markup: Any) -> Any:
         result = markup
-        _logger.info("start call methods. stack count: %s", len(self._stack_methods))
-        for method in self._stack_methods:
+        _logger.info("Start parse markup. Stack methods count: %s", len(self._stack_methods))
+        _logger.debug("Markup target:\nSTART:\n%s\nEND",
+                      markup.css("body").get() if isinstance(markup, (Selector, SelectorList)) else markup)
+        for i, method in enumerate(self._stack_methods, 1):
             try:
                 if isinstance(method.METHOD_NAME, SpecialMethods):
                     result = self._special_method(result, method)
                 else:
                     result = self._accept_method(result, method)
+                _logger.debug("[%s] %s -> %s", i, method, result)
             except Exception as e:
-                return self._stack_method_handler(method, e)
+                _logger.warning("Oops, %s throw exception %s", method, e)
+                return self._stack_method_handler(method, e, markup)
         _logger.info("Call methods done. result=%s", result)
         return result
 
     def _stack_method_handler(
-        self, method: Union[MarkupMethod, SpecialMethods], e: Exception
+            self, method: Union[MarkupMethod, SpecialMethods], e: Exception, markup
     ):
-        _logger.error("Method `%s` return traceback %s", method, e)
+        _logger.warning("Method `%s` return traceback %s", method, e)
+        _logger.warning("Full markup:\nSTART\n%s\nEND",
+                        markup.get() if isinstance(markup, (Selector, SelectorList)) else markup)
         _logger.exception(e)
         if self.default is Ellipsis:
             raise e
         _logger.warning("Set default value %s and disable type_casting", self.default)
         self.is_default = True
         return self.default
 
@@ -112,49 +118,49 @@
         return self.add_method(SpecialMethods.CONCAT_R, right_string)  # type: ignore
 
     def sc_replace(self, old: str, new: str, count: int = -1) -> SpecialMethodsProtocol:
         """replace string method. Last argument should be string"""
         return self.add_method(SpecialMethods.REPLACE, old, new, count)  # type: ignore
 
     def re_search(
-        self,
-        pattern: Union[str, Pattern[str]],
-        flags: Union[int, RegexFlag] = 0,
-        groupdict: bool = False,
+            self,
+            pattern: Union[str, Pattern[str]],
+            flags: Union[int, RegexFlag] = 0,
+            groupdict: bool = False,
     ) -> SpecialMethodsProtocol:
         """re.search method for text result.
 
         Last chain should be return string.
 
         :param pattern: regex pattern
         :param flags: compilation flags
         :param groupdict: accept groupdict method. patter required named groups. default False
         """
         pattern = re.compile(pattern, flags=flags)
         return self.add_method(SpecialMethods.REGEX_SEARCH, pattern, groupdict)  # type: ignore
 
     def re_findall(
-        self,
-        pattern: Union[str, Pattern[str]],
-        flags: Union[int, RegexFlag] = 0,
-        groupdict: bool = False,
+            self,
+            pattern: Union[str, Pattern[str]],
+            flags: Union[int, RegexFlag] = 0,
+            groupdict: bool = False,
     ) -> SpecialMethodsProtocol:
         """[match for match in re.finditer(...)] method for text result.
 
         Last chain should be return string.
 
         :param pattern: regex pattern
         :param flags: compilation flags
         :param groupdict: accept groupdict method. patter required named groups. default False
         """
         pattern = re.compile(pattern, flags=flags)
         return self.add_method(SpecialMethods.REGEX_FINDALL, pattern, groupdict)  # type: ignore
 
     def chomp_js_parse(
-        self, unicode_escape: Any = False, json_params: Any = None
+            self, unicode_escape: Any = False, json_params: Any = None
     ) -> SpecialMethodsProtocol:
         """Extracts first JSON object encountered in the input string
 
         Params:
             string – Input string
             unicode_escape – Attempt to fix input string if it contains escaped special characters
             json_params – Allow passing down standard json.loads options
@@ -163,18 +169,18 @@
             Extracted JSON object
         """
         return self.add_method(  # type: ignore
             SpecialMethods.CHOMP_JS_PARSE, unicode_escape, json_params
         )
 
     def chomp_js_parse_all(
-        self,
-        unicode_escape: Any = False,
-        omitempty: Any = False,
-        json_params: Any = None,
+            self,
+            unicode_escape: Any = False,
+            omitempty: Any = False,
+            json_params: Any = None,
     ) -> SpecialMethodsProtocol:
         """Returns a list extracting all JSON objects encountered in the input string. Can be used to read JSON Lines
 
         Params:
             string – Input string
             unicode_escape – Attempt to fix input string if it contains escaped special characters
             omitempty – Skip empty dictionaries and lists
@@ -184,15 +190,15 @@
             Iterating over it yields all encountered JSON objects
         """
         return self.add_method(  # type: ignore
             SpecialMethods.CHOMP_JS_PARSE_ALL, unicode_escape, omitempty, json_params
         )
 
     def add_method(
-        self, method_name: Union[str, SpecialMethods], *args, **kwargs
+            self, method_name: Union[str, SpecialMethods], *args, **kwargs
     ) -> Self:
         """low-level interface adding methods to call stack"""
         self._stack_methods.append(MarkupMethod(method_name, args=args, kwargs=kwargs))
         return self
 
     def __getitem__(self, item) -> Self:
         return self.add_method("__getitem__", item)
@@ -220,15 +226,15 @@
 
         cls_schema = super().__new__(mcs, name, bases, attrs)
         if cls_schema.__name__ == "BaseSchema":
             return cls_schema
 
         # localns={} kwarg avoid TypeError 'function' object is not subscriptable
         for name, value in get_type_hints(
-            cls_schema, localns={}, include_extras=True
+                cls_schema, localns={}, include_extras=True
         ).items():
             if name in ("__schema_fields__", "__schema_annotations__", "__parsers__"):
                 continue  # pragma: no cover
             if mcs.__is_type_field(value):  # pragma: no cover
                 field_type, field = mcs.__parse_annotated_field(value)
                 __schema_fields__[name] = field
                 __schema_annotations__[name] = field_type
```

### Comparing `scrape_schema-0.3.6/scrape_schema/field.py` & `scrape_schema-0.3.7/scrape_schema/field.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.6/scrape_schema/nested.py` & `scrape_schema-0.3.7/scrape_schema/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.6/scrape_schema/type_caster.py` & `scrape_schema-0.3.7/scrape_schema/type_caster.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.6/scrape_schema/special_methods/__init__.py` & `scrape_schema-0.3.7/scrape_schema/special_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.6/scrape_schema/special_methods/base.py` & `scrape_schema-0.3.7/scrape_schema/special_methods/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class MarkupMethod(NamedTuple):
     METHOD_NAME: Union[str, SpecialMethods]
     args: Tuple[Any, ...] = ()
     kwargs: Dict[str, Any] = {}
 
     def __repr__(self):
-        return f"{self.METHOD_NAME} args={self.args}, kwargs={self.kwargs}"  # pragma: no cover
+        return f"Method={self.METHOD_NAME}, args={self.args}, kwargs={self.kwargs}"  # pragma: no cover
 
 
 class SpecialMethodCallable(Protocol):
     def __call__(self, markup: Any, method: MarkupMethod, **kwargs):
         pass  # pragma: no cover
```

### Comparing `scrape_schema-0.3.6/scrape_schema/special_methods/methods.py` & `scrape_schema-0.3.7/scrape_schema/special_methods/methods.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.6/.gitignore` & `scrape_schema-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.6/LICENSE` & `scrape_schema-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.6/README.md` & `scrape_schema-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.6/pyproject.toml` & `scrape_schema-0.3.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 Documentation = "https://github.com/vypivshiy/scrape-schema#readme"
 Issues = "https://github.com/vypivshiy/scrape-schema/issues"
 Source = "https://github.com/vypivshiy/scrape-schema"
 Examples = "https://github.com/vypivshiy/scrape-schema/examples"
 
 
 [project.optional-dependencies]
-dev = ["flake8", "black", "isort", "pytest", "mypy", "parsel"]
-ci = ["hatch", "bs4", "selectolax", "flake8", "black", "isort", "pytest", "mypy", "parsel"]
+dev = ["flake8", "black", "isort", "pytest", "mypy"]
+ci = ["hatch", "flake8", "black", "isort", "pytest", "mypy", "parsel"]
 docs = ["mkdocs-material"]
 
 [tool.hatch.version]
 path = "scrape_schema/__init__.py"
 
 [tool.hatch.envs.docs]
 dependencies = [
@@ -53,18 +53,18 @@
 
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --clean --strict"
 serve = "mkdocs serve --dev-addr localhost:8000"
 
 [tool.hatch.envs.default]
 dependencies = [
-  "colorama",
+  "colorlog",
+  "chompjs",
+  "typing_extensions",
   "pytest",
-  "selectolax",
-  "bs4",
   "parsel",
   "pytest-cov"
 ]
 
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=scrape_schema --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
@@ -103,16 +103,7 @@
 
 [tool.mypy]
 python_version = 3.8
 pretty = true
 ignore_missing_imports = true
 exclude = ["env", ".env", "venv", "tests/*", "__pycache__", "examples"]
 files = "scrape_schema/*.py,scrape_schema/fields/*.py,scrape_schema/callbacks/*.py"
-
-[tool.pytest.ini_options]
-filterwarnings = [
-    "error",
-    'ignore::RuntimeWarning',
-    'ignore::DeprecationWarning'
-]
-
-
```

### Comparing `scrape_schema-0.3.6/PKG-INFO` & `scrape_schema-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.3.6
+Version: 0.3.7
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
@@ -23,28 +23,25 @@
 Requires-Python: >=3.8
 Requires-Dist: chompjs
 Requires-Dist: colorlog
 Requires-Dist: parsel
 Requires-Dist: typing-extensions; python_version < '3.11'
 Provides-Extra: ci
 Requires-Dist: black; extra == 'ci'
-Requires-Dist: bs4; extra == 'ci'
 Requires-Dist: flake8; extra == 'ci'
 Requires-Dist: hatch; extra == 'ci'
 Requires-Dist: isort; extra == 'ci'
 Requires-Dist: mypy; extra == 'ci'
 Requires-Dist: parsel; extra == 'ci'
 Requires-Dist: pytest; extra == 'ci'
-Requires-Dist: selectolax; extra == 'ci'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: parsel; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == 'docs'
 Description-Content-Type: text/markdown
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Documentation Status](https://readthedocs.org/projects/scrape-schema/badge/?version=latest)](https://scrape-schema.readthedocs.io/en/latest/?badge=latest)
```

