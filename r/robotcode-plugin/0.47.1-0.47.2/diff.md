# Comparing `tmp/robotcode_plugin-0.47.1.tar.gz` & `tmp/robotcode_plugin-0.47.2.tar.gz`

## Comparing `robotcode_plugin-0.47.1.tar` & `robotcode_plugin-0.47.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/src/robotcode/plugin/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/src/robotcode/plugin/__version__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/src/robotcode/plugin/manager.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/src/robotcode/plugin/py.typed
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/src/robotcode/plugin/specs.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/src/robotcode/plugin/click_helper/aliases.py
--rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/src/robotcode/plugin/click_helper/options.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/src/robotcode/plugin/click_helper/types.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/README.md
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/pyproject.toml
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.1/PKG-INFO
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/src/robotcode/plugin/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/src/robotcode/plugin/__version__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/src/robotcode/plugin/manager.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/src/robotcode/plugin/py.typed
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/src/robotcode/plugin/specs.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/src/robotcode/plugin/click_helper/aliases.py
+-rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/src/robotcode/plugin/click_helper/options.py
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/src/robotcode/plugin/click_helper/types.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/README.md
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/pyproject.toml
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 robotcode_plugin-0.47.2/PKG-INFO
```

### Comparing `robotcode_plugin-0.47.1/src/robotcode/plugin/__init__.py` & `robotcode_plugin-0.47.2/src/robotcode/plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass
 from enum import Enum, unique
 from pathlib import Path
 from typing import IO, Any, AnyStr, Callable, Iterable, Optional, Sequence, TypeVar, Union, cast
 
 import click
 import pluggy
+import tomli_w
 from robotcode.core.dataclasses import as_dict, as_json
 
 __all__ = [
     "hookimpl",
     "CommonConfig",
     "pass_application",
     "Application",
@@ -104,27 +105,21 @@
     def print_data(
         self, data: Any, remove_defaults: bool = True, default_output_format: Optional[OutputFormat] = None
     ) -> None:
         format = self.config.output_format or default_output_format or OutputFormat.TEXT
 
         text = None
         if format == OutputFormat.TOML:
-            try:
-                import tomli_w
-
-                text = tomli_w.dumps(
-                    as_dict(data, remove_defaults=remove_defaults)
-                    if dataclasses.is_dataclass(data)
-                    else data
-                    if isinstance(data, dict)
-                    else {data: data}
-                )
-            except ImportError:
-                self.warning("Package 'tomli_w' is required to use TOML output. Using JSON format instead.")
-                format = OutputFormat.JSON
+            text = tomli_w.dumps(
+                as_dict(data, remove_defaults=remove_defaults)
+                if dataclasses.is_dataclass(data)
+                else data
+                if isinstance(data, dict)
+                else {data: data}
+            )
 
         if text is None:
             if format in [OutputFormat.JSON, OutputFormat.JSON_INDENT]:
                 text = as_json(data, indent=format == OutputFormat.JSON_INDENT, compact=format == OutputFormat.TEXT)
             else:
                 text = str(data)
```

### Comparing `robotcode_plugin-0.47.1/src/robotcode/plugin/manager.py` & `robotcode_plugin-0.47.2/src/robotcode/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.47.1/src/robotcode/plugin/click_helper/aliases.py` & `robotcode_plugin-0.47.2/src/robotcode/plugin/click_helper/aliases.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.47.1/src/robotcode/plugin/click_helper/options.py` & `robotcode_plugin-0.47.2/src/robotcode/plugin/click_helper/options.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.47.1/src/robotcode/plugin/click_helper/types.py` & `robotcode_plugin-0.47.2/src/robotcode/plugin/click_helper/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.47.1/.gitignore` & `robotcode_plugin-0.47.2/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.47.1/LICENSE.txt` & `robotcode_plugin-0.47.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.47.1/README.md` & `robotcode_plugin-0.47.2/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.47.1/pyproject.toml` & `robotcode_plugin-0.47.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
-dependencies = ["click>=8.0.0", "pluggy>=1.0.0"]
+dependencies = ["click>=8.0.0", "pluggy>=1.0.0", "tomli_w>=1.0.0"]
 dynamic = ["version"]
 
 [project.urls]
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
 Changelog = "https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md"
 Issues = "https://github.com/d-biehl/robotcode/issues"
```

### Comparing `robotcode_plugin-0.47.1/PKG-INFO` & `robotcode_plugin-0.47.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-plugin
-Version: 0.47.1
+Version: 0.47.2
 Summary: Some classes for RobotCode plugin management
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
 Author-email: Daniel Biehl <dbiehl@live.de>
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: click>=8.0.0
 Requires-Dist: pluggy>=1.0.0
+Requires-Dist: tomli-w>=1.0.0
 Description-Content-Type: text/markdown
 
 # robotcode-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-plugin.svg)](https://pypi.org/project/robotcode-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-plugin.svg)](https://pypi.org/project/robotcode-plugin)
 [![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
```

