# Comparing `tmp/task2b-1.0.18.tar.gz` & `tmp/task2b-1.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2b-1.0.18.tar", max compression
+gzip compressed data, was "task2b-1.0.19.tar", max compression
```

## Comparing `task2b-1.0.18.tar` & `task2b-1.0.19.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2b-1.0.18/LICENSE
--rw-r--r--   0        0        0      321 2023-07-08 15:34:54.474410 task2b-1.0.18/pwgen2/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 15:34:54.488388 task2b-1.0.18/pwgen2/__main__.py
--rw-r--r--   0        0        0       24 2023-07-11 09:08:07.390951 task2b-1.0.18/pwgen2/__version__.py
--rw-r--r--   0        0        0       74 2023-07-08 15:35:37.625438 task2b-1.0.18/pwgen2/cli/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 15:35:37.612436 task2b-1.0.18/pwgen2/cli/__main__.py
--rw-r--r--   0        0        0     4668 2023-07-11 09:05:02.736640 task2b-1.0.18/pwgen2/cli/cli.py
--rw-r--r--   0        0        0    10294 2023-07-11 09:05:02.737647 task2b-1.0.18/pwgen2/pwgen2.py
--rw-r--r--   0        0        0       94 2023-07-08 15:35:37.620439 task2b-1.0.18/pwgen2/showcase/__init__.py
--rw-r--r--   0        0        0      133 2023-07-08 15:35:37.616441 task2b-1.0.18/pwgen2/showcase/__main__.py
--rw-r--r--   0        0        0      132 2023-07-11 09:05:02.737647 task2b-1.0.18/pwgen2/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      276 2023-07-11 09:05:02.738638 task2b-1.0.18/pwgen2/showcase/pattern-list.txt
--rw-r--r--   0        0        0    23176 2023-07-11 09:05:02.738638 task2b-1.0.18/pwgen2/showcase/showcase.py
--rw-r--r--   0        0        0      588 2023-07-11 09:08:07.395955 task2b-1.0.18/pyproject.toml
--rw-r--r--   0        0        0    17425 2023-07-11 09:05:02.726644 task2b-1.0.18/README.md
--rw-r--r--   0        0        0    17821 1970-01-01 00:00:00.000000 task2b-1.0.18/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2b-1.0.19/LICENSE
+-rw-r--r--   0        0        0      321 2023-07-08 15:34:54.474410 task2b-1.0.19/pwgen2/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 15:34:54.488388 task2b-1.0.19/pwgen2/__main__.py
+-rw-r--r--   0        0        0       24 2023-07-17 10:52:08.503168 task2b-1.0.19/pwgen2/__version__.py
+-rw-r--r--   0        0        0       74 2023-07-08 15:35:37.625438 task2b-1.0.19/pwgen2/cli/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 15:35:37.612436 task2b-1.0.19/pwgen2/cli/__main__.py
+-rw-r--r--   0        0        0     4668 2023-07-11 09:05:02.736640 task2b-1.0.19/pwgen2/cli/cli.py
+-rw-r--r--   0        0        0    10697 2023-07-17 10:52:08.493180 task2b-1.0.19/pwgen2/pwgen2.py
+-rw-r--r--   0        0        0       94 2023-07-08 15:35:37.620439 task2b-1.0.19/pwgen2/showcase/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-08 15:35:37.616441 task2b-1.0.19/pwgen2/showcase/__main__.py
+-rw-r--r--   0        0        0      132 2023-07-11 09:05:02.737647 task2b-1.0.19/pwgen2/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      276 2023-07-11 09:05:02.738638 task2b-1.0.19/pwgen2/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    23290 2023-07-17 10:45:09.379089 task2b-1.0.19/pwgen2/showcase/showcase.py
+-rw-r--r--   0        0        0      587 2023-07-17 10:52:08.498157 task2b-1.0.19/pyproject.toml
+-rw-r--r--   0        0        0    17425 2023-07-11 09:05:02.726644 task2b-1.0.19/README.md
+-rw-r--r--   0        0        0    17920 1970-01-01 00:00:00.000000 task2b-1.0.19/PKG-INFO
```

### Comparing `task2b-1.0.18/pwgen2/cli/cli.py` & `task2b-1.0.19/pwgen2/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2b-1.0.18/pwgen2/pwgen2.py` & `task2b-1.0.19/pwgen2/pwgen2.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,28 +36,38 @@
     'z': 'BCDFGHJKLMNPQRSTVWXYZ',
     'b': '()[]{}<>',
     's': '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~',
     'S': string.ascii_lowercase + string.ascii_uppercase + string.digits + '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~',
     'x': '¡¢£¤¥¦§¨©ª«¬®¯°±²³´µ¶·¸¹º»¼½¾¿ÀÁÂÃÄÅÆÇÈÉÊËÌÍÎÏÐÑÒÓÔÕÖ×ÙÚÛÜÝÞßàáâãäåæçèéêëìíîïðñòóôõö÷øùúûüýþÿ',
 }
 
-CHARACTER_SETS |= EXTENDED_CHARACTER_SETS
+# CHARACTER_SETS |= EXTENDED_CHARACTER_SETS
+CHARACTER_SETS.update(EXTENDED_CHARACTER_SETS)
 
 
 def set_log_level(level: int) -> None:
-    match level:
-        case 1:
-            console_handler.setLevel(logging.WARNING)
-            logger.setLevel(logging.WARNING)
-        case 2:
-            console_handler.setLevel(logging.INFO)
-            logger.setLevel(logging.INFO)
-        case v if v >= 3:
-            console_handler.setLevel(logging.DEBUG)
-            logger.setLevel(logging.DEBUG)
+    # match level:
+    #     case 1:
+    #         console_handler.setLevel(logging.WARNING)
+    #         logger.setLevel(logging.WARNING)
+    #     case 2:
+    #         console_handler.setLevel(logging.INFO)
+    #         logger.setLevel(logging.INFO)
+    #     case v if v >= 3:
+    #         console_handler.setLevel(logging.DEBUG)
+    #         logger.setLevel(logging.DEBUG)
+    if level == 1:
+        console_handler.setLevel(logging.WARNING)
+        logger.setLevel(logging.WARNING)
+    elif level == 2:
+        console_handler.setLevel(logging.INFO)
+        logger.setLevel(logging.INFO)
+    elif level >= 3:
+        console_handler.setLevel(logging.DEBUG)
+        logger.setLevel(logging.DEBUG)
 
 
 def packet_version() -> str:
     return __version__
 
 
 def split_placeholders(placeholders: str) -> List[str]:
```

### Comparing `task2b-1.0.18/pwgen2/showcase/showcase.py` & `task2b-1.0.19/pwgen2/showcase/showcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import os
 import platform
 import subprocess
 import sys
 import time
-from typing import Dict, List
+from typing import Dict, List, Union
 
 import questionary
 import select
 from questionary import prompt, Choice
 
 if sys.platform.startswith('win32'):
     import msvcrt
@@ -116,15 +116,16 @@
         'message': 'What logging level would you like to set?',
         'default': '0',
         'validation': lambda val: True if val.isdigit() else 'Please, provide a number',
         'filter': lambda val: f'{"-" if int(val) > 0 else ""}{"v" * (int(val) if int(val) <= 3 else 3)}',
     },
 }
 
-OPTIONS: Dict[str, Dict[str, str | List[Dict] | Dict[str, Dict[str, str | List[Dict]]]]] = {
+# OPTIONS: Dict[str, Dict[str, str | List[Dict] | Dict[str, Dict[str, str | List[Dict]]]]] = {
+OPTIONS: Dict[str, Dict[str, Union[str, List[Dict], Dict[str, Dict[str, Union[str, List[Dict]]]]]]] = {
     'charset': {
         'descr': 'character sets',
         'options': {
             'charset_default': {
                 'descr': 'default charset',
                 'command': 'pwgen2 -n{} -c{} {}',
                 'module_command': f'{python_command} pwgen2 -n{{}} -c{{}} {{}}',
```

### Comparing `task2b-1.0.18/pyproject.toml` & `task2b-1.0.19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "task2b"
-version = "1.0.18"
+version = "1.0.19"
 description = "Password generation CLI and library version 2"
 repository = "https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2b"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pwgen2"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 questionary = "^1.10.0"
 
 [tool.poetry.scripts]
 pwgen2 = "pwgen2:pwgen_cli"
 pwgen2_showcase = "pwgen2.showcase:pwgen_showcase"
```

### Comparing `task2b-1.0.18/README.md` & `task2b-1.0.19/README.md`

 * *Files identical despite different names*

### Comparing `task2b-1.0.18/PKG-INFO` & `task2b-1.0.19/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: task2b
-Version: 1.0.18
+Version: 1.0.19
 Summary: Password generation CLI and library version 2
 Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2b
 License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2b
 Description-Content-Type: text/markdown
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: task2b Version: 1.0.18 Summary: Password generation
+Metadata-Version: 2.1 Name: task2b Version: 1.0.19 Summary: Password generation
 CLI and library version 2 Home-page: https://gitlab.com/Bill-EPAM-
 DevOpsInt2023/python/task2b License: MIT Author: Bill.Avramenko Author-email:
-billavramenko@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
+billavramenko@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0)
-Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
-task2b Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: questionary
+(>=1.10.0,<2.0.0) Project-URL: Repository, https://gitlab.com/Bill-EPAM-
+DevOpsInt2023/python/task2b Description-Content-Type: text/markdown
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                             Password generator v2.
                           Module 2: Python. Task 2B.
                  [PYPI_v.]  [License]  [License]  [Python_v.] 
 ## Preface This project contains a solution to one of the tasks of the EPAM
 DevOps Initial Internal Training Course #7 in 2023. Detailed information about
 the course, as well as reports on each of the completed tasks (including this
```

