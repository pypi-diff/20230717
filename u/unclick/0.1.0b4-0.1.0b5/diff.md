# Comparing `tmp/unclick-0.1.0b4.tar.gz` & `tmp/unclick-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unclick-0.1.0b4.tar", max compression
+gzip compressed data, was "unclick-0.1.0b5.tar", max compression
```

## Comparing `unclick-0.1.0b4.tar` & `unclick-0.1.0b5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1504 2023-03-11 04:32:10.020730 unclick-0.1.0b4/LICENSE.md
--rw-r--r--   0        0        0      518 2023-03-11 04:32:10.021176 unclick-0.1.0b4/README.md
--rw-r--r--   0        0        0     1307 2023-03-11 04:32:10.022533 unclick-0.1.0b4/pyproject.toml
--rw-r--r--   0        0        0      241 2023-03-11 04:32:10.023016 unclick-0.1.0b4/src/unclick/__init__.py
--rw-r--r--   0        0        0    11554 2023-03-11 04:32:10.023387 unclick-0.1.0b4/src/unclick/core.py
--rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 unclick-0.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-17 06:03:01.374597 unclick-0.1.0b5/LICENSE.md
+-rw-r--r--   0        0        0      518 2023-07-17 06:03:01.375064 unclick-0.1.0b5/README.md
+-rw-r--r--   0        0        0     1307 2023-07-17 06:03:01.376440 unclick-0.1.0b5/pyproject.toml
+-rw-r--r--   0        0        0      241 2023-07-17 06:03:01.376936 unclick-0.1.0b5/src/unclick/__init__.py
+-rw-r--r--   0        0        0    11782 2023-07-17 06:03:01.377315 unclick-0.1.0b5/src/unclick/core.py
+-rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 unclick-0.1.0b5/PKG-INFO
```

### Comparing `unclick-0.1.0b4/LICENSE.md` & `unclick-0.1.0b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unclick-0.1.0b4/README.md` & `unclick-0.1.0b5/README.md`

 * *Files identical despite different names*

### Comparing `unclick-0.1.0b4/pyproject.toml` & `unclick-0.1.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unclick"
-version = "0.1.0b4"
+version = "0.1.0b5"
 description = "A reverse parser for the click CLI library"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD 3-clause"
 readme = "README.md"
 packages = [
     { include = "unclick", from = "src" }
 ]
```

### Comparing `unclick-0.1.0b4/src/unclick/core.py` & `unclick-0.1.0b5/src/unclick/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,19 @@
             raise ValueError(f"Value for parameter {name!r} must have len {param_len}.")
         for ii, vv in enumerate(value):
             vv_info = param_info.copy()
             vv_info["nargs"] = 1
             vv_info["type"] = param_info["type"]["types"][ii]
             _check_type(vv, vv_info)
         return
+    elif param_type == "choice":
+        choices = param_info["type"]["choices"]
+        if value not in choices:
+            raise ValueError(f"Value {value} is not one the allowed choices {choices}.")
+        return
     else:
         raise TypeError(f"click type {param_type} not supported.")
 
     test_values = [value] if not isinstance(value, (tuple, list)) else value
 
     if nargs != -1 and len(test_values) != nargs:
         raise ValueError(f"Invalid number of arguments for parameter {name!r}.")
@@ -126,15 +131,15 @@
     if value is None:
         if is_argument:
             raise ValueError(f"'None' cannot be used as value for argument {name!r}.")
         return ""
 
     value_str: str
 
-    if param_type in ["string", "int", "float"]:
+    if param_type in ["string", "int", "float", "choice"]:
         # For cases when the flag is not boolean.
         if param_info.get("is_flag", False):
             if isinstance(value, str):
                 if value == param_info["flag_value"]:
                     return opts[0]
             elif isinstance(value, bool):
                 if value != param_info["default"]:
```

### Comparing `unclick-0.1.0b4/PKG-INFO` & `unclick-0.1.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unclick
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: A reverse parser for the click CLI library
 License: BSD 3-clause
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

