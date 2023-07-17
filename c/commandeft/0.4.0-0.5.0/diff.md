# Comparing `tmp/commandeft-0.4.0.tar.gz` & `tmp/commandeft-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandeft-0.4.0.tar", last modified: Fri Jul 14 13:43:57 2023, max compression
+gzip compressed data, was "commandeft-0.5.0.tar", last modified: Mon Jul 17 08:10:37 2023, max compression
```

## Comparing `commandeft-0.4.0.tar` & `commandeft-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1078 2023-06-10 01:12:32.215348 commandeft-0.4.0/LICENSE
--rw-r--r--   0        0        0     3541 2023-07-13 06:12:07.752921 commandeft-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-06-11 23:37:24.840096 commandeft-0.4.0/commandeft/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009549 commandeft-0.4.0/commandeft/constants/__init__.py
--rw-r--r--   0        0        0     3265 2023-07-14 13:43:43.639342 commandeft-0.4.0/commandeft/constants/consts.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009834 commandeft-0.4.0/commandeft/core/__init__.py
--rw-r--r--   0        0        0     3065 2023-07-14 13:43:43.640135 commandeft-0.4.0/commandeft/core/cli.py
--rw-r--r--   0        0        0     1477 2023-07-14 13:43:43.640917 commandeft-0.4.0/commandeft/core/decision.py
--rw-r--r--   0        0        0     5054 2023-07-13 18:28:25.095963 commandeft-0.4.0/commandeft/core/generation.py
--rw-r--r--   0        0        0     2131 2023-07-13 06:12:07.759538 commandeft-0.4.0/commandeft/core/history_cache.py
--rw-r--r--   0        0        0      913 2023-07-13 06:12:07.760737 commandeft-0.4.0/commandeft/main.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.010171 commandeft-0.4.0/commandeft/util/__init__.py
--rw-r--r--   0        0        0     4961 2023-07-14 13:43:43.641629 commandeft-0.4.0/commandeft/util/config_util.py
--rw-r--r--   0        0        0      370 2023-07-13 06:12:07.762484 commandeft-0.4.0/commandeft/util/gen_util.py
--rw-r--r--   0        0        0     2438 2023-07-14 13:43:43.642519 commandeft-0.4.0/commandeft/util/interactive_util.py
--rw-r--r--   0        0        0     1995 2023-07-14 13:43:57.206047 commandeft-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5453 1970-01-01 00:00:00.000000 commandeft-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-10 01:12:32.215348 commandeft-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3541 2023-07-13 06:12:07.752921 commandeft-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 23:37:24.840096 commandeft-0.5.0/commandeft/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009549 commandeft-0.5.0/commandeft/constants/__init__.py
+-rw-r--r--   0        0        0     3265 2023-07-14 13:43:43.639342 commandeft-0.5.0/commandeft/constants/consts.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009834 commandeft-0.5.0/commandeft/core/__init__.py
+-rw-r--r--   0        0        0     2965 2023-07-17 08:10:22.558514 commandeft-0.5.0/commandeft/core/cli.py
+-rw-r--r--   0        0        0     1477 2023-07-14 13:43:43.640917 commandeft-0.5.0/commandeft/core/decision.py
+-rw-r--r--   0        0        0     5054 2023-07-13 18:28:25.095963 commandeft-0.5.0/commandeft/core/generation.py
+-rw-r--r--   0        0        0     2131 2023-07-13 06:12:07.759538 commandeft-0.5.0/commandeft/core/history_cache.py
+-rw-r--r--   0        0        0     1023 2023-07-17 08:10:22.559532 commandeft-0.5.0/commandeft/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:40:57.010171 commandeft-0.5.0/commandeft/util/__init__.py
+-rw-r--r--   0        0        0     4961 2023-07-14 13:43:43.641629 commandeft-0.5.0/commandeft/util/config_util.py
+-rw-r--r--   0        0        0      370 2023-07-13 06:12:07.762484 commandeft-0.5.0/commandeft/util/gen_util.py
+-rw-r--r--   0        0        0     2438 2023-07-14 13:43:43.642519 commandeft-0.5.0/commandeft/util/interactive_util.py
+-rw-r--r--   0        0        0     1202 2023-07-17 08:10:22.560060 commandeft-0.5.0/commandeft/util/versioning_util.py
+-rw-r--r--   0        0        0     2018 2023-07-17 08:10:37.771165 commandeft-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 commandeft-0.5.0/PKG-INFO
```

### Comparing `commandeft-0.4.0/LICENSE` & `commandeft-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commandeft-0.4.0/README.md` & `commandeft-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `commandeft-0.4.0/commandeft/constants/consts.py` & `commandeft-0.5.0/commandeft/constants/consts.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.4.0/commandeft/core/cli.py` & `commandeft-0.5.0/commandeft/core/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import shutil
 import json
-from importlib.metadata import version
 import click
 import pyperclip
 
 
 from commandeft.constants.consts import COMMANDEFT_ASCII_DESC, COMMANDEFT_NORMAL_DESC, CONFIG_FILE_PATH
 from commandeft.core.decision import decide_and_apply_action
 from commandeft.core.generation import Generation
@@ -85,11 +84,7 @@
     generation_config["mode"] = "inline"
     generation = Generation(generation_config)
 
     command = generation.generate_command(prompt)
     click.echo(click.style("> " + command, fg="green"))
     pyperclip.copy(command)
     click.echo("Command copied to clipboard!")
-
-
-def print_version():
-    click.echo(version("commandeft"))
```

### Comparing `commandeft-0.4.0/commandeft/core/decision.py` & `commandeft-0.5.0/commandeft/core/decision.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.4.0/commandeft/core/generation.py` & `commandeft-0.5.0/commandeft/core/generation.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.4.0/commandeft/core/history_cache.py` & `commandeft-0.5.0/commandeft/core/history_cache.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.4.0/commandeft/main.py` & `commandeft-0.5.0/commandeft/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import click
 
-from commandeft.core.cli import CustomCommand, configuration_mode, print_version, prompt_in_line, interactive_mode
+from commandeft.core.cli import CustomCommand, configuration_mode, prompt_in_line, interactive_mode
+from commandeft.util.versioning_util import check_for_updates, get_version
 
 
 @click.command(cls=CustomCommand)
 @click.help_option("-h", "--help")
 @click.option("-v", "--version", help="Show version and exit", is_flag=True)
 @click.option("-c", "--configure", help="Configure commandeft", is_flag=True)
 @click.option("-i", "--interactive", help="Run in interactive mode", is_flag=True)
 @click.option("-p", "--prompt", help="Specify your prompt inline")
 def commandeft(version, configure, interactive, prompt):
+    check_for_updates()
     if version:
-        print_version()
+        click.echo("installed: " + get_version())
     elif configure:
         configuration_mode()
     elif interactive:
         interactive_mode()
     elif prompt:
         prompt_in_line(prompt)
     else:
```

### Comparing `commandeft-0.4.0/commandeft/util/config_util.py` & `commandeft-0.5.0/commandeft/util/config_util.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.4.0/commandeft/util/interactive_util.py` & `commandeft-0.5.0/commandeft/util/interactive_util.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.4.0/pyproject.toml` & `commandeft-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "commandeft"
-version = "0.4.0"
+version = "0.5.0"
 description = "CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models."
 readme = "README.md"
 authors = [
     { name = "Petros Sidirokastritis", email = "sidirope@gmail.com" },
 ]
 requires-python = ">=3.8.1, <=3.11.4"
 dependencies = [
@@ -33,14 +33,15 @@
     "six==1.16.0",
     "tqdm==4.65.0",
     "urllib3==2.0.2",
     "wcwidth==0.2.6",
     "yarl<2.0,>=1.0",
     "InquirerPy>=0.3.4",
     "tiktoken>=0.4.0",
+    "packaging>=23.1",
 ]
 keywords = [
     "commandeft",
     "cli tool",
     "shell commands",
     "prompt-based command generation",
     "natural language prompts",
```

### Comparing `commandeft-0.4.0/PKG-INFO` & `commandeft-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandeft
-Version: 0.4.0
+Version: 0.5.0
 Summary: CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models.
 Keywords: commandeft cli tool shell commands prompt-based command generation natural language prompts shell commands shell scripts shell command generation intelligent code generation language-to-code conversion developer-friendly simplified scripting code efficiency streamline workflow intelligent suggestions efficient command composition gpt-3.5-turbo gpt-4 shell command suggestion interactive mode guided prompt command execution
 Author-Email: Petros Sidirokastritis <sidirope@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Ferrum-Citadel/commandeft
 Requires-Python: <=3.11.4,>=3.8.1
 Requires-Dist: PyJWT==2.7.0
@@ -32,14 +32,15 @@
 Requires-Dist: six==1.16.0
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: urllib3==2.0.2
 Requires-Dist: wcwidth==0.2.6
 Requires-Dist: yarl<2.0,>=1.0
 Requires-Dist: InquirerPy>=0.3.4
 Requires-Dist: tiktoken>=0.4.0
+Requires-Dist: packaging>=23.1
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-pep8; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # CommanDeft
```

