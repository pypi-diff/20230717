# Comparing `tmp/task2a-1.0.21.tar.gz` & `tmp/task2a-1.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2a-1.0.21.tar", max compression
+gzip compressed data, was "task2a-1.0.22.tar", max compression
```

## Comparing `task2a-1.0.21.tar` & `task2a-1.0.22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.21/LICENSE
--rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.21/pwgen/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.21/pwgen/__main__.py
--rw-r--r--   0        0        0       24 2023-07-11 00:04:03.245005 task2a-1.0.21/pwgen/__version__.py
--rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.21/pwgen/cli/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.21/pwgen/cli/__main__.py
--rw-r--r--   0        0        0     4662 2023-07-10 16:33:21.655774 task2a-1.0.21/pwgen/cli/cli.py
--rw-r--r--   0        0        0     8650 2023-07-11 00:04:03.249999 task2a-1.0.21/pwgen/pwgen.py
--rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.21/pwgen/showcase/__init__.py
--rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.21/pwgen/showcase/__main__.py
--rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.21/pwgen/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      171 2023-07-10 22:30:44.973674 task2a-1.0.21/pwgen/showcase/pattern-list.txt
--rw-r--r--   0        0        0    20824 2023-07-10 23:57:09.275818 task2a-1.0.21/pwgen/showcase/showcase.py
--rw-r--r--   0        0        0      686 2023-07-11 00:04:03.253997 task2a-1.0.21/pyproject.toml
--rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.21/README.md
--rw-r--r--   0        0        0    37291 1970-01-01 00:00:00.000000 task2a-1.0.21/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.22/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.22/pwgen/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.22/pwgen/__main__.py
+-rw-r--r--   0        0        0       24 2023-07-17 10:32:48.937984 task2a-1.0.22/pwgen/__version__.py
+-rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.22/pwgen/cli/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.22/pwgen/cli/__main__.py
+-rw-r--r--   0        0        0     4662 2023-07-10 16:33:21.655774 task2a-1.0.22/pwgen/cli/cli.py
+-rw-r--r--   0        0        0     9003 2023-07-17 10:29:06.782767 task2a-1.0.22/pwgen/pwgen.py
+-rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.22/pwgen/showcase/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.22/pwgen/showcase/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.22/pwgen/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      171 2023-07-10 22:30:44.973674 task2a-1.0.22/pwgen/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    20938 2023-07-17 10:31:01.885394 task2a-1.0.22/pwgen/showcase/showcase.py
+-rw-r--r--   0        0        0      685 2023-07-17 10:32:48.932983 task2a-1.0.22/pyproject.toml
+-rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.22/README.md
+-rw-r--r--   0        0        0    37390 1970-01-01 00:00:00.000000 task2a-1.0.22/PKG-INFO
```

### Comparing `task2a-1.0.21/pwgen/cli/cli.py` & `task2a-1.0.22/pwgen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.21/pwgen/pwgen.py` & `task2a-1.0.22/pwgen/pwgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,33 @@
     'L': string.ascii_letters,  # Mixed-case lateral ASCII
     'u': string.ascii_uppercase,  # Big lateral ASCII
     'p': ',.;:',
 }
 
 
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

### Comparing `task2a-1.0.21/pwgen/showcase/showcase.py` & `task2a-1.0.22/pwgen/showcase/showcase.py`

 * *Files 2% similar despite different names*

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
@@ -117,15 +117,16 @@
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
                 'command': 'pwgen -n{} -c{} {}',
                 'module_command': f'{python_command} pwgen -n{{}} -c{{}} {{}}',
```

### Comparing `task2a-1.0.21/pyproject.toml` & `task2a-1.0.22/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "task2a"
-version = "1.0.21"
+version = "1.0.22"
 description = "Password generation CLI and library"
 repository = "https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pwgen"}]
 #packages = [{include = "pwgen", format = "sdist"}]
 license = "MIT"
 
 #[tool.poetry.build]
 #generate-setup-file = true
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 questionary = "^1.10.0"
 
 [tool.poetry.scripts]
 pwgen = "pwgen:pwgen_cli"
 pwgen_showcase = "pwgen.showcase:pwgen_showcase"
```

### Comparing `task2a-1.0.21/README.md` & `task2a-1.0.22/README.md`

 * *Files identical despite different names*

### Comparing `task2a-1.0.21/PKG-INFO` & `task2a-1.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: task2a
-Version: 1.0.21
+Version: 1.0.22
 Summary: Password generation CLI and library
 Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a
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
 Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a
 Description-Content-Type: text/markdown
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: task2a Version: 1.0.21 Summary: Password generation
+Metadata-Version: 2.1 Name: task2a Version: 1.0.22 Summary: Password generation
 CLI and library Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
 task2a License: MIT Author: Bill.Avramenko Author-email:
-billavramenko@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
+billavramenko@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0)
-Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
-task2a Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: questionary
+(>=1.10.0,<2.0.0) Project-URL: Repository, https://gitlab.com/Bill-EPAM-
+DevOpsInt2023/python/task2a Description-Content-Type: text/markdown
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                               Password generator.
                           Module 2: Python. Task 2A.
                  [PYPI_v.]  [License]  [License]  [Python_v.] 
 ## Preface This project contains a solution to one of the tasks of the EPAM
 DevOps Initial Internal Training Course #7 in 2023. Detailed information about
 the course, as well as reports on each of the completed tasks (including this
```

