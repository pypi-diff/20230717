# Comparing `tmp/shil-2023.7.15.12.33.tar.gz` & `tmp/shil-2023.7.17.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shil-2023.7.15.12.33.tar", last modified: Sat Jul 15 12:33:45 2023, max compression
+gzip compressed data, was "shil-2023.7.17.7.1.tar", last modified: Mon Jul 17 07:01:18 2023, max compression
```

## Comparing `shil-2023.7.15.12.33.tar` & `shil-2023.7.17.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.884633 shil-2023.7.15.12.33/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/src/shil/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-15 12:32:51.000000 shil-2023.7.15.12.33/src/shil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-15 12:33:41.000000 shil-2023.7.15.12.33/src/shil/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/bin.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/src/shil/format/
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/format/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/format/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/src/shil/models/
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-15 12:32:51.000000 shil-2023.7.15.12.33/src/shil/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/src/shil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:01:18.788962 shil-2023.7.17.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-17 07:01:18.788962 shil-2023.7.17.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-17 07:01:18.788962 shil-2023.7.17.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:01:18.776962 shil-2023.7.17.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:01:18.788962 shil-2023.7.17.7.1/src/shil/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/src/shil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/src/shil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 07:01:14.000000 shil-2023.7.17.7.1/src/shil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/src/shil/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/src/shil/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:01:18.788962 shil-2023.7.17.7.1/src/shil/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-07-17 07:00:22.000000 shil-2023.7.17.7.1/src/shil/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/src/shil/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:01:18.788962 shil-2023.7.17.7.1/src/shil/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/src/shil/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/src/shil/parser/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/src/shil/parser/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-17 06:59:41.000000 shil-2023.7.17.7.1/src/shil/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:01:18.788962 shil-2023.7.17.7.1/src/shil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-17 07:01:18.000000 shil-2023.7.17.7.1/src/shil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-17 07:01:18.000000 shil-2023.7.17.7.1/src/shil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:01:18.000000 shil-2023.7.17.7.1/src/shil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:01:18.000000 shil-2023.7.17.7.1/src/shil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-17 07:01:18.000000 shil-2023.7.17.7.1/src/shil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 07:01:18.000000 shil-2023.7.17.7.1/src/shil.egg-info/top_level.txt
```

### Comparing `shil-2023.7.15.12.33/PKG-INFO` & `shil-2023.7.17.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shil
-Version: 2023.7.15.12.33
+Version: 2023.7.17.7.1
 Summary: Shell helper utilities for python
 Home-page: https://github.com/elo-enterprises/shil/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/shil/
 Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shil Version: 2023.7.15.12.33 Summary: Shell helper
+Metadata-Version: 2.1 Name: shil Version: 2023.7.17.7.1 Summary: Shell helper
 utilities for python Home-page: https://github.com/elo-enterprises/shil/
 Author: elo License: MIT Project-URL: Documentation, https://github.com/elo-
 enterprises/shil/ Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files Platform:
 any Classifier: Programming Language :: Python Requires-Python: >3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Provides-
 Extra: dev Provides-Extra: testing Provides-Extra: lint Provides-Extra: publish
```

### Comparing `shil-2023.7.15.12.33/README.md` & `shil-2023.7.17.7.1/README.md`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.12.33/setup.cfg` & `shil-2023.7.17.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.12.33/setup.py` & `shil-2023.7.17.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.12.33/src/shil/__main__.py` & `shil-2023.7.17.7.1/src/shil/__main__.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.12.33/src/shil/format/__init__.py` & `shil-2023.7.17.7.1/src/shil/parser/semantics.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,55 @@
-""" shil.format
+""" shil.parser.semantics
 """
-import json as modjson
+import json
 from pathlib import Path
 
-import tatsu
 from fleks.util import lme
 
-from .grammar import bashParser
-
-DEBUG = True  # False
 LOGGER = lme.get_logger(__name__)
 
 
 class Semantics:
-    """ """
-
     def strict_word(self, ast):
-        LOGGER.warning(f"strict_word: {ast}")
+        LOGGER.info(f"strict_word: {ast}")
         return ast
 
     def dquote(self, ast):
-        LOGGER.warning(f"dquote: {ast}")
+        LOGGER.info(f"dquote: {ast}")
         if len(ast) > 10:
             ast = ast.lstrip()
             return f'"\\n{ast}\\n"'
         return ast
 
     def squote(self, ast):
-        LOGGER.warning(f"squote: {ast}")
+        from json import loads
+
+        LOGGER.info(f"squote: {ast}")
         ast = ast.strip().lstrip()
         is_json = ast.startswith("{") and ast.strip().endswith("}")
         if is_json:
             try:
-                tmp = modjson.loads(ast)
+                # tmp = loads.json5(ast)
+                tmp = loads(ast)
             except:
                 is_json = False
             else:
                 LOGGER.critical(f"found json: {tmp}")
-                ast = modjson.dumps(tmp, indent=2)
+                ast = json.dumps(tmp, indent=2)
             out = [x + " \\" for x in ast.split("\n")]
             out = "\n".join(out)
             return f"'{out}'"
         return ast
 
-    # def group_command(self, ast):
-    #     LOGGER.warning(f"group_command: {ast}")
-    #     return ast
-
     def word(self, ast):
-        LOGGER.warning(f"word: {ast}")
+        LOGGER.info(f"word: {ast}")
         return ast
 
     def simple_command(self, ast):
-        LOGGER.warning(f"simple_command: {ast}")
+        LOGGER.info(f"simple_command: {ast}")
         tail = ast
         biggest = ""
         for i, l in enumerate(tail):
             if len(l) > len(biggest):
                 biggest = l
         result = []
         skip_next = False
@@ -64,15 +57,15 @@
             if skip_next:
                 skip_next = False
                 continue
             try:
                 n = tail[i + 1]
             except:
                 n = ""
-                # LOGGER.warning(f'looking at {[i,l,n]}')
+                # LOGGER.info(f'looking at {[i,l,n]}')
             comb = f"{l} {n}"
             if len(comb) < len(biggest):
                 result.append(comb)
                 skip_next = True
             else:
                 result.append(l)
         # import IPython; IPython.embed()
@@ -82,76 +75,50 @@
             if isinstance(item, (tuple,)):
                 item = " ".join(item)
             newp.append(item)
         result = newp
         return "\n  ".join(map(str, result))
 
     def shell_command(self, ast):
-        LOGGER.warning(f"shell_command: {ast}")
+        LOGGER.info(f"shell_command: {ast}")
         return ast
 
     def path(self, ast):
-        LOGGER.warning(f"path: {ast}")
+        LOGGER.info(f"path: {ast}")
         try:
             tmp = Path(ast).relative_to(Path(".").absolute())
         except ValueError:
             return ast
         else:
             return f"'{tmp}'"
 
     def pipeline_command(self, ast):
-        LOGGER.warning(f"pipeline_command: {ast}")
+        LOGGER.info(f"pipeline_command: {ast}")
         return ast
 
     def simple_list(self, ast):
-        LOGGER.warning(f"simple_list: {ast}")
+        LOGGER.info(f"simple_list: {ast}")
         return ast
 
     def word_list(self, ast):
-        LOGGER.warning(f"word_list: {ast}")
+        LOGGER.info(f"word_list: {ast}")
         return ast
 
     def opt(self, ast):
-        LOGGER.warning(f"opt: {ast}")
+        LOGGER.info(f"opt: {ast}")
         return ast if isinstance(ast, (str,)) else " ".join(ast)
 
     def opt_val(self, ast):
-        LOGGER.warning(f"opt_val: {ast}")
+        LOGGER.info(f"opt_val: {ast}")
         return ast
 
     def subcommands(self, ast):
-        LOGGER.warning(f"subcommands: {ast}")
+        LOGGER.info(f"subcommands: {ast}")
         return " ".join(ast)
 
     def drilldown(self, ast):
-        LOGGER.warning(f"drilldown: {ast}")
+        LOGGER.info(f"drilldown: {ast}")
         return ast
 
     def entry(self, ast):
-        LOGGER.warning(f"entry: {ast}")
+        LOGGER.info(f"entry: {ast}")
         return str(ast)
-
-
-def shfmt(text, filename="?"):
-    """ """
-    semantics = Semantics()
-    parser = bashParser()
-    try:
-        parsed = parser.parse(
-            text,
-            parseinfo=True,
-            filename=filename,
-            semantics=semantics,
-        )
-    except (tatsu.exceptions.FailedParse,) as exc:
-        LOGGER.critical(exc)
-        return text
-    else:
-        out = []
-        for item in parsed:
-            if isinstance(item, (list, tuple)):
-                item = " ".join([str(x) for x in item])
-            out.append(item)
-        head = out.pop(0)
-        # tail=out.copy()
-        tail = "\n  ".join(out)
-        return f"{head} {tail}"
```

### Comparing `shil-2023.7.15.12.33/src/shil/format/grammar.py` & `shil-2023.7.17.7.1/src/shil/parser/grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" shil.format.grammar
+""" shil.grammar
 """
 GRAMMAR = r"""@@grammar::bash
 @@comments :: /\(\*.*?\*\)/
 @@eol_comments :: /#.*?$/
 @@whitespace :: /[\t \n \\]/
 @@keyword :: do done for in
 #
```

### Comparing `shil-2023.7.15.12.33/src/shil/models/__init__.py` & `shil-2023.7.17.7.1/src/shil/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,87 +1,126 @@
 """ shil.models
 """
 import os
+import json
 import typing
 import subprocess
 
 import pydantic
 from fleks.util import lme
 
-from shil.format import shfmt
-from shil.console import Panel, Syntax, Text
+from shil import console
+from shil.parser import shfmt
 
 LOGGER = lme.get_logger(__name__)
 
 Field = pydantic.Field
 
-
-class BaseModel(pydantic.BaseModel):
-    """ """
-
-    def update(self, **kwargs):
-        return self.__dict__.update(**kwargs)
-
-    class Config:
-        arbitrary_types_allowed = True
-        # frozen = True
+from .base import BaseModel
 
 
 class Invocation(BaseModel):
-    command: typing.Optional[str] = Field()
-    stdin: typing.Optional[str] = Field(help="stdin to send to command")
-    strict: bool = Field(default=False, help="Fail if command fails")
-    shell: typing.Optional[bool] = Field(help="Fail if command fails")
-    interactive: bool = Field(default=False, help="Interactive mode")
+    command: typing.Optional[str] = Field(help="")
+    stdin: typing.Optional[str] = Field(default=None, help="stdin to send to command")
+    strict: bool = Field(
+        default=False,
+        help="Fail if command fails",
+    )
+    shell: typing.Optional[bool] = Field(
+        help="Fail if command fails",
+    )
+    interactive: bool = Field(
+        default=False,
+        help="Interactive mode",
+    )
     large_output: bool = Field(
         default=False, help="Flag for indicating that output is huge"
     )
-    log_command: bool = Field(
-        default=True,
-        help="Flag indicating whether command should be logged when it is run",
+    command_logger: typing.Optional[typing.Any] = Field(
+        default=None,
+        help="",
+    )
+    output_logger: typing.Optional[typing.Any] = Field(
+        default=None,
+        help="",
     )
-    environment: dict = Field(default={})
-    log_stdin: bool = Field(default=True)
+    environment: dict = Field(
+        default={},
+        help="",
+    )
+    # log_stdin: bool = Field(default=True)
     system: bool = Field(help='Execute command in "system" mode', default=False)
     load_json: bool = Field(help="Load JSON from output", default=False)
 
-    def __rich_console__(self, console, options):  # noqa
-        """
-        https://rich.readthedocs.io/en/stable/protocol.html
-        """
-        yield f"[dim]$[/dim] [b]{self.command}[/b]"
+    @property
+    def system(self):
+        """ """
+        tmp = self.__dict__.get("system", False)
+        if tmp:
+            if self.stdin or self.interactive:
+                err = f"{self} `system` cannot be used with `stdin`/`interactive`"
+                LOGGER.critical(err)
+                raise ValueError(err)
+                # assert not self.stdin and not self.interactive
 
     def __call__(self):
         """ """
-        #     if self.log_command:
-        #         msg = f"running command: (system={self.system})\n  {self.command}"
-        #         LOGGER.warning(msg)
-        LOGGER.warning(self.command)
+        if self.command_logger:
+            tmp_sys = f"system={self.system}" if self.system else ""
+            tmp_str = f"strict={self.strict}" if self.strict else ""
+            tmp = " ".join([tmp_sys, tmp_str]).strip() or ".."
+            tmp = f"({tmp})"
+            msg = f"Running command: {tmp}\n  {self.command}"
+            self.command_logger(msg)
         result = InvocationResult(**self.dict())
 
         if self.system:
-            assert not self.stdin and not self.interactive
-            error = os.system(self.command)
+            # FIXME: record `pid` and support `environment`
+
+            # proc = subprocess.call(
+            proc = subprocess.run(
+                self.command,
+                shell=True,
+                # capture_output=True,
+            )
+            # result.update(
+            #     stderr=proc.stderr.decode("utf-8"),
+            #     stdout=proc.stdout.decode("utf-8"),
+            # )
+            # error = os.system(self.command)
+            # import sys
+            # proc = subprocess.Popen(
+            #     self.command,
+            #     # stdout=sys.stdout,
+            #     stdout=subprocess.PIPE
+            #     )
+            # stdout=""
+            # for c in iter(lambda: proc.stdout.read(1), b""):
+            #     sys.stdout.buffer.write(c)
+            #     stdout+=c
+            error = proc.returncode > 0
             result.update(
                 failed=bool(error),
                 failure=bool(error),
                 success=not bool(error),
                 succeeded=not bool(error),
-                stdout="<os.system>",
-                stdin="<os.system>",
+                stdout=proc.stdout.decode("utf-8"),
+                # stdout="<os.system>",
+                # stdin="<os.system>",
             )
             return result
 
         exec_kwargs = dict(
             shell=True,
             env={**{k: v for k, v in os.environ.items()}, **self.environment},
         )
         if self.stdin:
-            msg = "command will receive pipe:\n{}"
-            self.log_stdin and LOGGER.debug(msg.format(self.stdin))
+            self.command_logger and self.command_logger(
+                f"Command will receive pipe:\n{self.stdin}"
+            )
             exec_kwargs.update(
                 stdin=subprocess.PIPE,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
             )
             LOGGER.critical([self.command, exec_kwargs])
             tmp = subprocess.run(
@@ -101,96 +140,112 @@
                 failure=result.failed,
                 succeeded=not result.failure,
                 success=not result.failure,
             )
             return result
         else:
             if not self.interactive:
-                exec_kwargs.update(stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                exec_kwargs.update(
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.PIPE,
+                )
             exec_cmd = subprocess.Popen(self.command, **exec_kwargs)
             exec_cmd.wait()
         if exec_cmd.stdout:
-            exec_cmd.hstdout = exec_cmd.stdout
             result.update(
                 stdout=(
                     "<LargeOutput>"
                     if self.large_output
                     else exec_cmd.stdout.read().decode("utf-8")
                 )
             )
-            exec_cmd.hstdout.close()
+            exec_cmd.stdout.close()
         else:
             exec_cmd.stdout = "<Interactive>"
             result.update(stdout="<Interactive>")
         if exec_cmd.stderr:
-            exec_cmd.hstderr = exec_cmd.stderr
-            exec_cmd.stderr = exec_cmd.stderr.read().decode("utf-8")
-            exec_cmd.hstderr.close()
-            result.update(stderr=exec_cmd.stderr)
+            result.update(stderr=exec_cmd.stderr.read().decode("utf-8"))
+            exec_cmd.stderr.close()
         result.pid = exec_cmd.pid
         result.failed = exec_cmd.returncode > 0
         result.succeeded = not result.failed
         result.success = result.succeeded
         result.failure = result.failed
         result.data = loaded_json = None
         if self.load_json:
             if result.failed:
-                err = f"{self} did not succeed; cannot return JSON from failure"
+                err = f"Command @ {self.command} did not succeed; cannot return JSON from failure!"
                 LOGGER.critical(err)
                 LOGGER.critical(result.stderr)
                 raise RuntimeError(err)
-            import json
 
             try:
                 loaded_json = json.loads(result.stdout)
             except (json.decoder.JSONDecodeError,) as exc:
                 loaded_json = dict(error=str(exc))
+
         if self.strict and not result.succeeded:
             LOGGER.critical(f"Invocation failed and strict={self.strict}")
-            # raise InvocationError
-            LOGGER.critical(result.stderr)
-            raise RuntimeError(result.stderr)
+            LOGGER.critical(f"\n{result.stdout}")
+            LOGGER.critical(f"\n{result.stderr}")
+            raise RuntimeError()
+        if self.output_logger:
+            self.output_logger(result)
         return result
 
+    def __rich_console__(self, _console, options):  # noqa
+        """
+        https://rich.readthedocs.io/en/stable/protocol.html
+        """
+        fmt = shfmt(self.command)
+        extras = [
+            f"[yellow]{attr}=1" if getattr(self, attr, None) else ""
+            for attr in "system stdin interactive strict".split()
+        ]
+        extras = " ".join(extras)
+        yield self.command
+        yield console.Panel(
+            f"[bold gold3]$ [dim italic pale_green3]{fmt}",
+            title=(f"{self.__class__.__name__} {extras}"),
+            title_align="left",
+            style=console.Style(bgcolor="grey19"),
+            subtitle=console.Text("not executed yet", style="yellow"),
+        )
+
 
 class InvocationResult(Invocation):
     data: typing.Optional[typing.Dict] = Field(
         default=None, help="Data loaded from JSON on stdout"
     )
     failed: bool = Field(default=None, help="")
     failure: bool = Field(default=None, help="")
     succeeded: bool = Field(default=None, help="")
     success: bool = Field(default=None, help="")
     stdout: str = Field(default=None, help="")
     stderr: str = Field(default=None, help="")
     return_code: int = Field(default=-1, help="")
     pid: int = Field(default=-1, help="")
 
-    def __rich_console__(self, console, options):  # noqa
+    def __rich_console__(self, _console, options):  # noqa
         """
         https://rich.readthedocs.io/en/stable/protocol.html
         """
 
         def status_string():
             if self.succeeded is None:
                 return "??"
             else:
-                return "[cyan]=> [green]ok" if self.succeeded else "[red]failed"
+                return "[cyan]🠦 [green]ok" if self.succeeded else "[red]failed"
 
         fmt = shfmt(self.command)
-        syntax = Syntax(
-            f"{fmt}",
-            # f"[dim]$[/dim] [b]{fmt}[/b]",
-            "bash",
-            word_wrap=True,
-            line_numbers=False,
-        )
-        yield Panel(
-            syntax,
+        stcol = "[bold pale_green3]" if self.succeeded else "[red3]"
+        yield console.Panel(
+            f"[bold gold3]$ [dim]{fmt.strip()}\n{stcol} 🠦 [dim italic pale_green3]{self.stdout}",
             title=(
                 f"{self.__class__.__name__} from " f"pid {self.pid} {status_string()}"
             ),
+            style=console.Style(bgcolor="grey19"),
             title_align="left",
-            subtitle=Text("✔", style="green")
+            subtitle=console.Text("✔", style="green")
             if self.success
-            else Text("❌", style="red"),
+            else console.Text("❌", style="red"),
         )
```

### Comparing `shil-2023.7.15.12.33/src/shil/util.py` & `shil-2023.7.17.7.1/src/shil/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """ shil.util
 """
+import functools
+
 from fleks.util import lme
 
 LOGGER = lme.get_logger(__name__)
 
 
+def Runner(**kwargs):
+    return functools.partial(invoke, **kwargs)
+
+
 def invoke(*args, **kwargs):
     """ """
     from shil.models import Invocation
 
     if args:
         if len(args) == 1 and "command" not in kwargs:
             command = args[0]
             assert isinstance(command, (str,)), f"expected string, got {type(command)}"
             kwargs.update(command=command)
         else:
             raise ValueError("expected args[0] would be `command`!")
-    LOGGER.critical(kwargs)
+    # LOGGER.critical(kwargs)
     cmd = Invocation(**kwargs)
     return cmd()
```

### Comparing `shil-2023.7.15.12.33/src/shil.egg-info/PKG-INFO` & `shil-2023.7.17.7.1/src/shil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shil
-Version: 2023.7.15.12.33
+Version: 2023.7.17.7.1
 Summary: Shell helper utilities for python
 Home-page: https://github.com/elo-enterprises/shil/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/shil/
 Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shil Version: 2023.7.15.12.33 Summary: Shell helper
+Metadata-Version: 2.1 Name: shil Version: 2023.7.17.7.1 Summary: Shell helper
 utilities for python Home-page: https://github.com/elo-enterprises/shil/
 Author: elo License: MIT Project-URL: Documentation, https://github.com/elo-
 enterprises/shil/ Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files Platform:
 any Classifier: Programming Language :: Python Requires-Python: >3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Provides-
 Extra: dev Provides-Extra: testing Provides-Extra: lint Provides-Extra: publish
```

