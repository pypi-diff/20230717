# Comparing `tmp/examon_core-1.0.4.tar.gz` & `tmp/examon_core-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-1.0.4.tar", max compression
+gzip compressed data, was "examon_core-1.0.5.tar", max compression
```

## Comparing `examon_core-1.0.4.tar` & `examon_core-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.4/examon_core/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-15 20:10:36.790579 examon_core-1.0.4/examon_core/code_metrics.py
--rwxr-xr-x   0        0        0      705 2023-05-28 20:45:23.567671 examon_core-1.0.4/examon_core/examon_item.py
--rwxr-xr-x   0        0        0      478 2023-06-23 14:39:27.007604 examon_core-1.0.4/examon_core/examon_item_registry.py
--rwxr-xr-x   0        0        0     1761 2023-06-23 14:39:27.015545 examon_core-1.0.4/examon_core/function_raw_code.py
--rw-r--r--   0        0        0      389 2023-06-23 14:39:26.999135 examon_core-1.0.4/examon_core/multi_choice_factory.py
--rw-r--r--   0        0        0      950 2023-07-15 22:19:35.785327 examon_core-1.0.4/examon_core/print_ext.py
--rwxr-xr-x   0        0        0      621 2023-05-23 09:37:48.400052 examon_core-1.0.4/examon_core/question.py
--rw-r--r--   0        0        0     2525 2023-06-23 14:33:10.050623 examon_core-1.0.4/examon_core/question_factory.py
--rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.0.4/examon_core/question_response.py
--rw-r--r--   0        0        0      107 2023-06-23 14:39:27.010739 examon_core-1.0.4/examon_core/todo.md
--rw-r--r--   0        0        0      517 2023-07-15 22:21:58.826766 examon_core-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 examon_core-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.5/examon_core/__init__.py
+-rw-r--r--   0        0        0     1039 2023-07-16 08:19:13.878728 examon_core-1.0.5/examon_core/code_metrics.py
+-rwxr-xr-x   0        0        0      574 2023-07-17 15:50:11.694400 examon_core-1.0.5/examon_core/examon_item.py
+-rwxr-xr-x   0        0        0      479 2023-07-16 08:19:13.894322 examon_core-1.0.5/examon_core/examon_item_registry.py
+-rwxr-xr-x   0        0        0     1697 2023-07-16 08:20:56.019327 examon_core-1.0.5/examon_core/function_raw_code.py
+-rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.0.5/examon_core/multi_choice_factory.py
+-rw-r--r--   0        0        0      980 2023-07-16 08:19:13.846489 examon_core-1.0.5/examon_core/print_ext.py
+-rwxr-xr-x   0        0        0      620 2023-07-16 08:19:13.933636 examon_core-1.0.5/examon_core/question.py
+-rw-r--r--   0        0        0     2591 2023-07-16 08:19:13.826878 examon_core-1.0.5/examon_core/question_factory.py
+-rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.0.5/examon_core/question_response.py
+-rw-r--r--   0        0        0      107 2023-07-17 15:48:04.895960 examon_core-1.0.5/examon_core/todo.md
+-rw-r--r--   0        0        0      517 2023-07-17 15:51:48.352026 examon_core-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 examon_core-1.0.5/PKG-INFO
```

### Comparing `examon_core-1.0.4/examon_core/code_metrics.py` & `examon_core-1.0.5/examon_core/code_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from dataclasses import dataclass
 
 
 from radon.raw import analyze
 from radon.metrics import h_visit
 
+
 @dataclass
 class CodeMetrics:
     code_as_string: str
     no_of_functions: int = None
     loc: int = None
     lloc: int = None
     sloc: int = None
```

### Comparing `examon_core-1.0.4/examon_core/function_raw_code.py` & `examon_core-1.0.5/examon_core/function_raw_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import re
 import logging
 
+
 class RawCodeFactory:
     @staticmethod
     def build(function, decorators=[]):
         src_code = RawCodeFactory.function_src(function)
         for decorator in decorators:
             logging.debug(f'RawCodeFactory.build: {decorator}')
             src_code = decorator.decorate(src_code)
@@ -46,12 +47,11 @@
 
     def decorate(self, src_code):
         println = f'\n\nprint({self.function_name}())'
         return src_code + println
 
 
 def function_raw_code(function, hints):
-    code_comments_decorator = SourceCodeCommentsDecorator(hints)
     append_print_decorator = AppendPrintDecorator(function.__name__)
     remove_quiz_item_decorator = RemoveQuizItemDecorator()
     decorators = [remove_quiz_item_decorator, append_print_decorator]
     return RawCodeFactory.build(function, decorators)
```

### Comparing `examon_core-1.0.4/examon_core/print_ext.py` & `examon_core-1.0.5/examon_core/print_ext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 import builtins
 from contextlib import redirect_stdout
 import io
 from inspect import getframeinfo, stack
 
+
 @dataclass
 class PrintLogItem:
     output: str
     line_no: int
 
 
 class PrintLog:
@@ -20,15 +21,17 @@
     @classmethod
     def logs(cls):
         return cls.print_logs
 
     @classmethod
     def apply_offset(cls, offset):
         def offset_pl(print_log_item):
-            return PrintLogItem(print_log_item.output, print_log_item.line_no - offset)
+            return PrintLogItem(
+                print_log_item.output,
+                print_log_item.line_no - offset)
 
         cls.print_logs = list(map(offset_pl, cls.print_logs))
 
     @classmethod
     def reset(cls):
         cls.print_logs = []
 
@@ -36,8 +39,8 @@
 def print(*args, **kwargs):
     caller = getframeinfo(stack()[1][0])
     f = io.StringIO()
 
     with redirect_stdout(f):
         builtins.print(*args, **kwargs)
     s = f.getvalue().rstrip()
-    PrintLog.append(PrintLogItem    (s, caller.lineno))
+    PrintLog.append(PrintLogItem(s, caller.lineno))
```

### Comparing `examon_core-1.0.4/examon_core/question.py` & `examon_core-1.0.5/examon_core/question.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 @dataclass
 class ExpectedResultQuestion(BaseQuestion):
     correct_answer: str = None
 
 
-
 @dataclass
 class InputParameterQuestion(BaseQuestion):
     return_value: str = None
     selected_param: str = None
 
     def answer(self, choice):
         return choice == self.selected_param
```

### Comparing `examon_core-1.0.4/examon_core/question_factory.py` & `examon_core-1.0.5/examon_core/question_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .function_raw_code import function_raw_code
 from .print_ext import PrintLog
 from .code_metrics import CodeMetricsFactory
 
 import random
 import logging
 
+
 class QuestionFactory:
     @staticmethod
     def build(**kwargs):
         function = kwargs['function']
         tags = kwargs['tags']
         hints = kwargs['hints']
         param1 = kwargs['param1'] if 'param1' in kwargs else None
@@ -43,16 +44,18 @@
             correct_answer = QuestionFactory.run_function(function=function)
             PrintLog.apply_offset(first_line_no)
             print_logs = PrintLog.logs()
             PrintLog.reset()
 
             if choice_list is not None:
                 question = ExpectedResultQuestion(
-                    choices=(MultiChoiceFactory.build(correct_answer, choice_list))
-                )
+                    choices=(
+                        MultiChoiceFactory.build(
+                            correct_answer,
+                            choice_list)))
             else:
                 question = BaseQuestion()
             question.correct_answer = correct_answer
 
         question.metrics = metrics
         question.hints = hints
         question.tags = tags
```

### Comparing `examon_core-1.0.4/pyproject.toml` & `examon_core-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "examon_core"
-version = "1.0.4"
+version = "1.0.5"
 description = "Examon Core Libs"
 authors = ["Jarrod Folino <jdfolino@icloud.com>"]
 packages = [{include = "examon_core"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 radon = "^6.0.1"
```

