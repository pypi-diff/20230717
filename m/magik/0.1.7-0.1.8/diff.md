# Comparing `tmp/magik-0.1.7.tar.gz` & `tmp/magik-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magik-0.1.7.tar", last modified: Mon Jul 17 11:27:10 2023, max compression
+gzip compressed data, was "magik-0.1.8.tar", last modified: Mon Jul 17 13:25:17 2023, max compression
```

## Comparing `magik-0.1.7.tar` & `magik-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 11:27:10.930063 magik-0.1.7/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     4164 2023-07-17 11:27:10.929867 magik-0.1.7/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     3738 2023-07-14 14:03:48.000000 magik-0.1.7/README.md
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 11:27:10.924376 magik-0.1.7/magik/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.1.7/magik/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2349 2023-07-17 11:21:33.000000 magik-0.1.7/magik/cli.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      443 2023-07-17 11:22:00.000000 magik-0.1.7/magik/config.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      587 2023-07-17 11:02:45.000000 magik-0.1.7/magik/constants.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1385 2023-07-17 11:26:19.000000 magik-0.1.7/magik/deploy.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)    11751 2023-07-17 11:24:16.000000 magik-0.1.7/magik/evaluators.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 11:27:10.928817 magik-0.1.7/magik/examples/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.1.7/magik/examples/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2020 2023-07-14 12:27:41.000000 magik-0.1.7/magik/examples/assertions.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1331 2023-07-17 11:22:11.000000 magik-0.1.7/magik/generate.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2143 2023-07-17 11:22:17.000000 magik-0.1.7/magik/initialize.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-14 11:50:58.000000 magik-0.1.7/magik/internal_logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      596 2023-07-17 11:22:23.000000 magik-0.1.7/magik/logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.7/magik/matchers.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1031 2023-07-17 11:22:29.000000 magik-0.1.7/magik/openai_helper.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     7772 2023-07-17 11:22:35.000000 magik-0.1.7/magik/run.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2984 2023-07-17 11:22:40.000000 magik-0.1.7/magik/sys_exec.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      451 2023-07-16 17:12:15.000000 magik-0.1.7/magik/utils.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 11:27:10.928575 magik-0.1.7/magik.egg-info/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     4164 2023-07-17 11:27:10.000000 magik-0.1.7/magik.egg-info/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      518 2023-07-17 11:27:10.000000 magik-0.1.7/magik.egg-info/SOURCES.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-17 11:27:10.000000 magik-0.1.7/magik.egg-info/dependency_links.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-17 11:27:10.000000 magik-0.1.7/magik.egg-info/entry_points.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-17 11:27:10.000000 magik-0.1.7/magik.egg-info/requires.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-17 11:27:10.000000 magik-0.1.7/magik.egg-info/top_level.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-17 11:27:10.930401 magik-0.1.7/setup.cfg
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-17 11:25:34.000000 magik-0.1.7/setup.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 13:25:17.899994 magik-0.1.8/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     4164 2023-07-17 13:25:17.899864 magik-0.1.8/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3738 2023-07-14 14:03:48.000000 magik-0.1.8/README.md
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 13:25:17.898455 magik-0.1.8/magik/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.1.8/magik/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2379 2023-07-17 13:24:26.000000 magik-0.1.8/magik/cli.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-17 13:22:43.000000 magik-0.1.8/magik/config.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      587 2023-07-17 11:02:45.000000 magik-0.1.8/magik/constants.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1403 2023-07-17 13:21:09.000000 magik-0.1.8/magik/deploy.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)    11769 2023-07-17 13:21:36.000000 magik-0.1.8/magik/evaluators.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 13:25:17.899552 magik-0.1.8/magik/examples/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.1.8/magik/examples/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2020 2023-07-14 12:27:41.000000 magik-0.1.8/magik/examples/assertions.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1355 2023-07-17 13:21:44.000000 magik-0.1.8/magik/generate.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2161 2023-07-17 13:21:18.000000 magik-0.1.8/magik/initialize.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-14 11:50:58.000000 magik-0.1.8/magik/internal_logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      608 2023-07-17 13:22:27.000000 magik-0.1.8/magik/logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.8/magik/matchers.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1043 2023-07-17 13:21:56.000000 magik-0.1.8/magik/openai_helper.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     7808 2023-07-17 13:22:05.000000 magik-0.1.8/magik/run.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-17 13:22:12.000000 magik-0.1.8/magik/sys_exec.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      451 2023-07-16 17:12:15.000000 magik-0.1.8/magik/utils.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-17 13:25:17.899326 magik-0.1.8/magik.egg-info/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     4164 2023-07-17 13:25:17.000000 magik-0.1.8/magik.egg-info/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      518 2023-07-17 13:25:17.000000 magik-0.1.8/magik.egg-info/SOURCES.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-17 13:25:17.000000 magik-0.1.8/magik.egg-info/dependency_links.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-17 13:25:17.000000 magik-0.1.8/magik.egg-info/entry_points.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-17 13:25:17.000000 magik-0.1.8/magik.egg-info/requires.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-17 13:25:17.000000 magik-0.1.8/magik.egg-info/top_level.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-17 13:25:17.900033 magik-0.1.8/setup.cfg
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-17 13:25:01.000000 magik-0.1.8/setup.py
```

### Comparing `magik-0.1.7/PKG-INFO` & `magik-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.7
+Version: 0.1.8
 Summary: SDK to write and run tests for your LLM app
 Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `magik-0.1.7/README.md` & `magik-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `magik-0.1.7/magik/cli.py` & `magik-0.1.8/magik/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import argparse
-from initialize import initialize
-from generate import generate_test
-from deploy import deploy_test
-from internal_logger import logger
-from run import Run
+from magik.initialize import initialize
+from magik.generate import generate_test
+from magik.deploy import deploy_test
+from magik.internal_logger import logger
+from magik.run import Run
 
 commands = [
     "init",
     "generate",
     "run",
     "deploy",
 ]
```

### Comparing `magik-0.1.7/magik/constants.py` & `magik-0.1.8/magik/constants.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.7/magik/deploy.py` & `magik-0.1.8/magik/deploy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import requests
-from internal_logger import logger
-from constants import CONFIG_FILE_PATH, DEPLOY_URL, TEST_DIR
-from config import get_magik_api_key
+from magik.internal_logger import logger
+from magik.constants import CONFIG_FILE_PATH, DEPLOY_URL, TEST_DIR
+from magik.config import get_magik_api_key
 
 
 def deploy_test(test_name: str):
     api_key = get_magik_api_key()
     if api_key == None:
         logger.error(f"No API key found. Please add your API key to {CONFIG_FILE_PATH}")
```

### Comparing `magik-0.1.7/magik/evaluators.py` & `magik-0.1.8/magik/evaluators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Contains functions to evaluate assertions.
 import requests
 import json
 import re
 import ast
-from openai_helper import OpenAI
-from utils import standardize_url
-from constants import OPEN_AI_DEFAULT_MODEL
+from magik.openai_helper import OpenAI
+from magik.utils import standardize_url
+from magik.constants import OPEN_AI_DEFAULT_MODEL
 
 
 def generate_grading_prompt(output_to_evaluate, grading_criteria):
     return (
         """
     You are grading a response string according to a grading criteria given to you.
```

### Comparing `magik-0.1.7/magik/examples/assertions.py` & `magik-0.1.8/magik/examples/assertions.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.7/magik/generate.py` & `magik-0.1.8/magik/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from internal_logger import logger
-from constants import TEST_DIR
-from sys_exec import read_from_file, write_to_file
-from constants import EXAMPLES_DIR
+from magik.internal_logger import logger
+from magik.constants import TEST_DIR
+from magik.sys_exec import read_from_file, write_to_file
+from magik.constants import EXAMPLES_DIR
 import inspect
 
 
 # Get the path of the file within the module
 def _get_module_file_path(file_name):
     module = inspect.getmodule(_get_module_file_path)
     module_file_path = inspect.getfile(module)
```

### Comparing `magik-0.1.7/magik/initialize.py` & `magik-0.1.8/magik/initialize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
-from internal_logger import logger
-from sys_exec import write_to_file
-from constants import (
+from magik.internal_logger import logger
+from magik.sys_exec import write_to_file
+from magik.constants import (
     TESTRUNS_DIR,
     TEST_DIR,
     CONFIG_FILE_PATH,
 )
 from magik.sys_exec import read_from_file
```

### Comparing `magik-0.1.7/magik/internal_logger.py` & `magik-0.1.8/magik/internal_logger.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.7/magik/openai_helper.py` & `magik-0.1.8/magik/openai_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import openai
-from constants import API_BASE_URL
-from config import (
+from magik.constants import API_BASE_URL
+from magik.config import (
     get_open_ai_api_key,
     get_open_ai_default_model,
     get_magik_api_key,
 )
 
 
 class OpenAI:
```

### Comparing `magik-0.1.7/magik/run.py` & `magik-0.1.8/magik/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import requests
 import sys
 import importlib.util
 from datetime import datetime
-from internal_logger import logger
-from utils import substitute_vars
-from openai_helper import OpenAI
-from sys_exec import read_from_file, create_file
-from config import get_open_ai_default_model, get_magik_api_key
-from constants import TESTRUNS_DIR, TEST_DIR, RUN_URL
+from magik.internal_logger import logger
+from magik.utils import substitute_vars
+from magik.openai_helper import OpenAI
+from magik.sys_exec import read_from_file, create_file
+from magik.config import get_open_ai_default_model, get_magik_api_key
+from magik.constants import TESTRUNS_DIR, TEST_DIR, RUN_URL
 
 
 class Run:
     def __init__(self):
         self.saved_prompt_response = ""
 
     def run_tests(self, test_name):
```

### Comparing `magik-0.1.7/magik/sys_exec.py` & `magik-0.1.8/magik/sys_exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import os
 import json
 import subprocess
-from internal_logger import logger
+from magik.internal_logger import logger
 
 
 def execute_command(command, confirm=True, log=True):
     if confirm:
         confirmation = input(f"Run '{command}'? (y/n)")
         if confirmation != "y":
             return
```

### Comparing `magik-0.1.7/magik.egg-info/PKG-INFO` & `magik-0.1.8/magik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.7
+Version: 0.1.8
 Summary: SDK to write and run tests for your LLM app
 Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `magik-0.1.7/magik.egg-info/SOURCES.txt` & `magik-0.1.8/magik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magik-0.1.7/setup.py` & `magik-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="magik",
-    version="0.1.7",
+    version="0.1.8",
     author="Magik Labs Team",
     author_email="hello@magiklabs.app",
     description="SDK to write and run tests for your LLM app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

