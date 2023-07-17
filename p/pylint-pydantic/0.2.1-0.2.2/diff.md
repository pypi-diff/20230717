# Comparing `tmp/pylint_pydantic-0.2.1-py3-none-any.whl.zip` & `tmp/pylint_pydantic-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14930 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1876 b- defN 23-Jul-12 01:41 pylint_pydantic/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-12 01:41 pylint_pydantic-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1869 b- defN 23-Jul-12 01:41 pylint_pydantic-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 01:41 pylint_pydantic-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-12 01:41 pylint_pydantic-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      511 b- defN 23-Jul-12 01:41 pylint_pydantic-0.2.1.dist-info/RECORD
-6 files, 39513 bytes uncompressed, 14000 bytes compressed:  64.6%
+Zip file size: 15126 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     2469 b- defN 23-Jul-17 09:52 pylint_pydantic/__init__.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-17 09:53 pylint_pydantic-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1931 b- defN 23-Jul-17 09:53 pylint_pydantic-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 09:53 pylint_pydantic-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-17 09:53 pylint_pydantic-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      511 b- defN 23-Jul-17 09:53 pylint_pydantic-0.2.2.dist-info/RECORD
+6 files, 40168 bytes uncompressed, 14196 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pylint_pydantic/__init__.py
 Comment: 
 
-Filename: pylint_pydantic-0.2.1.dist-info/LICENSE
+Filename: pylint_pydantic-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: pylint_pydantic-0.2.1.dist-info/METADATA
+Filename: pylint_pydantic-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: pylint_pydantic-0.2.1.dist-info/WHEEL
+Filename: pylint_pydantic-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: pylint_pydantic-0.2.1.dist-info/top_level.txt
+Filename: pylint_pydantic-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pylint_pydantic-0.2.1.dist-info/RECORD
+Filename: pylint_pydantic-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylint_pydantic/__init__.py

```diff
@@ -1,39 +1,60 @@
 import astroid
-from astroid import (MANAGER, Attribute, Call, ClassDef, FunctionDef, Name, nodes)
+from astroid import MANAGER, Attribute, Call, ClassDef, FunctionDef, Name, nodes
 from pylint.checkers.design_analysis import MisdesignChecker
 from pylint_plugin_utils import suppress_message
 
-VALIDATOR_METHOD_NAMES = {"validator", "root_validator", "field_validator", "model_validator"}
+CLASSMETHOD_VALIDATOR_NAMES = {"validator", "root_validator", "field_validator"}
+MODE_VALIDATOR_NAMES = {"model_validator"}
 
 
-def is_validator_method(node: FunctionDef):
+def _mode_validator_is_classmethod(call: Call):
+    # https://docs.pydantic.dev/latest/api/functional_validators/#pydantic.functional_validators.model_validator
+    for keyword in call.keywords:
+        if keyword.arg == "mode" and "after" in keyword.value.as_string():
+            return False
+    return True
+
+
+# def _get_decorator_name(decorator: Name | Attribute):
+def _get_decorator_name(decorator):
+
+    # @validator(pre=True)
+    if isinstance(decorator, Call):
+        decorator = decorator.func
+
+    # @validator
+    if isinstance(decorator, Name):
+        return decorator.name
+
+    # @pydantic.validator
+    if isinstance(decorator, Attribute):
+        return decorator.attrname
+
+    raise ValueError("Invalid decorator name")
+
+
+def _is_classmethod_decorator(node: FunctionDef):
 
     if not node.decorators:
         return False
 
     for decorator in node.decorators.get_children():
-        # @validator(pre=True)
-        if isinstance(decorator, Call):
-            # transform to @validator case
-            decorator = decorator.func
-
-        # @validator
-        if (isinstance(decorator, Name) and decorator.name in VALIDATOR_METHOD_NAMES):
+        decorator_name = _get_decorator_name(decorator)
+        if decorator_name in CLASSMETHOD_VALIDATOR_NAMES:
             return True
 
-        # @pydantic.validator
-        if (isinstance(decorator, Attribute) and decorator.attrname in VALIDATOR_METHOD_NAMES):
-            return True
+        if decorator_name in MODE_VALIDATOR_NAMES:
+            return _mode_validator_is_classmethod(decorator)
 
     return False
 
 
 def transform(node: FunctionDef):
-    if is_validator_method(node):
+    if _is_classmethod_decorator(node):
         node.type = "classmethod"
 
 
 def is_pydantic_config_class(node: ClassDef):
     if node.name == "Config" \
         and isinstance(node.parent, ClassDef) \
             and node.parent.is_subtype_of("pydantic.main.BaseModel"):
```

## Comparing `pylint_pydantic-0.2.1.dist-info/LICENSE` & `pylint_pydantic-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pylint_pydantic-0.2.1.dist-info/METADATA` & `pylint_pydantic-0.2.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-pydantic
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Pylint plugin to help Pylint understand the Pydantic
 Home-page: https://github.com/fcfangcc/pylint-pydantic
 Author: fcfangcc
 Author-email: swjfc22@163.com
 License: GPLv3
 Keywords: pylint,pydantic
 Platform: UNKNOWN
@@ -65,9 +65,9 @@
 https://github.com/fcfangcc/pylint-pydantic/issues
 
 
 Changelog
 =====================
 - v0.2.0: support Pydantic V2
 - v0.2.1: support `model_validator`
-
+- v0.2.2: fix model_validator keyword **mode**, pydatic>=2.0.3
```

