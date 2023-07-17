# Comparing `tmp/typer_config-0.5.0.tar.gz` & `tmp/typer_config-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.5.0.tar", max compression
+gzip compressed data, was "typer_config-0.6.0.tar", max compression
```

## Comparing `typer_config-0.5.0.tar` & `typer_config-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-05-16 04:06:27.574721 typer_config-0.5.0/LICENSE
--rw-r--r--   0        0        0     1840 2023-05-18 01:01:35.696589 typer_config-0.5.0/README.md
--rw-r--r--   0        0        0     2612 2023-05-25 12:59:26.323443 typer_config-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4077 2023-05-25 12:57:11.693626 typer_config-0.5.0/typer_config/__init__.py
--rw-r--r--   0        0        0     1480 2023-05-25 12:57:02.863636 typer_config-0.5.0/typer_config/__typing.py
--rw-r--r--   0        0        0     9207 2023-05-25 12:57:02.863636 typer_config-0.5.0/typer_config/loaders.py
--rw-r--r--   0        0        0     3593 1970-01-01 00:00:00.000000 typer_config-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-01 15:54:43.337757 typer_config-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2473 2023-07-17 16:12:30.477542 typer_config-0.6.0/README.md
+-rw-r--r--   0        0        0     2651 2023-07-17 16:13:24.487598 typer_config-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      363 2023-07-17 15:34:49.905969 typer_config-0.6.0/typer_config/__init__.py
+-rw-r--r--   0        0        0      819 2023-07-17 15:34:49.909791 typer_config-0.6.0/typer_config/__optional_imports.py
+-rw-r--r--   0        0        0     1910 2023-07-17 15:34:49.913567 typer_config-0.6.0/typer_config/__typing.py
+-rw-r--r--   0        0        0     4086 2023-07-17 15:34:49.917414 typer_config-0.6.0/typer_config/callbacks.py
+-rw-r--r--   0        0        0     9482 2023-07-17 15:34:49.920773 typer_config-0.6.0/typer_config/decorators.py
+-rw-r--r--   0        0        0     1611 2023-07-17 15:34:49.924143 typer_config-0.6.0/typer_config/dumpers.py
+-rw-r--r--   0        0        0     8598 2023-07-17 15:34:49.928143 typer_config-0.6.0/typer_config/loaders.py
+-rw-r--r--   0        0        0     4226 1970-01-01 00:00:00.000000 typer_config-0.6.0/PKG-INFO
```

### Comparing `typer_config-0.5.0/LICENSE` & `typer_config-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_config-0.5.0/README.md` & `typer_config-0.6.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -25,8 +25,33 @@
 # Long commands like this:
 $ my-typer-app --opt1 foo --opt2 bar arg1 arg2
 
 # Can become this:
 $ my-typer-app --config config.yml
 ```
 
+## Quickstart
+
+You can use a decorator to quickly add a configuration parameter to your `typer` application:
+
+```py
+import typer
+from typer_config import use_yaml_config
+
+app = typer.Typer()
+
+
+@app.command()
+@use_yaml_config() # MUST BE AFTER @app.command()
+def main(...):
+    ...
+
+if __name__ == "__main__":
+    app()
+```
+
+Your typer command will now include a `--config CONFIG_FILE` option at the command line.
+
+> **Note**: this package also provides `@use_json_config`, `@use_toml_config`, and `@use_dotenv_config` for those file formats.
+> You can also use your own loader function and the `@use_config(loader_func)` decorator.
+
 See the [documentation](https://maxb2.github.io/typer-config/latest/examples/simple_yaml/) for more examples using typer-config.
```

### Comparing `typer_config-0.5.0/pyproject.toml` & `typer_config-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-config"
-version = "0.5.0"
+version = "0.6.0"
 description = "Utilities for working with configuration files in typer CLIs. "
 authors = ["Matt Anderson <matt@manderscience.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "typer_config"}]
 repository = "https://github.com/maxb2/typer-config"
 documentation = "https://maxb2.github.io/typer-config/"
@@ -50,34 +50,34 @@
 [tool.poetry.extras]
 python-dotenv = ["python-dotenv"]
 toml = ["toml"]
 yaml = ["pyyaml"]
 all = ["toml", "pyyaml", "python-dotenv"]
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.263"
+ruff = ">=0.0.263,<0.0.279"
 pylint = "^2.17.3"
 black = "^23.3.0"
 isort = "^5.12.0"
 pytest = "^7.3.1"
 mypy = "^1.2.0"
 types-toml = "^0.10.8.6"
 types-pyyaml = "^6.0.12.9"
-git-changelog = "^1.0.1"
-duty = "^0.11.0"
+git-changelog = ">=1.0.1,<3.0.0"
+duty = ">=0.11,<1.1"
 pytest-cov = "^4.0.0"
 safety = "^2.3.5"
-griffe = "^0.28.1"
+griffe = "^0.32.2"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1.9"
-mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+mkdocstrings = {extras = ["python"], version = ">=0.21.2,<0.23.0"}
 mike = "^1.1.2"
 mkdocs-gen-files = "^0.5.0"
-pydantic = "^1.10.7"
+pydantic = ">=1.10.7,<3.0.0"
 blacken-docs = { git = "https://github.com/maxb2/blacken-docs.git", rev = "b3c82da4df8eaca840b101d0aeab12ae029b6364" }
 schema = "^0.7.5"
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.format]
```

### Comparing `typer_config-0.5.0/typer_config/__init__.py` & `typer_config-0.6.0/typer_config/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Typer Configuration Utilities
-"""
+"""Typer Configuration Parameter Callbacks."""
 
 from typer import BadParameter, CallbackParam, Context
 
 from .__typing import ConfigLoader, ConfigParameterCallback, TyperParameterValue
 from .loaders import (
     dotenv_loader,
     json_loader,
```

### Comparing `typer_config-0.5.0/typer_config/__typing.py` & `typer_config-0.6.0/typer_config/__typing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Data and Function types.
 """
 
 import sys
-from typing import Any, Callable, Dict, Iterable
+from pathlib import Path
+from typing import Any, Callable, Dict, Iterable, Union
 
 from typer import CallbackParam, Context
 
 # Handle some imports based on python version
 if sys.version_info < (3, 10):  # pragma: no cover
     from typing_extensions import TypeAlias
 else:  # pragma: no cover
@@ -22,14 +23,17 @@
 
 ConfigDict: TypeAlias = Dict[TyperParameterName, Any]
 """Configuration dictionary to be applied to the click context default map."""
 
 ConfigDictAccessorPath: TypeAlias = Iterable[str]
 """Configuration dictionary accessor path."""
 
+FilePath: TypeAlias = Union[Path, str]
+"""File path"""
+
 # Function types
 TyperParameterValueTransformer: TypeAlias = Callable[
     [TyperParameterValue], TyperParameterValue
 ]
 """Typer parameter value transforming function."""
 
 ConfigDictTransformer: TypeAlias = Callable[[ConfigDict], ConfigDict]
@@ -44,7 +48,16 @@
 ConfigParameterCallback: TypeAlias = Callable[
     [Context, CallbackParam, TyperParameterValue], TyperParameterValue
 ]
 """Typer config parameter callback function."""
 
 NoArgCallable: TypeAlias = Callable[[], Any]
 """No argument callable."""
+
+ConfigDumper: TypeAlias = Callable[[ConfigDict, FilePath], None]
+"""Configuration dumper function."""
+
+TyperCommand: TypeAlias = Callable[..., Any]
+"""A function that will be decorated with `typer.Typer().command()`."""
+
+TyperCommandDecorator: TypeAlias = Callable[[TyperCommand], TyperCommand]
+"""A decorator applied to a typer command."""
```

### Comparing `typer_config-0.5.0/typer_config/loaders.py` & `typer_config-0.6.0/typer_config/loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,29 @@
 """
 Configuration File Loaders.
 
 These loaders must implement the `typer_config.__typing.ConfigLoader` interface.
 """
 import json
-import sys
 from configparser import ConfigParser
 from typing import Optional
 from warnings import warn
 
+from .__optional_imports import *  # pylint: disable=wildcard-import, unused-wildcard-import
 from .__typing import (
     ConfigDict,
     ConfigDictAccessorPath,
     ConfigDictTransformer,
     ConfigLoader,
     ConfigLoaderConditional,
     NoArgCallable,
     TyperParameterValue,
     TyperParameterValueTransformer,
 )
 
-USING_TOMLLIB = False
-TOML_MISSING = True
-YAML_MISSING = True
-DOTENV_MISSING = True
-
-
-if sys.version_info >= (3, 11):  # pragma: no cover
-    import tomllib  # type: ignore
-
-    TOML_MISSING = False
-    USING_TOMLLIB = True
-else:  # pragma: no cover
-    try:
-        # Third-party toml parsing library
-        import toml
-
-        TOML_MISSING = False
-
-    except ImportError:
-        pass
-
-
-try:  # pragma: no cover
-    import yaml
-
-    YAML_MISSING = False
-except ImportError:  # pragma: no cover
-    pass
-
-try:  # pragma: no cover
-    import dotenv
-
-    DOTENV_MISSING = False
-except ImportError:  # pragma: no cover
-    pass
-
 
 def loader_transformer(
     loader: ConfigLoader,
     loader_conditional: Optional[ConfigLoaderConditional] = None,
     param_transformer: Optional[TyperParameterValueTransformer] = None,
     config_transformer: Optional[ConfigDictTransformer] = None,
 ) -> ConfigLoader:
@@ -92,15 +56,15 @@
             param_transformer = lambda param: param if param else "pyproject.toml"
             config_transformer = lambda config: config["tool"]["my_tool"],
         )
         ```
 
     Args:
         loader (ConfigLoader): Loader to transform.
-        loader_condtional (Optional[ConfigLoaderConditional], optional): Function
+        loader_conditional (Optional[ConfigLoaderConditional], optional): Function
             to determine whether to execute loader. Defaults to None (no-op).
         param_transformer (Optional[TyperParameterValueTransformer], optional): Typer
             parameter transformer. Defaults to None (no-op).
         config_transformer (Optional[ConfigDictTransformer], optional): Config
             dictionary transformer. Defaults to None (no-op).
 
     Returns:
@@ -270,27 +234,22 @@
     Raises:
         ModuleNotFoundError: toml library is not installed
 
     Returns:
         ConfigDict: dictionary loaded from file
     """
 
-    if TOML_MISSING:  # pragma: no cover
-        raise ModuleNotFoundError("Please install the toml library.")
-
-    conf: ConfigDict = {}
-
     if USING_TOMLLIB:  # pragma: no cover
         with open(param_value, "rb") as _file:
-            conf = tomllib.load(_file)  # type: ignore
-    else:  # pragma: no cover
-        with open(param_value, "r", encoding="utf-8") as _file:
-            conf = toml.load(_file)  # type: ignore
+            return tomllib.load(_file)  # type: ignore
 
-    return conf
+    if TOML_MISSING:  # pragma: no cover
+        raise ModuleNotFoundError("Please install the toml library.")
+    with open(param_value, "r", encoding="utf-8") as _file:  # pragma: no cover
+        return toml.load(_file)  # type: ignore
 
 
 def dotenv_loader(param_value: TyperParameterValue) -> ConfigDict:
     """Dotenv file loader.
 
     Args:
         param_value (TyperParameterValue): path of Dotenv file
```

### Comparing `typer_config-0.5.0/PKG-INFO` & `typer_config-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-config
-Version: 0.5.0
+Version: 0.6.0
 Summary: Utilities for working with configuration files in typer CLIs. 
 Home-page: https://maxb2.github.io/typer-config/
 License: MIT
 Keywords: typer,config,configuration,configuration-file,yaml,toml,json,dotenv,cli
 Author: Matt Anderson
 Author-email: matt@manderscience.com
 Requires-Python: >=3.8,<4.0
@@ -64,8 +64,33 @@
 # Long commands like this:
 $ my-typer-app --opt1 foo --opt2 bar arg1 arg2
 
 # Can become this:
 $ my-typer-app --config config.yml
 ```
 
+## Quickstart
+
+You can use a decorator to quickly add a configuration parameter to your `typer` application:
+
+```py
+import typer
+from typer_config import use_yaml_config
+
+app = typer.Typer()
+
+
+@app.command()
+@use_yaml_config() # MUST BE AFTER @app.command()
+def main(...):
+    ...
+
+if __name__ == "__main__":
+    app()
+```
+
+Your typer command will now include a `--config CONFIG_FILE` option at the command line.
+
+> **Note**: this package also provides `@use_json_config`, `@use_toml_config`, and `@use_dotenv_config` for those file formats.
+> You can also use your own loader function and the `@use_config(loader_func)` decorator.
+
 See the [documentation](https://maxb2.github.io/typer-config/latest/examples/simple_yaml/) for more examples using typer-config.
```

