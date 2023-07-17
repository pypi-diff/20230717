# Comparing `tmp/auto_click_auto-0.1.0a1.tar.gz` & `tmp/auto_click_auto-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_click_auto-0.1.0a1.tar", max compression
+gzip compressed data, was "auto_click_auto-0.1.0a2.tar", max compression
```

## Comparing `auto_click_auto-0.1.0a1.tar` & `auto_click_auto-0.1.0a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-07-17 17:33:57.779256 auto_click_auto-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     5174 2023-07-17 17:33:57.779256 auto_click_auto-0.1.0a1/README.md
--rw-r--r--   0        0        0       99 2023-07-17 17:33:57.779256 auto_click_auto-0.1.0a1/auto_click_auto/__init__.py
--rw-r--r--   0        0        0      532 2023-07-17 17:33:57.779256 auto_click_auto-0.1.0a1/auto_click_auto/constants.py
--rw-r--r--   0        0        0     5264 2023-07-17 17:33:57.779256 auto_click_auto-0.1.0a1/auto_click_auto/core.py
--rw-r--r--   0        0        0      460 2023-07-17 17:33:57.779256 auto_click_auto-0.1.0a1/auto_click_auto/exceptions.py
--rw-r--r--   0        0        0     2823 2023-07-17 17:33:57.779256 auto_click_auto-0.1.0a1/auto_click_auto/utils.py
--rw-r--r--   0        0        0     1476 2023-07-17 17:33:57.783256 auto_click_auto-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     6475 1970-01-01 00:00:00.000000 auto_click_auto-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     5252 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/README.md
+-rw-r--r--   0        0        0       99 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/auto_click_auto/__init__.py
+-rw-r--r--   0        0        0      532 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/auto_click_auto/constants.py
+-rw-r--r--   0        0        0     5271 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/auto_click_auto/core.py
+-rw-r--r--   0        0        0      460 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/auto_click_auto/exceptions.py
+-rw-r--r--   0        0        0     2823 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/auto_click_auto/utils.py
+-rw-r--r--   0        0        0     1476 2023-07-17 19:49:12.934242 auto_click_auto-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     6553 1970-01-01 00:00:00.000000 auto_click_auto-0.1.0a2/PKG-INFO
```

### Comparing `auto_click_auto-0.1.0a1/LICENSE` & `auto_click_auto-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a1/README.md` & `auto_click_auto-0.1.0a2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -135,10 +135,13 @@
 In summary, `auto-click-auto`:
 - Has one specific purpose, it "automatically" enables shell completion for Click programs
 - Does not have any 3rd party dependencies, besides Click
 - Provides an option for seamless enabling of the shell completion
 - Comes ready with ways to add shell completion as a command option or subcommand
 - Has simple examples of how to quickly use the library
 
+## Changelog
+https://github.com/KAUTH/auto-click-auto/blob/main/CHANGELOG.md
+
 ## Contributing
 You can always submit a PR if you want to suggest improvements or fix issues.
 Check out the open issues at https://github.com/KAUTH/auto-click-auto/issues.
```

### Comparing `auto_click_auto-0.1.0a1/auto_click_auto/constants.py` & `auto_click_auto-0.1.0a2/auto_click_auto/constants.py`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a1/auto_click_auto/core.py` & `auto_click_auto-0.1.0a2/auto_click_auto/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 _AnyCallable = Callable[..., Any]
 _Decorator: "te.TypeAlias" = Callable[[T], T]
 FC = TypeVar("FC", bound=Union[_AnyCallable, Command])
 
 
 def enable_click_shell_completion(
     program_name: str,
-    shells: Optional[Set[ShellType]],
+    shells: Optional[Set[ShellType]] = None,
     verbose: Optional[bool] = False,
 ) -> None:
     """
     Enable tab completion for Click's supported shell types.
 
     If ``shells`` is not provided, `auto-click-auto` will attempt to detect the
     shell type the user is currently running the program on.
```

### Comparing `auto_click_auto-0.1.0a1/auto_click_auto/utils.py` & `auto_click_auto-0.1.0a2/auto_click_auto/utils.py`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a1/pyproject.toml` & `auto_click_auto-0.1.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-click-auto"
-version = "0.1.0-alpha.1"
+version = "0.1.0-alpha.2"
 description = "Automatically enable tab autocompletion for shells in Click CLI applications."
 authors = ["Konstantinos Papadopoulos <konpap1996@yahoo.com>"]
 maintainers = ["Konstantinos Papadopoulos <konpap1996@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/KAUTH/auto-click-auto"
 repository = "https://github.com/KAUTH/auto-click-auto"
```

### Comparing `auto_click_auto-0.1.0a1/PKG-INFO` & `auto_click_auto-0.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-click-auto
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Automatically enable tab autocompletion for shells in Click CLI applications.
 Home-page: https://github.com/KAUTH/auto-click-auto
 License: MIT
 Keywords: click,autocomplete,shell
 Author: Konstantinos Papadopoulos
 Author-email: konpap1996@yahoo.com
 Maintainer: Konstantinos Papadopoulos
@@ -165,11 +165,14 @@
 In summary, `auto-click-auto`:
 - Has one specific purpose, it "automatically" enables shell completion for Click programs
 - Does not have any 3rd party dependencies, besides Click
 - Provides an option for seamless enabling of the shell completion
 - Comes ready with ways to add shell completion as a command option or subcommand
 - Has simple examples of how to quickly use the library
 
+## Changelog
+https://github.com/KAUTH/auto-click-auto/blob/main/CHANGELOG.md
+
 ## Contributing
 You can always submit a PR if you want to suggest improvements or fix issues.
 Check out the open issues at https://github.com/KAUTH/auto-click-auto/issues.
```

