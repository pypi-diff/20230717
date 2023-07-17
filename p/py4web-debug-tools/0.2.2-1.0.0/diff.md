# Comparing `tmp/py4web-debug-tools-0.2.2.tar.gz` & `tmp/py4web_debug_tools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-debug-tools-0.2.2.tar", last modified: Fri Jul 14 13:59:15 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `py4web-debug-tools-0.2.2.tar` & `py4web_debug_tools-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,17 @@
-drwxrwxr-x   0 eddie     (1001) eddie     (1001)        0 2023-07-14 13:59:15.885692 py4web-debug-tools-0.2.2/
--rw-rw-r--   0 eddie     (1001) eddie     (1001)     3687 2023-07-14 13:59:15.881692 py4web-debug-tools-0.2.2/PKG-INFO
--rw-rw-r--   0 eddie     (1001) eddie     (1001)     3393 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/README.md
-drwxrwxr-x   0 eddie     (1001) eddie     (1001)        0 2023-07-14 13:59:15.881692 py4web-debug-tools-0.2.2/py4web_debug/
--rw-rw-r--   0 eddie     (1001) eddie     (1001)      157 2023-07-14 13:53:47.000000 py4web-debug-tools-0.2.2/py4web_debug/__init__.py
--rw-rw-r--   0 eddie     (1001) eddie     (1001)     3073 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/core.py
--rw-rw-r--   0 eddie     (1001) eddie     (1001)     7232 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/debugbar.py
--rw-rw-r--   0 eddie     (1001) eddie     (1001)     3496 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/dumping.py
--rw-rw-r--   0 eddie     (1001) eddie     (1001)       82 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/env.py
--rw-rw-r--   0 eddie     (1001) eddie     (1001)     4316 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/internals.py
-drwxrwxr-x   0 eddie     (1001) eddie     (1001)        0 2023-07-14 13:59:15.881692 py4web-debug-tools-0.2.2/py4web_debug/templates/
--rw-rw-r--   0 eddie     (1001) eddie     (1001)     7169 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/templates/debugbar.html
--rw-rw-r--   0 eddie     (1001) eddie     (1001)       60 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/templates/dumpdie.html
--rw-rw-r--   0 eddie     (1001) eddie     (1001)      868 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/templates/error_default.html
--rw-rw-r--   0 eddie     (1001) eddie     (1001)      532 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/templates/fancy_dumpdie.html
--rw-rw-r--   0 eddie     (1001) eddie     (1001)      207 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/wsgi.py
-drwxrwxr-x   0 eddie     (1001) eddie     (1001)        0 2023-07-14 13:59:15.881692 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/
--rw-rw-r--   0 eddie     (1001) eddie     (1001)     3687 2023-07-14 13:59:15.000000 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/PKG-INFO
--rw-rw-r--   0 eddie     (1001) eddie     (1001)      546 2023-07-14 13:59:15.000000 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 eddie     (1001) eddie     (1001)        1 2023-07-14 13:59:15.000000 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 eddie     (1001) eddie     (1001)       36 2023-07-14 13:59:15.000000 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/requires.txt
--rw-rw-r--   0 eddie     (1001) eddie     (1001)       13 2023-07-14 13:59:15.000000 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/top_level.txt
--rw-rw-r--   0 eddie     (1001) eddie     (1001)       38 2023-07-14 13:59:15.885692 py4web-debug-tools-0.2.2/setup.cfg
--rw-rw-r--   0 eddie     (1001) eddie     (1001)      671 2023-07-14 13:54:29.000000 py4web-debug-tools-0.2.2/setup.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/__about__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/__init__.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/core.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/debugbar.py
+-rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/dumping.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/env.py
+-rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/internals.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/wsgi.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/templates/debugbar.html
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/templates/dumpdie.html
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/templates/error_default.html
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/templates/fancy_dumpdie.html
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/.gitignore
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/README.md
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/PKG-INFO
```

### Comparing `py4web-debug-tools-0.2.2/PKG-INFO` & `py4web_debug_tools-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: py4web-debug-tools
-Version: 0.2.2
-Summary: Debug Tools for py4web
-Home-page: https://github.com/trialandsuccess/py4web-debug-tools
-Author: Robin van der Noord
-Author-email: contact@trialandsuccess.nl
-Requires-Python: >3.10.0
-Description-Content-Type: text/markdown
-
 # py4web debug tools
 
 Tooling to improve the developer experience when working with py4web.
 
 There are two main tools and some helpers that this package provides.
 
 1. A better error 500 screen, that shows the error + traceback of what happened
```

### Comparing `py4web-debug-tools-0.2.2/README.md` & `py4web_debug_tools-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: py4web-debug-tools
+Version: 1.0.0
+Summary: Debug Tools for py4web
+Project-URL: Documentation, https://github.com/trialandsuccess/py4web-debug-tools#readme
+Project-URL: Issues, https://github.com/trialandsuccess/py4web-debug-tools/issues
+Project-URL: Source, https://github.com/trialandsuccess/py4web-debug-tools
+Author-email: Robin van der Noord <contact@trialandsuccess.nl>
+License-Expression: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.10
+Requires-Dist: configurable-json
+Requires-Dist: py4web
+Requires-Dist: pydal
+Requires-Dist: yatl
+Provides-Extra: dev
+Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: su6[all]; extra == 'dev'
+Description-Content-Type: text/markdown
+
 # py4web debug tools
 
 Tooling to improve the developer experience when working with py4web.
 
 There are two main tools and some helpers that this package provides.
 
 1. A better error 500 screen, that shows the error + traceback of what happened
```

### Comparing `py4web-debug-tools-0.2.2/py4web_debug/core.py` & `py4web_debug_tools-1.0.0/py4web_debug/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Transforms janky 'internals' into easy to work with tool
 import os
 import typing
 from dataclasses import dataclass
 
 from py4web import DAL as P4WDAL
 
-from .debugbar import DummyDebugBar, DebugBar
+from .debugbar import DebugBar, DummyDebugBar
 from .env import is_debug
 from .internals import patch_py4
 
 # in: context, out: string
 RendererMethod = typing.Callable[[typing.Dict[str, typing.Any]], str]
```

### Comparing `py4web-debug-tools-0.2.2/py4web_debug/debugbar.py` & `py4web_debug_tools-1.0.0/py4web_debug/debugbar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import typing
 import warnings
 from collections import Counter
 
 import yatl
 from py4web import request
-from py4web.core import Template, Fixture
+from py4web.core import Fixture, Template
 from yatl import XML
 
-from .env import is_debug
 from .dumping import dump
+from .env import is_debug
 
 
 def _fmt_callframe(cf):
     # 0: frame
     # 1: file
     # 2: lineno
     # 3: function
@@ -87,33 +87,29 @@
     3. context['output'] from before it is rendered by the template
     """
 
     debug_data, _, input_data = contexts
     return _debugbar(debug_data, fancy=fancy) + "</html>"
 
 
-def debugbar_template(fixture: Fixture, debug_data: dict, fancy=True):
+def debugbar_template(_: Fixture, debug_data: dict, fancy=True):
     """
     debug_data is reset and filled every request
     """
 
     if not hasattr(Template, "_on_success"):
         # DON'T overwrite existing _on_success because that will lead to recursion...
         Template._on_success = Template.on_success
 
     def _on_request(self, context: dict):
         if not (context and context.get("output")):
             # do nothing
             return
 
-        if isinstance(context.get("output"), dict):
-            pre_render_output = context["output"].copy()
-        else:
-            # no data?
-            pre_render_output = {}
+        pre_render_output = context["output"].copy() if isinstance(context.get("output"), dict) else {}
 
         Template._on_success(self, context)
 
         # only replace actual templates (= end in /html)
         if (output := context["output"]) and isinstance(output, str):
             context["output"] = output.replace(
                 "</html>",
@@ -167,16 +163,16 @@
 
 
 class DummyDebugBar(Fixture):
     ...
 
 
 class DebugBar(Fixture):
-    queries = []  # mutable but DONT OVERWRITE !!!
-    debug_data = {}  # mutable but DON'T OVERWRITE!!
+    queries: typing.ClassVar[list[str]] = []  # mutable but DONT OVERWRITE !!!
+    debug_data: typing.ClassVar[dict[str, typing.Any]] = {}  # mutable but DON'T OVERWRITE!!
 
     def __init__(
         self,
         db,
         fancy_rendering: bool,
         bar_style: typing.Literal["bootstrap"],
         slow_threshold_ms: int,
@@ -195,21 +191,17 @@
 
         return {query: count for query, count in counts.items() if count > 1}
 
     def _find_slow_queries(self, timings: list[tuple[str, float]], threshold_ms: int):
         """
         Returns: a list of queries that took longer than threshold_ms
         """
-        return [
-            {q: f"{round(t * 1000, 5)}ms"}
-            for q, t in timings
-            if t > threshold_ms / 1000
-        ]
+        return [{q: f"{round(t * 1000, 5)}ms"} for q, t in timings if t > threshold_ms / 1000]
 
-    def on_request(self, context):
+    def on_request(self, _: dict[str, typing.Any]):
         db = self.db
         # these two are scoped to the request
         self.queries.clear()  # DON'T OVERWRITE WITH = [] !!!
         self.debug_data.clear()  # idem
         db._timings.clear()
 
         self.debug_data["queries"] = db._timings
@@ -217,39 +209,32 @@
 
         # empty before debug_pydal adds new queries
         # patch the Template.on_success:
         debugbar_template(self, self.debug_data, fancy=self.fancy)
 
     def filter_context(self, input_data: dict):
         """
-        Returns: a dict with all keys that are not in __ignored and it's values shortened (nested long values are pruned)
+        Returns: a dict with all keys that are not in __ignored \
+         and it's values shortened (nested long values are pruned).
         """
         if not input_data or not isinstance(input_data, dict):
             return {}
 
         __ignored = input_data.get("__ignore", [])
 
         # remove common helper methods etc.
-        return {
-            k: convert_for_debugbar(v)
-            for k, v in input_data.items()
-            if k not in __ignored
-        }
+        return {k: convert_for_debugbar(v) for k, v in input_data.items() if k not in __ignored}
 
     def on_success(self, context):
-        self.debug_data["duplicate_queries"] = self._find_duplicate_queries(
-            self.debug_data["queries"]
-        )
+        self.debug_data["duplicate_queries"] = self._find_duplicate_queries(self.debug_data["queries"])
         self.debug_data["slow_queries"] = self._find_slow_queries(
             self.debug_data["queries"], threshold_ms=self.threshold_ms
         )
 
         try:
-            json_context = dump(
-                self.filter_context(context["output"]), with_headers=False
-            )
-        except:
+            json_context = dump(self.filter_context(context["output"]), with_headers=False)
+        except Exception:
             json_context = "(Something went wrong)"
 
         self.debug_data["json_context"] = XML(json_context)
 
         self.debug_data["catch"] = getattr(request, "_catch", [])
```

### Comparing `py4web-debug-tools-0.2.2/py4web_debug/dumping.py` & `py4web_debug_tools-1.0.0/py4web_debug/dumping.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from py4web import response
 
 from .env import is_debug
 
 
 class DDJsonEncoder(ConfigurableJsonEncoder):
     @staticmethod
-    def _default(o):
+    def _default(o) -> str:
         if hasattr(o, "as_list"):
             # note: prefer as_list now as not every Rows may have an id (= default key of as_dict)
             return o.as_list()
         # more as list stuff?
 
         if hasattr(o, "as_dict"):
             return o.as_dict()
@@ -35,45 +35,39 @@
             return o._to_dict()
         elif hasattr(o, "__json__"):
             return o.__json__()
 
         return str(o)
 
     @staticmethod
-    def is_probably_namedtuple(o):
+    def is_probably_namedtuple(o: typing.Any) -> bool:
+        """
+        Try to guess if 'o' is a Named Tuple or something else.
+        """
         return isinstance(o, tuple) and hasattr(o, "_fields")
 
     def rules(self, o, with_default=True) -> JSONRule:
         """
         Custom rules for the DD json: set to list and namedtuple to dict
         # NOTE: with_default is (probably) false anyway!!!!
         """
 
-        if self.is_probably_namedtuple(o):
-            _type = typing.NamedTuple
-        else:
-            _type = type(o)
+        _type = typing.NamedTuple if self.is_probably_namedtuple(o) else type(o)
 
-        # other rules:
-        rule = {
+        return {
             # convert set to list
             set: JSONRule(preprocess=lambda o: list(o)),
             # convert namedtuple to dict
             typing.NamedTuple: JSONRule(preprocess=self._default),
             pydal.objects.Row: JSONRule(preprocess=lambda row: row.as_dict()),
             pydal.objects.Rows: JSONRule(preprocess=lambda row: row.as_list()),
         }.get(_type, JSONRule(transform=self._default) if with_default else None)
 
-        # debug: catch but ignore callframes:
-        # catch(o, _type, rule, levels=0)
-
-        return rule
-
 
-def dump(data: typing.Iterable, with_headers=True):
+def dump(data: typing.Iterable, with_headers=True) -> str:
     """
     Helper to json dump some data with custom converter and headers
     """
     if with_headers:
         response.headers["Content-Type"] = "application/json"
 
     return json.dumps(data, indent=2, cls=DDJsonEncoder)
```

### Comparing `py4web-debug-tools-0.2.2/py4web_debug/internals.py` & `py4web_debug_tools-1.0.0/py4web_debug/internals.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 import logging
 import os
 import re
 import traceback
 import typing
 
 import ombott as bottle
-import py4web.core
 import yatl
-from py4web import action, response, HTTP
+from py4web import HTTP, action, response
 from py4web.core import (
+    REGEX_APPJSON,
+    Template,
     dumps,
-    request,
     error_logger,
     get_error_snapshot,
-    REGEX_APPJSON,
-    Template,
+    request,
 )
 from yatl import XML
 
 
 def custom_error_page(
     code,
     button_text=None,
@@ -41,19 +40,15 @@
 
     if hasattr(Template, "_on_success"):
         # reset here on error, because on_error might not be called!
         Template.on_success = Template._on_success
         del Template._on_success
 
     message = http.client.responses[code].upper() if message is None else message
-    color = (
-        {"4": "#F44336", "5": "#607D8B"}.get(str(code)[0], "#2196F3")
-        if not color
-        else color
-    )
+    color = color or {"4": "#F44336", "5": "#607D8B"}.get(str(code)[0], "#2196F3")
     context = dict(
         code=code,
         message=message,
         button_text=button_text,
         href=href,
         color=color,
         traceback=traceback,
```

### Comparing `py4web-debug-tools-0.2.2/py4web_debug/templates/debugbar.html` & `py4web_debug_tools-1.0.0/py4web_debug/templates/debugbar.html`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.2/py4web_debug/templates/error_default.html` & `py4web_debug_tools-1.0.0/py4web_debug/templates/error_default.html`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.2/py4web_debug/templates/fancy_dumpdie.html` & `py4web_debug_tools-1.0.0/py4web_debug/templates/fancy_dumpdie.html`

 * *Files identical despite different names*

