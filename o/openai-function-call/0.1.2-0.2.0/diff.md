# Comparing `tmp/openai_function_call-0.1.2.tar.gz` & `tmp/openai_function_call-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_call-0.1.2.tar", max compression
+gzip compressed data, was "openai_function_call-0.2.0.tar", max compression
```

## Comparing `openai_function_call-0.1.2.tar` & `openai_function_call-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-07-17 09:19:43.513220 openai_function_call-0.1.2/LICENSE
--rw-r--r--   0        0        0     8394 2023-07-17 09:19:43.513220 openai_function_call-0.1.2/README.md
--rw-r--r--   0        0        0      187 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/__init__.py
--rw-r--r--   0        0        0      151 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/__init__.py
--rw-r--r--   0        0        0     5799 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/completion.py
--rw-r--r--   0        0        0      505 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/messages/__init__.py
--rw-r--r--   0        0        0     1669 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/messages/base.py
--rw-r--r--   0        0        0     3260 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/messages/messages.py
--rw-r--r--   0        0        0     1486 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/messages/user.py
--rw-r--r--   0        0        0     2210 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/dsl/multitask.py
--rw-r--r--   0        0        0     6351 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/openai_function_call/function_calls.py
--rw-r--r--   0        0        0      663 2023-07-17 09:19:43.521220 openai_function_call-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9128 1970-01-01 00:00:00.000000 openai_function_call-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-17 13:01:37.119032 openai_function_call-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8394 2023-07-17 13:01:37.119032 openai_function_call-0.2.0/README.md
+-rw-r--r--   0        0        0      187 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/__init__.py
+-rw-r--r--   0        0        0      151 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/__init__.py
+-rw-r--r--   0        0        0     5799 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/completion.py
+-rw-r--r--   0        0        0      505 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/messages/__init__.py
+-rw-r--r--   0        0        0     1669 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/messages/base.py
+-rw-r--r--   0        0        0     3260 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/messages/messages.py
+-rw-r--r--   0        0        0     1486 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/messages/user.py
+-rw-r--r--   0        0        0     2210 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/multitask.py
+-rw-r--r--   0        0        0     6330 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/function_calls.py
+-rw-r--r--   0        0        0      662 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9127 1970-01-01 00:00:00.000000 openai_function_call-0.2.0/PKG-INFO
```

### Comparing `openai_function_call-0.1.2/LICENSE` & `openai_function_call-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.2/README.md` & `openai_function_call-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.2/openai_function_call/dsl/completion.py` & `openai_function_call-0.2.0/openai_function_call/dsl/completion.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.2/openai_function_call/dsl/messages/base.py` & `openai_function_call-0.2.0/openai_function_call/dsl/messages/base.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.2/openai_function_call/dsl/messages/messages.py` & `openai_function_call-0.2.0/openai_function_call/dsl/messages/messages.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.2/openai_function_call/dsl/messages/user.py` & `openai_function_call-0.2.0/openai_function_call/dsl/messages/user.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.2/openai_function_call/dsl/multitask.py` & `openai_function_call-0.2.0/openai_function_call/dsl/multitask.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.1.2/openai_function_call/function_calls.py` & `openai_function_call-0.2.0/openai_function_call/function_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import json
 from functools import wraps
-from typing import Any, Callable, Optional, List, Type
-from pydantic import validate_arguments, BaseModel, create_model, Field
+from typing import Any, Callable
+from pydantic import BaseModel, validate_arguments
 
 
 def _remove_a_key(d, remove_key) -> None:
     """Remove a key from a dictionary recursively"""
     if isinstance(d, dict):
         for key in list(d.keys()):
             if key == remove_key:
@@ -61,15 +61,15 @@
         # 2
         ```
     """
 
     def __init__(self, func: Callable) -> None:
         self.func = func
         self.validate_func = validate_arguments(func)
-        parameters = self.validate_func.model.schema()
+        parameters = self.validate_func.model.model_json_schema()
         parameters["properties"] = {
             k: v
             for k, v in parameters["properties"].items()
             if k not in ("v__duplicate_kwargs", "args", "kwargs")
         }
         parameters["required"] = sorted(
             parameters["properties"]
@@ -123,15 +123,15 @@
 
         Note:
             Its important to add a docstring to describe how to best use this class, it will be included in the description attribute and be part of the prompt.
 
         Returns:
             model_json_schema (dict): A dictionary in the format of OpenAI's schema as jsonschema
         """
-        schema = cls.schema()
+        schema = cls.model_json_schema()
         parameters = {
             k: v for k, v in schema.items() if k not in ("title", "description")
         }
         parameters["required"] = sorted(parameters["properties"])
         _remove_a_key(parameters, "title")
 
         if "description" not in schema:
```

### Comparing `openai_function_call-0.1.2/pyproject.toml` & `openai_function_call-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "openai-function-call"
-version = "0.1.2"
+version = "0.2.0"
 description = "Helper functions that allow us to improve openai's function_call ergonomics"
 authors = ["Jason <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "openai_function_call"}]
 repository = "https://github.com/jxnl/openai_function_call"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^0.27.8"
-pydantic = "^1.10.9"
+pydantic = "^2.0.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.18"
 mkdocstrings = "^0.22.0"
```

### Comparing `openai_function_call-0.1.2/PKG-INFO` & `openai_function_call-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openai-function-call
-Version: 0.1.2
+Version: 0.2.0
 Summary: Helper functions that allow us to improve openai's function_call ergonomics
 Home-page: https://github.com/jxnl/openai_function_call
 License: MIT
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Project-URL: Repository, https://github.com/jxnl/openai_function_call
 Description-Content-Type: text/markdown
 
 # Pydantic is all you need, for openai function calls.
 
 Check out the [docs](https://openai-function-call.onrender.com/)!
```

