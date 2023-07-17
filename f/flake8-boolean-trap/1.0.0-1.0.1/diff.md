# Comparing `tmp/flake8_boolean_trap-1.0.0.tar.gz` & `tmp/flake8_boolean_trap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_boolean_trap-1.0.0.tar", max compression
+gzip compressed data, was "flake8_boolean_trap-1.0.1.tar", max compression
```

## Comparing `flake8_boolean_trap-1.0.0.tar` & `flake8_boolean_trap-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      622 2023-02-13 16:27:38.940830 flake8_boolean_trap-1.0.0/README.md
--rw-r--r--   0        0        0     2648 2023-02-13 16:27:38.940830 flake8_boolean_trap-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7274 2023-02-13 16:27:38.940830 flake8_boolean_trap-1.0.0/src/flake8_boolean_trap.py
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 flake8_boolean_trap-1.0.0/setup.py
--rw-r--r--   0        0        0     1920 1970-01-01 00:00:00.000000 flake8_boolean_trap-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1110 2023-07-17 17:00:45.899197 flake8_boolean_trap-1.0.1/README.md
+-rw-r--r--   0        0        0     2648 2023-07-17 17:00:45.899197 flake8_boolean_trap-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7912 2023-07-17 17:00:45.899197 flake8_boolean_trap-1.0.1/src/flake8_boolean_trap.py
+-rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 flake8_boolean_trap-1.0.1/PKG-INFO
```

### Comparing `flake8_boolean_trap-1.0.0/pyproject.toml` & `flake8_boolean_trap-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8_boolean_trap"
-version = "1.0.0"
+version = "1.0.1"
 description = "flake8 plugin which forbids boolean positional arguments"
 authors = ["Pablo Woolvett <github@devx.pw>"]
 packages = [
     { include = "flake8_boolean_trap.py", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://pwoolvett.github.io/flake8_boolean_trap"
@@ -78,15 +78,15 @@
   "D202",  # black conflict
   "W503",  # black conflict, looks ok
 ]
 max_line_length = 88
 
 
 [tool.commitizen]
-version = "1.0.0"
+version = "1.0.1"
 annotated_tag = true
 update_changelog_on_bump = true
 name = "cz_conventional_commits"
 tag_format = "$version"
 # keep this in sync with the bump workflow to avoid
 # re-triggering it after commitizen bump command pushes
 bump_message = "bump: $current_version → $new_version"
```

### Comparing `flake8_boolean_trap-1.0.0/src/flake8_boolean_trap.py` & `flake8_boolean_trap-1.0.1/src/flake8_boolean_trap.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 BooleanTrapRegistry = List[Tuple[int, int, Union[str, int], str, BooleanTrapReason]]
 CandidateGen = Generator[Tuple[ast.expr, int, int, str], None, None]
 LintError = Tuple[int, int, str, Type[Any]]
 LintErrorGen = Generator[LintError, None, None]
 
 
 def positional_hints(func_node: ast.FunctionDef) -> CandidateGen:
-    """Extract type hints from postiional arguments.
+    """Extract type hints from positional arguments.
 
     Args:
         func_node: Function ast containing the arguments to search.
 
     Yields:
         Type annotations for arguments which could be used as positional.
     """
@@ -113,14 +113,32 @@
     """
 
     arg_defaults = zip(reversed(func_node.args.args), reversed(func_node.args.defaults))
     for arg, default in arg_defaults:
         yield default, default.lineno, default.col_offset, arg.arg
 
 
+def is_property_setter(func_node: ast.FunctionDef) -> bool:
+    """Detect whether a function node is a property setter.
+
+    Args:
+        func_node: The functions ast to check its decorations. If any is
+            a property setter, returns `True`. Otherwise, returns `False`.
+
+    Returns:
+        True if the function corresponds to a property setter.
+    """
+    for decorator in func_node.decorator_list:
+        if not isinstance(decorator, ast.Attribute):
+            continue
+        if decorator.attr == "setter":
+            return True
+    return False
+
+
 def is_boolean_default(default: ast.expr) -> bool:
     """Detect whether a default argument value is a boolean.
 
     Args:
         default: Default parameter value ast.
 
     Returns:
@@ -149,14 +167,16 @@
 
         See Also
             * `BooleanTrapReason.TYPE_HINT`: `positional_hints`, `is_boolean_typehint`
             * `BooleanTrapReason.DEFAULT_VALUE`: `default_values`, `is_boolean_default`
 
         """
         for hint, lineno, col, argname in positional_hints(func_node):
+            if is_property_setter(func_node):
+                continue
             if is_boolean_typehint(hint):
                 self.registry.append(
                     (lineno, col, argname, func_node.name, BooleanTrapReason.TYPE_HINT)
                 )
 
         for default, lineno, col, argname in default_values(func_node):
             if is_boolean_default(default):
```

