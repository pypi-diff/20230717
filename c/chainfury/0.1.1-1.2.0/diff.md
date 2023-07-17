# Comparing `tmp/chainfury-0.1.1.tar.gz` & `tmp/chainfury-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainfury-0.1.1.tar", max compression
+gzip compressed data, was "chainfury-1.2.0.tar", max compression
```

## Comparing `chainfury-0.1.1.tar` & `chainfury-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0    11351 2023-06-12 10:47:25.719426 chainfury-0.1.1/LICENSE
--rw-r--r--   0        0        0     7783 2023-06-12 10:47:25.719584 chainfury-0.1.1/README.md
--rw-r--r--   0        0        0      256 2023-06-19 19:54:10.712240 chainfury-0.1.1/chainfury/__init__.py
--rw-r--r--   0        0        0    12524 2023-06-19 10:21:46.091911 chainfury-0.1.1/chainfury/agent.py
--rw-r--r--   0        0        0    30518 2023-06-19 10:28:45.737597 chainfury-0.1.1/chainfury/base.py
--rw-r--r--   0        0        0      996 2023-06-19 19:50:21.074486 chainfury-0.1.1/chainfury/cli.py
--rw-r--r--   0        0        0     6035 2023-06-19 19:50:32.084245 chainfury-0.1.1/chainfury/client.py
--rw-r--r--   0        0        0     1699 2023-06-12 14:13:15.392725 chainfury-0.1.1/chainfury/components/README.md
--rw-r--r--   0        0        0      795 2023-06-19 19:58:00.971782 chainfury-0.1.1/chainfury/components/__init__.py
--rw-r--r--   0        0        0     4187 2023-06-19 10:28:49.030833 chainfury-0.1.1/chainfury/components/ai_actions/__init__.py
--rw-r--r--   0        0        0     2003 2023-06-19 10:28:44.950061 chainfury-0.1.1/chainfury/components/functional/__init__.py
--rw-r--r--   0        0        0     2237 2023-06-19 10:28:44.907614 chainfury-0.1.1/chainfury/components/nbx/__init__.py
--rw-r--r--   0        0        0     8981 2023-06-19 10:28:44.986884 chainfury-0.1.1/chainfury/components/openai/__init__.py
--rw-r--r--   0        0        0       78 2023-06-19 19:54:19.450567 chainfury-0.1.1/chainfury/components/redis/__init__.py
--rw-r--r--   0        0        0     9400 2023-06-19 10:28:44.949439 chainfury-0.1.1/chainfury/components/stability/__init__.py
--rw-r--r--   0        0        0     1262 2023-06-19 19:53:04.579434 chainfury-0.1.1/chainfury/utils.py
--rw-r--r--   0        0        0      113 2023-06-19 19:59:21.715065 chainfury-0.1.1/chainfury/version.py
--rw-r--r--   0        0        0      628 2023-06-19 19:59:57.165966 chainfury-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9106 1970-01-01 00:00:00.000000 chainfury-0.1.1/setup.py
--rw-r--r--   0        0        0     8631 1970-01-01 00:00:00.000000 chainfury-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-06-12 10:47:25.719426 chainfury-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8030 2023-06-26 17:41:18.027685 chainfury-1.2.0/README.md
+-rw-r--r--   0        0        0      297 2023-06-26 17:41:18.082832 chainfury-1.2.0/chainfury/__init__.py
+-rw-r--r--   0        0        0    19865 2023-07-17 10:21:32.408643 chainfury-1.2.0/chainfury/agent.py
+-rw-r--r--   0        0        0    46008 2023-07-16 11:49:08.560482 chainfury-1.2.0/chainfury/base.py
+-rw-r--r--   0        0        0      766 2023-07-17 09:33:13.149326 chainfury-1.2.0/chainfury/cli.py
+-rw-r--r--   0        0        0    13266 2023-07-04 11:02:16.679972 chainfury-1.2.0/chainfury/client.py
+-rw-r--r--   0        0        0     1699 2023-06-26 07:50:14.048396 chainfury-1.2.0/chainfury/components/README.md
+-rw-r--r--   0        0        0      864 2023-07-03 11:39:00.427129 chainfury-1.2.0/chainfury/components/__init__.py
+-rw-r--r--   0        0        0     1146 2023-06-26 07:50:14.048972 chainfury-1.2.0/chainfury/components/ai_actions/__init__.py
+-rw-r--r--   0        0        0      836 2023-07-04 04:54:19.835188 chainfury-1.2.0/chainfury/components/const.py
+-rw-r--r--   0        0        0     6808 2023-07-16 11:53:54.430158 chainfury-1.2.0/chainfury/components/functional/__init__.py
+-rw-r--r--   0        0        0     4603 2023-07-05 13:25:46.908873 chainfury-1.2.0/chainfury/components/nbx/__init__.py
+-rw-r--r--   0        0        0    10036 2023-07-07 20:05:42.618404 chainfury-1.2.0/chainfury/components/openai/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-26 07:50:14.049729 chainfury-1.2.0/chainfury/components/redis/__init__.py
+-rw-r--r--   0        0        0     8659 2023-07-16 12:39:23.305115 chainfury-1.2.0/chainfury/components/serper/__init__.py
+-rw-r--r--   0        0        0     9904 2023-07-03 13:14:41.480424 chainfury-1.2.0/chainfury/components/stability/__init__.py
+-rw-r--r--   0        0        0     1013 2023-07-04 09:56:27.058762 chainfury-1.2.0/chainfury/types.py
+-rw-r--r--   0        0        0     2616 2023-07-03 15:18:38.323479 chainfury-1.2.0/chainfury/utils.py
+-rw-r--r--   0        0        0      135 2023-07-17 10:29:18.555431 chainfury-1.2.0/chainfury/version.py
+-rw-r--r--   0        0        0      698 2023-07-17 10:29:27.765087 chainfury-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9495 1970-01-01 00:00:00.000000 chainfury-1.2.0/setup.py
+-rw-r--r--   0        0        0     8962 1970-01-01 00:00:00.000000 chainfury-1.2.0/PKG-INFO
```

### Comparing `chainfury-0.1.1/LICENSE` & `chainfury-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainfury-0.1.1/README.md` & `chainfury-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 <img src="./docs/1.png" align="center"/>
 
 🦋 Build complex chat apps using LLMs in 4 clicks ⚡️ [Try it out here](https://chainfury.nbox.ai/)
 
 ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs. 
 
+[ChainFury- Create LLM ChatBots in 4 clicks!](https://medium.com/@chandranih/chainfury-create-llm-chatbots-in-4-clicks-3663538db8c6)
+
+[Why the Fury? Building a new flow engine from scratch](https://blog.nimblebox.ai/new-flow-engine-from-scratch)
+
 With a simple GUI inspired by [LangFlow](https://github.com/logspace-ai/langflow), ChainFury enables you to chain components of [LangChain](https://github.com/hwchase17/langchain) together, allowing you to embed more complex chat applications with a simple JS snippet.
 
 ChainFury supports a range of features, including but not limited to:
 
 - Recording all prompts and responses and storing them in a database
 - Collecting metrics like response latency
 - Querying OpenAI's API to obtain a rating for the response, which it stores in the database
@@ -59,20 +63,20 @@
 <details>
 <summary>For this, you will need to build the frontend and and then run the backend. The frontend can be built using the following command:</summary>
 
 ```bash
 cd client
 yarn install
 yarn build
+cd ..
 ```
 
 To copy the frontend to the backend, run the following command:
 
 ```bash
-cd ..
 cp -r client/dist/ server/static/
 mkdir -p ./server/templates
 cp ./client/dist/index.html ./server/templates/index.html
 ```
 
 Now you can install the backend dependencies and run the server. We recommend using Python 3.9 virtual environment for this:
```

### Comparing `chainfury-0.1.1/chainfury/base.py` & `chainfury-1.2.0/chainfury/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,29 @@
-import os
 import copy
 import json
 import inspect
-import logging
 import datetime
 import traceback
 from pprint import pformat
-from hashlib import sha256
-from typing import Any, Union, Optional, Dict, List, Tuple, Callable
+from typing import Any, Union, Optional, Dict, List, Tuple, Callable, Generator
 from collections import deque, defaultdict
 
 import jinja2schema
 from jinja2schema import model as j2sm
 
-
-def terminal_top_with_text(msg: str = "") -> str:
-    width = os.get_terminal_size().columns
-    if len(msg) > width - 5:
-        x = "=" * width
-        x += "\n" + msg
-        x += "\n" + "=" * width // 2  # type: ignore
-    else:
-        x = "=" * (width - len(msg) - 1) + " " + msg
-    return x
-
-
-def get_logger():
-    logger = logging.getLogger("fury")
-    lvl = os.getenv("FURY_LOG_LEVEL", "info").upper()
-    logger.setLevel(getattr(logging, lvl))
-    log_handler = logging.StreamHandler()
-    log_handler.setFormatter(
-        logging.Formatter("[%(asctime)s] [%(levelname)s] [%(filename)s:%(lineno)d] %(message)s", datefmt="%Y-%m-%dT%H:%M:%S%z")
-    )
-    logger.addHandler(log_handler)
-    return logger
-
-
-logger = get_logger()
+from chainfury.utils import logger, terminal_top_with_text
+from chainfury.types import FENode
 
 
 class Secret(str):
     """This class just means that in Var it will be taken as a password field"""
 
+    def __init__(self, value):
+        self.value = value
+
 
 #
 # Vars: this is the base class for all the fields that the user can provide from the front end
 #
 
 
 class Var:
@@ -61,14 +38,28 @@
         required: bool = False,
         placeholder: str = "",
         show: bool = False,
         name: str = "",
         *,
         loc: Optional[Tuple] = (),
     ):
+        """`Var` is a single input / output for a node.
+
+        Args:
+            type (Union[str, List[Var]]): The type of the variable. If it is a list, then it is a list of Var objects.
+            format (str, optional): The format of the variable. Defaults to "".
+            items (List[Var], optional): If the type is a list, then this is the list of Var objects that are in the list. Defaults to [].
+            additionalProperties (Union[List[Var], Var], optional): If the type is an object, then this is the list of Var objects that are in the object. Defaults to [].
+            password (bool, optional): If the type is a string, then this is whether it is a password field. Defaults to False.
+            required (bool, optional): Whether this field is required. Defaults to False.
+            placeholder (str, optional): The placeholder text for this field. Defaults to "".
+            show (bool, optional): Whether this field should be shown. Defaults to False.
+            name (str, optional): The name of this field. Defaults to "".
+            loc (Optional[Tuple], optional): The location of this field. Defaults to ().
+        """
         self.type = type
         self.format = format
         self.items = items or []
         self.additionalProperties = additionalProperties
         self.password = password
         #
         self.required = required
@@ -79,14 +70,19 @@
         self.value = None
         self.loc = loc  # this is the location from which this value is extracted
 
     def __repr__(self) -> str:
         return f"Var({'*' if self.required else ''}'{self.name}', type={self.type}, items={self.items}, additionalProperties={self.additionalProperties})"
 
     def to_dict(self) -> Dict[str, Any]:
+        """Serialise this Var to a dictionary that can be JSON serialised and sent to the client.
+
+        Returns:
+            Dict[str, Any]: The serialised Var.
+        """
         d: Dict[str, Any] = {"type": self.type}
         if type(self.type) == list and len(self.type) and type(self.type[0]) == Var:
             d["type"] = [x.to_dict() for x in self.type]
         if self.format:
             d["format"] = self.format
         if self.items:
             d["items"] = [item.to_dict() for item in self.items]
@@ -108,14 +104,22 @@
             d["name"] = self.name
         if self.loc:
             d["loc"] = self.loc
         return d
 
     @classmethod
     def from_dict(cls, d: Dict[str, Any]) -> "Var":
+        """Deserialise a Var from a dictionary.
+
+        Args:
+            d (Dict[str, Any]): The dictionary to deserialise from.
+
+        Returns:
+            Var: The deserialised Var.
+        """
         type_val = d.get("type")
         format_val = d.get("format", "")
         items_val = d.get("items", [])
         additional_properties_val = d.get("additionalProperties", [])
         password_val = d.get("password", False)
         required_val = d.get("required", False)
         placeholder_val = d.get("placeholder", "")
@@ -144,20 +148,43 @@
             show=show_val,
             name=name_val,
             loc=loc_val,
         )
         return var
 
     def set_value(self, v: Any):
+        """Set the value of this Var.
+
+        Args:
+            v (Any): The value to set.
+        """
         self.value = v
 
 
-def pyannotation_to_json_schema(x, allow_any, allow_exc, allow_none, *, trace: bool = False) -> Var:
-    """Function to convert the given annotation from python to a Var which can then be
-    JSON serialised and sent to the clients."""
+def pyannotation_to_json_schema(
+    x: Any,
+    allow_any: bool,
+    allow_exc: bool,
+    allow_none: bool,
+    *,
+    trace: bool = False,
+) -> Var:
+    """Function to convert the given annotation from python to a Var which can then be JSON serialised and sent to the
+    clients.
+
+    Args:
+        x (Any): The annotation to convert.
+        allow_any (bool): Whether to allow the `Any` type.
+        allow_exc (bool): Whether to allow the `Exception` type.
+        allow_none (bool): Whether to allow the `None` type.
+        trace (bool, optional): Adds verbosity the schema generation. Defaults to False.
+
+    Returns:
+        Var: The converted annotation.
+    """
     if isinstance(x, type):
         if trace:
             logger.debug("t0")
 
         if x == str:
             return Var(type="string")
         elif x == int or x == float:
@@ -171,15 +198,15 @@
         elif x == dict:
             return Var(type="object", additionalProperties=Var(type="string"))
 
         # there are some types that are unique to the fury system
         elif x == Secret:
             return Var(type="string", password=True)
         elif x == Model:
-            return Var(type=Model.type_name, required=False, show=False)
+            return Var(type=Model.TYPE_NAME, required=False, show=False)
         if x == Exception and allow_exc:
             return Var(type="exception", required=False, show=False)
         elif x == type(None) and allow_none:
             return Var(type="null", required=False, show=False)
         else:
             raise ValueError(f"i0: Unsupported type: {x}")
     elif isinstance(x, str):
@@ -252,35 +279,47 @@
         return Var(type="string")
     else:
         if trace:
             logger.debug("t6")
         raise ValueError(f"i4: Unsupported type: {x}")
 
 
-def func_to_vars(func) -> List[Var]:
+def func_to_vars(func: object) -> List[Var]:
     """
     Extracts the signature of a function and converts it to an array of Var objects.
+
+    Args:
+        func (Callable): The function to extract the signature from.
+
+    Returns:
+        List[Var]: The array of Var objects.
     """
-    signature = inspect.signature(func)
+    signature = inspect.signature(func)  # type: ignore
     fields = []
     for param in signature.parameters.values():
         schema = pyannotation_to_json_schema(param.annotation, allow_any=False, allow_exc=False, allow_none=False)
         schema.required = param.default is inspect.Parameter.empty
         schema.name = param.name
         schema.placeholder = str(param.default) if param.default is not inspect.Parameter.empty else ""
         if not schema.name.startswith("_"):
             schema.show = True
         fields.append(schema)
     return fields
 
 
 def func_to_return_vars(func, returns: Dict[str, Tuple]) -> List[Var]:
     """
-    Analyses the return annotation type of the signature of a function and converts it to an array of
-    named Var objects.
+    Analyses the return annotation type of the signature of a function and converts it to an array of named Var objects.
+
+    Args:
+        func (Callable): The function to extract the signature from.
+        returns (Dict[str, Tuple]): The dictionary of return types.
+
+    Returns:
+        List[Var]: The array of Var objects.
     """
     signature = inspect.signature(func)
     schema = pyannotation_to_json_schema(signature.return_annotation, allow_any=False, allow_exc=True, allow_none=True)
     if not (
         schema.type == "array"
         and len(schema.items) == 2
         and type(schema.items[1].type) == list
@@ -309,14 +348,23 @@
             ret,
         ]
     logger.debug(f"FINAL: {ret}")
     return ret
 
 
 def jinja_schema_to_vars(v) -> Var:
+    """
+    Converts a Jinja schema to a Var object.
+
+    Args:
+        v ([type]): The Jinja schema.
+
+    Returns:
+        Var: The Var object.
+    """
     if type(v) == j2sm.Scalar or type(v) == j2sm.String:
         field = Var(type="string", required=True)
     elif type(v) == j2sm.Number:
         field = Var(type="number", required=True)
     elif type(v) == j2sm.Boolean:
         field = Var(type="boolean", required=True)
     elif type(v) == j2sm.Unknown:
@@ -340,14 +388,23 @@
             field.items = [jinja_schema_to_vars(x) for x in v.items]
     else:
         raise ValueError(f"cannot handle type {type(v)}")
     return field
 
 
 def jtype_to_vars(prompt: str) -> List[Var]:
+    """
+    Converts a Jinja prompt to an array of Var objects.
+
+    Args:
+        prompt (str): The Jinja prompt.
+
+    Returns:
+        List[Var]: The array of Var objects.
+    """
     try:
         s = jinja2schema.infer(prompt)
         fields = []
         for k, v in s.items():
             f = jinja_schema_to_vars(v)
             f.name = k
             fields.append(f)
@@ -356,25 +413,43 @@
             "Could not parse prompt to jinja schema. We support only for/if/filters in jinja2. "
             "Please read here for more information: https://jinja.palletsprojects.com/en/3.1.x/templates/"
         )
         raise e
     return fields
 
 
-def extract_jinja_indices(data, current_index=(), indices=None) -> List:
+def extract_jinja_indices(data: Union[str, List, Dict[str, Any]], current_index=(), indices=None) -> List:
     """
-    Returns things like:
+    This takes in a nested object and returns all the locations where jinja template was detected.
 
-    [(('3', 'content'), [Var('num1', type=string, items=[], additionalProperties=[]), Var('num2', type=string, items=[], additionalProperties=[])])]
-    [((), [Var('message', type=string, items=[], additionalProperties=[])])]
-    [(('meta_prompt', 'data'), [Var('place', type=string, items=[], additionalProperties=[])])]
-    [('0', [Var('name', type=string, items=[], additionalProperties=[])])]
-    [(('meta', 'ptype'), [Var('genome', type=string, items=[], additionalProperties=[])])]
-    [(('level-0', 'level-1', 'level-2'), [Var('thing', type=string, items=[], additionalProperties=[])]), (('level-0', 'nice'), [Var('feeling', type=string, items=[], additionalProperties=[])])]
-    []
+    Args:
+        data (Union[str, List, Dict[str, Any]]): The nested object.
+        current_index (tuple, optional): The current index. Defaults to ().
+        indices ([type], optional): The indices. Defaults to None.
+
+    Returns:
+        List: The list of indices.
+
+    Example:
+        >>> from chainfury.base import extract_jinja_indices
+        >>> extract_jinja_indices({
+        ...     "foo": {
+        ...         "bar": "{{ baz }}",
+        ...         "gaa": ["{{ joo }}"]
+        ...    }
+        ... })
+        [(('foo', 'bar'), Var(...)), (('foo', 'gaa', '0'), Var(...))]
+        >>> # more examples
+        [(('3', 'content'), [Var('num1', type=string, items=[], additionalProperties=[]), Var('num2', type=string, items=[], additionalProperties=[])])]
+        [((), [Var('message', type=string, items=[], additionalProperties=[])])]
+        [(('meta_prompt', 'data'), [Var('place', type=string, items=[], additionalProperties=[])])]
+        [('0', [Var('name', type=string, items=[], additionalProperties=[])])]
+        [(('meta', 'ptype'), [Var('genome', type=string, items=[], additionalProperties=[])])]
+        [(('level-0', 'level-1', 'level-2'), [Var('thing', type=string, items=[], additionalProperties=[])]), (('level-0', 'nice'), [Var('feeling', type=string, items=[], additionalProperties=[])])]
+        []
     """
     if indices is None:
         indices = []
 
     if isinstance(data, str):
         fields = jtype_to_vars(data)
         if fields:
@@ -384,44 +459,60 @@
             if current_index:
                 if type(current_index) == tuple:
                     new_index = (*current_index, i)
                 else:
                     new_index = (current_index, i)
             else:
                 new_index = str(i)
-            extract_jinja_indices(item, new_index, indices)
+            extract_jinja_indices(data=item, current_index=new_index, indices=indices)
     elif isinstance(data, dict):
         for key, value in data.items():
             if current_index:
                 if type(current_index) == tuple:
                     new_index = (*current_index, key)
                 else:
                     new_index = (current_index, key)
             else:
                 new_index = key
-            extract_jinja_indices(value, new_index, indices)
+            extract_jinja_indices(data=value, current_index=new_index, indices=indices)
 
     return indices
 
 
-def get_value_by_keys(obj, keys):
+def get_value_by_keys(obj, keys) -> Any:
+    """Takes in an arbitrary nested object and returns the value at the location specified by the keys.
+
+    Args:
+        obj (Union[List, Dict[str, Any]]): The nested object.
+        keys (Union[str, List[str], Tuple[str, ...]]): The keys. See `extract_jinja_indices` for examples.
+
+    Returns:
+        Any: The value at the location specified by the keys.
+    """
     if not keys:
         return obj
     keys = (keys,) if not isinstance(keys, (list, tuple)) else keys
     key = keys[0]
     if isinstance(obj, dict):
         return get_value_by_keys(obj.get(key), keys[1:])
     elif isinstance(obj, (list, tuple)):
         key = int(key)
         if isinstance(key, int) and 0 <= key < len(obj):
             return get_value_by_keys(obj[key], keys[1:])
     return None
 
 
-def put_value_by_keys(obj, keys, value):
+def put_value_by_keys(obj, keys, value: Any):
+    """Takes in an arbitrary nested object and sets the value at the location specified by the keys.
+
+    Args:
+        obj (Union[List, Dict[str, Any]]): The nested object.
+        keys (Union[str, List[str], Tuple[str, ...]]): The keys. See `extract_jinja_indices` for examples.
+        value (Any): The value to set.
+    """
     if not keys:
         return
 
     keys = (keys,) if not isinstance(keys, (list, tuple)) else keys
     key = keys[0]
     if len(keys) == 1:
         if isinstance(obj, dict):
@@ -441,55 +532,75 @@
 
 #
 # Model: Each model is the processing engine of the AI actions. It is responsible for keeping
 #        the state of each of the wrapped functions for different API calls.
 #
 
 
-class ModelTags:
-    TEXT_TO_TEXT = "text_to_text"
-    TEXT_TO_IMAGE = "text_to_image"
-    IMAGE_TO_IMAGE = "image_to_image"
-
-
 class Model:
-    model_tags = ModelTags
-    type_name = "model"
+    TYPE_NAME = "model"
+    """constant for the type name"""
 
     def __init__(
         self,
-        collection_name,
-        id,
+        collection_name: str,
+        id: str,
         fn: object,
         description,
         usage: List[Union[str, int]] = [],
         tags=[],
     ):
+        """Defines a single callable model.
+
+        Args:
+            collection_name (str): The name of the collection.
+            id (str): The id of the model.
+            fn (Callable): The callable to wrap.
+            description (str): The description of the model.
+            usage (List[Union[str, int]], optional): The location that tells usage for a call. Defaults to [].
+            tags (List[str], optional): The tags for the model. Defaults to [].
+        """
         self.collection_name = collection_name
         self.id = id
         self.fn = fn
         self.description = description
         self.usage = usage
         self.vars = func_to_vars(fn)
         self.tags = tags
 
     def __repr__(self) -> str:
         return f"Model('{self.collection_name}', '{self.id}')"
 
     def to_dict(self, no_vars: bool = False) -> Dict[str, Any]:
+        """Converts the model to a dictionary.
+
+        Args:
+            no_vars (bool, optional): Whether to include the vars. Defaults to False.
+
+        Returns:
+            Dict[str, Any]: The dictionary representation of the model.
+        """
         return {
             "collection_name": self.collection_name,
             "id": self.id,
             "description": self.description,
             "usage": self.usage,
             "vars": [x.to_dict() for x in self.vars] if not no_vars else [],
             "tags": self.tags,
         }
 
     def __call__(self, model_data: Dict[str, Any]) -> Tuple[Any, Optional[Exception]]:
+        """Calls the model with the given data.
+
+        Args:
+            model_data (Dict[str, Any]): The data to pass to the model.
+
+        Returns:
+            Tuple[Any, Optional[Exception]]: The result of the model and the exception if any.
+        """
         try:
             out = self.fn(**model_data)  # type: ignore
             return out, None
         except Exception as e:
             return traceback.format_exc(), e
 
 
@@ -498,38 +609,43 @@
 #       its inputs, outputs and fields that are shown in the UI. It can be of different types and
 #       it only wraps teh
 #
 
 
 class NodeType:
     PROGRAMATIC = "programatic"
+    """constant for the programatic node type"""
     AI = "ai-powered"
-
-
-class NodeConnection:
-    def __init__(self, id: str, name: str = "", required: bool = False, description: str = ""):
-        self.id = id
-        self.name = name
-        self.required = required
-        self.description = description
+    """constant for the AI node type"""
 
 
 class Node:
     types = NodeType()
 
     def __init__(
         self,
         id: str,
         type: str,
         fn: object,  # the function to call
         fields: List[Var],
         outputs: List[Var],
         description: str = "",
-        tags: str = [],
+        tags: List[str] = [],
     ):
+        """Node is a single unit of computation in a Dag. All the actions are considered as nodes.
+
+        Args:
+            id (str): The id of the node.
+            type (str): The type of the node. See `Node.types` for valid types.
+            fn (object): The function to call.
+            fields (List[Var]): The fields of the node.
+            outputs (List[Var]): The outputs of the node.
+            description (str, optional): The description of the node. Defaults to "".
+            tags (List[str], optional): The tags for the node. Defaults to [].
+        """
         # some bacic checks
         if type == NodeType.AI:
             pass
         elif type == NodeType.PROGRAMATIC:
             pass
         else:
             raise ValueError(f"Invalid node type: {type}, see Node.types for valid types")
@@ -550,35 +666,61 @@
                 out += f"\n      {f},"
         out += f"\n] ({len(self.fields)}) => ({len(self.outputs)}) ["
         for o in self.outputs:
             out += f"\n      {o},"
         out += f"\n] }}"
         return out
 
-    def has_field(self, field: str):
+    def has_field(self, field: str) -> bool:
+        """helper function to check if the node has a field with the given name.
+
+        Args:
+            field (str): The name of the field to check.
+
+        Returns:
+            bool: True if the node has the field, False otherwise.
+        """
         return any([x.name == field for x in self.fields])
 
     def to_dict(self) -> Dict[str, Any]:
+        """Converts the node to a dictionary.
+
+        Returns:
+            Dict[str, Any]: The dictionary representation of the node.
+        """
         from chainfury.agent import AIAction
 
         fn = {}
+        name = self.id
         if isinstance(self.fn, AIAction):
             fn = self.fn.to_dict(no_vars=True)
+            name = fn.pop("action_name")
 
         return {
             "id": self.id,
             "type": self.type,
             "fn": fn,
+            "name": name,
             "description": self.description,
             "fields": [field.to_dict() for field in self.fields],
             "outputs": [o.to_dict() for o in self.outputs],
         }
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Any]):
+    def from_dict(cls, data: Dict[str, Any], verbose: bool = False) -> "Node":
+        """Creates a node from a dictionary.
+
+        Args:
+            data (Dict[str, Any]): The dictionary representation of the node.
+
+        Returns:
+            Node: The node created from the dictionary.
+        """
+        if verbose:
+            logger.info("Creating node from dict: %s", data)
         fields = [Var.from_dict(x) for x in data["fields"]]
         outputs = [Var.from_dict(x) for x in data["outputs"]]
         fn = data["fn"]
         if not fn:
             raise ValueError(f"Invalid fn: {fn}")
 
         from chainfury.agent import AIAction
@@ -591,21 +733,46 @@
             fn=ai_action,
             description=data["description"],
             fields=fields,
             outputs=outputs,
         )
 
     def to_json(self, indent=None) -> str:
+        """Converts the node to a json string.
+
+        Args:
+            indent (int, optional): The indent to use. Defaults to None.
+
+        Returns:
+            str: The json string representation of the node.
+        """
         return json.dumps(self.to_dict(), indent=indent)
 
     @classmethod
-    def from_json(cls, data: str):
+    def from_json(cls, data: str) -> "Node":
+        """Creates a node from a json string.
+
+        Args:
+            data (str): The json string representation of the node.
+
+        Returns:
+            Node: The node created from the json string.
+        """
         return cls.from_dict(json.loads(data))
 
     def __call__(self, data: Dict[str, Any], print_thoughts: bool = False) -> Tuple[Any, Optional[Exception]]:
+        """Calls the node with the given data.
+
+        Args:
+            data (Dict[str, Any]): The data to pass to the node.
+            print_thoughts (bool, optional): Whether to print the thoughts of the node, useful for debugging. Defaults to False.
+
+        Returns:
+            Tuple[Any, Optional[Exception]]: The result of the node and the exception if any.
+        """
         data_keys = set(data.keys())
         template_keys = set([x.name for x in self.fields])
         try:
             if not data_keys.issubset(template_keys):
                 raise ValueError(f"Invalid keys passed to node '{self.id}': {data_keys - template_keys}")
             if print_thoughts:
                 print(terminal_top_with_text(f"Node: {self.id}"))
@@ -635,124 +802,303 @@
 
 #
 # Edge: Each connection between two boxes on the UI is called an Edge, it is only a dataclass without any methods.
 #
 
 
 class Edge:
-    def __init__(self, src_node_id: str, trg_node_id: str, *connections: Tuple[str, str]):
-        # some basic checks
-        for c in connections:
-            assert isinstance(c, (tuple, list)), f"Invalid connection: {c}"
-            assert len(c) == 2, f"Invalid connection: {c}"
-            assert isinstance(c[0], str), f"Invalid connection: {c}"
-            assert isinstance(c[1], str), f"Invalid connection: {c}"
+    """Creates an edge between two nodes.
 
+    Args:
+        src_node_id (str): The id of the source node.
+        src_node_var (str): The name of the source node variable.
+        trg_node_id (str): The id of the target node.
+        trg_node_var (str): The name of the target node variable.
+    """
+
+    def __init__(
+        self,
+        src_node_id: str,
+        src_node_var: str,
+        trg_node_id: str,
+        trg_node_var,
+    ):
         self.src_node_id = src_node_id
         self.trg_node_id = trg_node_id
-        self.connections = connections
+        self.src_node_var = src_node_var
+        self.trg_node_var = trg_node_var
 
     def __repr__(self) -> str:
-        out = f"FuryEdge('{self.src_node_id}' => '{self.trg_node_id}',"
-        for c in self.connections:
-            out += f"\n  {c[0]} -> {c[1]},"
-        out += "\n)"
+        out = f"FuryEdge('{self.src_node_id}/{self.src_node_var}' => '{self.trg_node_id}/{self.trg_node_var}')"
         return out
 
     def to_dict(self) -> Dict[str, Any]:
+        """Serializes the edge to a dictionary.
+
+        Returns:
+            Dict[str, Any]: The dictionary representation of the edge.
+        """
         return {
-            "src_node_id": self.src_node_id,
-            "trg_node_id": self.trg_node_id,
-            "connections": self.connections,
+            "source": self.src_node_id,
+            "sourceHandle": self.src_node_var,
+            "target": self.trg_node_id,
+            "targetHandle": self.trg_node_var,
         }
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Any]):
+    def from_dict(cls, data: Dict[str, Any], verbose: bool = False) -> "Edge":
+        """Creates an edge from a dictionary.
+
+        Args:
+            data (Dict[str, Any]): The dictionary representation of the edge.
+
+        Returns:
+            Edge: The edge created from the dictionary.
+        """
         return cls(
-            data["src_node_id"],
-            data["trg_node_id"],
-            *data["connections"],
+            data["source"],
+            data["sourceHandle"],
+            data["target"],
+            data["targetHandle"],
         )
 
 
 #
 # Dag: An entire flow is called the Chain
 #
 
 
 class Chain:
+    """A chain is a full flow of nodes and edges.
+
+    Args:
+        nodes (List[Node], optional): The list of nodes in the chain. Defaults to [].
+        edges (List[Edge], optional): The list of edges in the chain. Defaults to [].
+        sample (Dict[str, Any], optional): The sample data to use for the chain. Defaults to {}.
+        main_in (str, optional): The name of the input var for the chat input. Defaults to "".
+        main_out (str, optional): The name of the output var for the chat output. Defaults to "".
+    """
+
     def __init__(
         self,
         nodes: List[Node] = [],
         edges: List[Edge] = [],
         *,
         sample: Dict[str, Any] = {},
         main_in: str = "",
         main_out: str = "",
     ):
-        self.nodes = {node.id: node for node in nodes}
+        self.nodes: Dict[str, Node] = {node.id: node for node in nodes}
         self.edges = edges
 
         if len(self.nodes) == 1:
             assert len(self.edges) == 0, "Cannot have edges with only 1 node"
             self.topo_order = [next(iter(self.nodes))]
         else:
             self.topo_order = topological_sort(self.edges)
         self.sample = sample
         self.main_in = main_in
         self.main_out = main_out
 
         for node_id in self.topo_order:
             assert node_id in self.nodes, f"Missing node from an edge: {node_id}"
 
+        # to a dry run to validate everything
+        self.to_dict()
+
     def __repr__(self) -> str:
         # return f"FuryDag(nodes: {len(self.nodes)}, edges: {len(self.edges)})"
         out = "FuryDag(\n  nodes: ["
         for n in self.nodes:
             out += f"\n    {n},"
         out += "\n  ],\n  edges: ["
         for e in self.edges:
             out += f"\n    {e},"
-        out += "\n  ]\n)"
+        out += f"\n  ]\n  main_in: {self.main_in}\n  main_out: {self.main_out}\n)"
         return out
 
     def to_dict(self, main_in: str = "", main_out: str = "", sample: Dict[str, Any] = {}) -> Dict[str, Any]:
+        """Serializes the chain to a dictionary.
+
+        Args:
+            main_in (str, optional): The name of the input var for the chat input. Defaults to "".
+            main_out (str, optional): The name of the output var for the chat output. Defaults to "".
+            sample (Dict[str, Any], optional): The sample data to use for the chain. Defaults to {}.
+
+        Returns:
+            Dict[str, Any]: The dictionary representation of the chain.
+        """
         main_in = main_in or self.main_in
         main_out = main_out or self.main_out
         sample = sample or self.sample
-        assert main_in in sample, f"Invalid key: {main_in}"
+        if main_in not in sample:
+            logger.error(f"Key should be present in 'sample': {main_in}")
+        # assert main_in in sample, f"Invalid key: {main_in}"
 
         if not (main_in or main_out or sample):
             logger.warning("No main_in, main_out or sample provided, using defaults")
             raise ValueError("No main_in, main_out or sample provided, using defaults")
         return {
             "nodes": [node.to_dict() for node in self.nodes.values()],
             "edges": [edge.to_dict() for edge in self.edges],
             "topo_order": self.topo_order,
             "sample": sample,
             "main_in": main_in,
             "main_out": main_out,
         }
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Any]):
-        nodes = [Node.from_dict(x) for x in data["nodes"]]
-        edges = [Edge.from_dict(x) for x in data["edges"]]
+    def from_dict(cls, data: Dict[str, Any], verbose: bool = False) -> "Chain":
+        """Creates a chain from a dictionary.
+
+        Args:
+            data (Dict[str, Any]): The dictionary representation of the chain.
+
+        Returns:
+            Chain: The chain created from the dictionary.
+        """
+        nodes = [Node.from_dict(data=x, verbose=verbose) for x in data["nodes"]]
+        edges = [Edge.from_dict(data=x, verbose=verbose) for x in data["edges"]]
         return cls(nodes=nodes, edges=edges, sample=data["sample"], main_in=data["main_in"], main_out=data["main_out"])
 
     def to_json(self) -> str:
+        """Serializes the chain to a JSON string.
+
+        Returns:
+            str: The JSON string representation of the chain.
+        """
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, data: str):
+        """Creates a chain from a JSON string.
+
+        Args:
+            data (str): The JSON string representation of the chain.
+
+        Returns:
+            Chain: The chain created from the JSON string.
+        """
         return cls.from_dict(json.loads(data))
 
+    @classmethod
+    def from_id(cls, id: str):
+        from chainfury.client import get_chain_from_id
+
+        return get_chain_from_id(id)
+
+    def step(
+        self,
+        node_id: str,
+        pre_data: Dict[str, Any],
+        full_ir: Dict[str, Any],
+        print_thoughts: bool = False,
+        thoughts_callback: Optional[Callable] = None,
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        """Performs a single step in the chain, useful for manual debugging.
+
+        Args:
+            node_id (str): The id of the node to step.
+            pre_data (Dict[str, Any]): The data to use for the step.
+            full_ir (Dict[str, Any]): The full IR to use for the step.
+            print_thoughts (bool, optional): Whether to print the thoughts. Defaults to False.
+            thoughts_callback (Optional[Callable], optional): A callback to call with the thoughts. Defaults to None.
+
+        Returns:
+            Tuple[Dict[str, Any], Dict[str, Any]]: The currrent output and updated thoughts ir buffer.
+        """
+        node = self.nodes[node_id]
+        incoming_edges = list(filter(lambda edge: edge.trg_node_id == node_id, self.edges))
+
+        # clear out all the nodes that this thing needs into a separate rep
+        logger.debug(f"Processing node: {node_id}")
+        logger.debug(f"Current full_ir: {set(full_ir.keys())}")
+        _data = {}
+
+        # first check if this node has any fields that are in the data
+        all_keys = list(pre_data.keys())
+        for k in all_keys:
+            if node.has_field(k):
+                _data[k] = pre_data[k]  # don't pop this, some things are shared between actions eg. openai_api_key
+            elif k.startswith(node.id):
+                _data[k.split("/", 1)[1]] = pre_data.pop(k)  # pop this, it is not needed anymore
+
+        # then merge from the ir buffer
+        for edge in incoming_edges:
+            logger.debug(f"Incoming edge: {edge}")
+            req_key = f"{edge.src_node_id}/{edge.src_node_var}"
+            logger.debug(f"Looking for key: {req_key}")
+            # need to check if this information is available in the IR buffer, if it is not then this is an error
+            ir_value = pre_data.get(req_key, None) or full_ir.get(req_key, {}).get("value", None)
+            if ir_value is None:
+                raise ValueError(f"Missing value for {req_key}")
+            _data[edge.trg_node_var] = ir_value
+
+        # then run the node
+        out, err = node(_data, print_thoughts=print_thoughts)
+        if err:
+            logger.error(f"TRACE: {out}")
+            raise err
+
+        yield_dict = {}
+        for k, v in out.items():
+            key = f"{node_id}/{k}"
+            value = {
+                "value": v,
+                "timestamp": datetime.datetime.now().isoformat(),
+            }
+            full_ir[key] = value
+            thought = {"key": key, **value}
+            yield_dict[key] = value
+            if thoughts_callback is not None:
+                thoughts_callback(thought)
+                if print_thoughts:
+                    print(thought)
+
+        return yield_dict, full_ir
+
     def __call__(
-        self, data: Union[str, Dict[str, Any]], thoughts_callback: Optional[Callable] = None, print_thoughts: bool = False
+        self,
+        data: Union[str, Dict[str, Any]],
+        thoughts_callback: Optional[Callable] = None,
+        print_thoughts: bool = False,
     ) -> Tuple[Var, Dict[str, Any]]:
+        """
+        Runs the chain on the given data. In this function it will run a full dataflow engine along with thoughts buffer
+        and a simple callback system at each step.
+
+        Example:
+            >>> chain = Chain(...)
+            >>> out, thoughts = chain("Hello world")
+            >>> print(out)
+            ... The first man chuckled and shook his head, "You always have the weirdest explanations for everything."
+            >>> print(thoughts)
+            ... {
+                    '38c813a2-850c-448b-8cfb-bd5775cc4b61/answer': {
+                        'timestamp': '2023-06-27T16:50:04.178833',
+                        'value': '...'
+                    }
+                    '1378538b-a15e-475b-9a9d-a31a261165c0/out': {
+                        'timestamp': '2023-06-27T16:50:07.818709',
+                        'value': '...'
+                    }
+                }
+
+        You can also stream the intermediate responses by setting using `stream_call` method. You can get the exact same
+        result as above by iterating over the response and getting the last response.
+
+        Args:
+            data (Union[str, Dict[str, Any]]): The data to run the chain on.
+            thoughts_callback (Optional[Callable], optional): The callback function to call at each step. Defaults to None.
+            print_thoughts (bool, optional): Whether to print the thoughts buffer at each step. Defaults to False.
+            stream (bool, optional): Whether to stream the output or not. Defaults to False.
+
+        Returns:
+            Tuple[Var, Dict[str, Any]]: The output of the chain and the thoughts buffer.
+        """
         if not isinstance(data, dict):
             assert isinstance(data, str), f"Invalid data type: {type(data)}"
             assert self.sample and self.main_in, "Cannot run a chain without a sample and main_in for string input, please use a dict input"
             data = {self.main_in: data}
         _data = copy.deepcopy(self.sample)  # don't corrupt yourself over multiple calls
         _data.update(data)
         data = _data
@@ -761,98 +1107,149 @@
             print(terminal_top_with_text("Chain Starts"))
             print("Inputs:\n------")
             print(pformat(data))
 
         full_ir = {}
         out = None
         for node_id in self.topo_order:
-            node = self.nodes[node_id]
-            incoming_edges = list(filter(lambda edge: edge.trg_node_id == node_id, self.edges))
+            yield_dict, full_ir = self.step(
+                node_id=node_id,
+                pre_data=data,
+                full_ir=full_ir,
+                print_thoughts=print_thoughts,
+                thoughts_callback=thoughts_callback,
+            )
 
-            # clear out all the nodes that this thing needs into a separate rep
-            logger.debug(f"Processing node: {node_id}")
-            logger.debug(f"Current full_ir: {set(full_ir.keys())}")
-            _data = {}
-            for edge in incoming_edges:
-                # need to check if this information is available in the IR buffer, if it is not
-                # then this is an error
-                logger.debug(f"Incoming edge: {edge}")
-                for conns in edge.connections:
-                    req_key = f"{edge.src_node_id}/{conns[0]}"
-                    logger.debug(f"Looking for key: {req_key}")
-                    ir_value = full_ir.get(req_key, {}).get("value", None)
-                    if ir_value is None:
-                        raise ValueError(f"Missing value for {req_key}")
-                    _data[conns[1]] = ir_value
-
-            all_keys = list(data.keys())
-            for k in all_keys:
-                if node.has_field(k):
-                    _data[k] = data[k]  # don't pop this, some things are shared between actions eg. openai_api_key
-            out, err = node(_data, print_thoughts=print_thoughts)
-            if err:
-                logger.error("TRACE: {out}")
-                raise err
+        if self.main_out:
+            out = full_ir.get(self.main_out)["value"]  # type: ignore
 
-            for k, v in out.items():
-                key = f"{node_id}/{k}"
-                value = {
-                    "value": v,
-                    "timestamp": datetime.datetime.now().isoformat(),
+        if print_thoughts:
+            print(terminal_top_with_text("Chain Last"))
+            print("Outputs:\n------")
+            print(pformat(out))
+            print(terminal_top_with_text("Chain Ends"))
+
+        return out, full_ir  # type: ignore
+
+    def stream(
+        self,
+        data: Union[str, Dict[str, Any]],
+        thoughts_callback: Optional[Callable] = None,
+        print_thoughts: bool = False,
+    ) -> Generator[Tuple[Union[Any, Dict[str, Any]], bool], None, None]:
+        """
+        This is a streaming version of __call__ method. It will yield the intermediate responses as they come in.
+
+        Example:
+            >>> chain = Chain(...)
+            >>> cf_response_gen = chain.stream("Hello world")
+            >>> out = None
+            >>> thoughts = {}
+            >>> for ir, done in cf_response_gen:
+            ...     if done:
+            ...         out = ir
+            ...     else:
+            ...         thoughts.update(ir)
+            >>> print(out)
+            ... The first man chuckled and shook his head, "You always have the weirdest explanations for everything."
+            >>> print(thoughts)
+            ... {
+                    '38c813a2-850c-448b-8cfb-bd5775cc4b61/answer': {
+                        'timestamp': '2023-06-27T16:50:04.178833',
+                        'value': '...'
+                    }
+                    '1378538b-a15e-475b-9a9d-a31a261165c0/out': {
+                        'timestamp': '2023-06-27T16:50:07.818709',
+                        'value': '...'
+                    }
                 }
-                full_ir[key] = value
-                thought = {"key": key, **value}
-                if thoughts_callback is not None:
-                    thoughts_callback(thought)
-                    if print_thoughts:
-                        print(thought)
+
+        Args:
+            data (Union[str, Dict[str, Any]]): The data to run the chain on.
+            thoughts_callback (Optional[Callable], optional): The callback function to call at each step. Defaults to None.
+            print_thoughts (bool, optional): Whether to print the thoughts buffer at each step. Defaults to False.
+
+        Yields:
+            Generator[Tuple[Union[Any, Dict[str, Any]], bool], None, None]: The intermediate responses and whether the
+            response is the final response or not.
+        """
+        if not isinstance(data, dict):
+            assert isinstance(data, str), f"Invalid data type: {type(data)}"
+            assert self.sample and self.main_in, "Cannot run a chain without a sample and main_in for string input, please use a dict input"
+            data = {self.main_in: data}
+        _data = copy.deepcopy(self.sample)  # don't corrupt yourself over multiple calls
+        _data.update(data)
+        data = _data
+
+        if print_thoughts:
+            print(terminal_top_with_text("Chain Starts"))
+            print("Inputs:\n------")
+            print(pformat(data))
+
+        full_ir = {}
+        out = None
+        for node_id in self.topo_order:
+            yield_dict, full_ir = self.step(
+                node_id=node_id,
+                pre_data=data,
+                full_ir=full_ir,
+                print_thoughts=print_thoughts,
+                thoughts_callback=thoughts_callback,
+            )
+            yield yield_dict, False
 
         if print_thoughts:
             print(terminal_top_with_text("Chain Last"))
             print("Outputs:\n------")
             print(pformat(out))
             print(terminal_top_with_text("Chain Ends"))
 
         if self.main_out:
             out = full_ir.get(self.main_out)["value"]  # type: ignore
-        return out, full_ir  # type: ignore
+        yield out, True
 
 
 #
 # helper functions
 #
 
 
 class NotDAGError(Exception):
     pass
 
 
 def edge_array_to_adjacency_list(edges: List[Edge]):
-    """Convert silk format dag edges to adjacency list format"""
     adjacency_lists = {}
     for edge in edges:
         src = edge.src_node_id
         dst = edge.trg_node_id
         if src not in adjacency_lists:
             adjacency_lists[src] = []
         adjacency_lists[src].append(dst)
     return adjacency_lists
 
 
 def adjacency_list_to_edge_map(adjacency_list) -> List[Edge]:
-    """Convert adjacency list format to silk format dag edges"""
     edges = []
     for src, dsts in adjacency_list.items():
         for dst in dsts:
-            edges.append(Edge(src_node_id=src, trg_node_id=dst))
+            edges.append(Edge(src_node_id=src, src_node_var="", trg_node_id=dst, trg_node_var=""))
     return edges
 
 
 def topological_sort(edges: List[Edge]) -> List[str]:
-    """Topological sort of a DAG, raises NotDAGError if the graph is not a DAG"""
+    """Topological sort of a DAG, raises NotDAGError if the graph is not a DAG. This is full proof version
+    which will work even if the DAG contains several unconnected chains.
+
+    Args:
+        edges (List[Edge]): The edges of the DAG
+
+    Returns:
+        List[str]: The topologically sorted list of node ids
+    """
     adjacency_lists = edge_array_to_adjacency_list(edges)
     in_degree = defaultdict(int)
     for src, dsts in adjacency_lists.items():
         for dst in dsts:
             in_degree[dst] += 1
 
     # Add all nodes with no incoming edges to the queue
```

### Comparing `chainfury-0.1.1/chainfury/components/README.md` & `chainfury-1.2.0/chainfury/components/README.md`

 * *Files identical despite different names*

### Comparing `chainfury-0.1.1/chainfury/components/__init__.py` & `chainfury-1.2.0/chainfury/components/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from chainfury.components.openai import openai_chat, openai_completion
+from chainfury.components.serper import serper_api
 from chainfury.components.stability import (
     stability_image_to_image,
     stability_image_to_image_masking,
     stability_image_to_image_upscale,
     stability_text_to_image,
 )
 from chainfury.components.functional import (
@@ -25,8 +26,9 @@
     "stability_image_to_image_masking",
     "stability_image_to_image_upscale",
     #
     # functional things
     "call_api_requests",
     "regex_search",
     "regex_substitute",
+    "serper_api",
 ]
```

### Comparing `chainfury-0.1.1/chainfury/components/openai/__init__.py` & `chainfury-1.2.0/chainfury/components/openai/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import requests
 from typing import Any, List, Union, Dict
 
-from chainfury import Secret, model_registry, exponential_backoff, Model
+from chainfury import Secret, model_registry, exponential_backoff, Model, UnAuthException
+from chainfury.components.const import Env
 
 
 def openai_completion(
-    openai_api_key: Secret,
     model: str,
     prompt: Union[str, List[Union[str, List[str]]]],
+    openai_api_key: Secret = Secret(""),
     max_tokens: int = 16,
     temperature: float = 1,
     top_p: float = 1,
     n: int = 1,
     logprobs: int = 0,
     echo: bool = False,
     stop: Union[str, List[str]] = "",
     presence_penalty: float = 0,
     frequency_penalty: float = 0,
     best_of: int = 1,
     logit_bias: dict = {},
     user: str = "",
     *,
-    raw: bool = False,
+    retry_count: int = 3,
+    retry_delay: int = 1,
 ) -> Dict[str, Any]:
     """
     Generate text completion using OpenAI's GPT-3 API.
 
     Args:
         model (str): ID of the model to use.
         prompt (Union[str, List[Union[str, List[str]]]]): The prompt(s) to generate completions for.
             Encoded as a string, array of strings, array of tokens, or array of token arrays.
+        openai_api_key (Secret): The OpenAI API key. Defaults to "" or the OPENAI_TOKEN environment variable.
         max_tokens (Optional[int]): The maximum number of tokens to generate in the completion. Defaults to 16.
         temperature (Optional[float]): What sampling temperature to use, between 0 and 2. Defaults to 1.
         top_p (Optional[float]): An alternative to sampling with temperature. Defaults to 1.
         n (Optional[int]): How many completions to generate for each prompt. Defaults to 1.
         logprobs (Optional[int]): Include the log probabilities on the logprobs most likely tokens.
             The maximum value for logprobs is 5. Defaults to None.
         echo (Optional[bool]): Echo back the prompt in addition to the completion. Defaults to False.
@@ -53,14 +56,18 @@
         user (Optional[str]): A unique identifier representing your end-user, which can help OpenAI to monitor and detect
             abuse. Defaults to None.
 
     Returns:
         Any: The completion(s) generated by the API.
 
     """
+    if not openai_api_key:
+        openai_api_key = Secret(Env.OPENAI_TOKEN("")).value
+    if not openai_api_key:
+        raise Exception("OpenAI API key not found. Please set OPENAI_TOKEN environment variable or pass through function")
 
     def _fn():
         r = requests.post(
             "https://api.openai.com/v1/completions",
             headers={
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {openai_api_key}",
@@ -78,71 +85,78 @@
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "best_of": best_of,
                 "logit_bias": logit_bias,
                 "user": user,
             },
         )
+        if r.status_code == 401:
+            raise UnAuthException(r.text)
         if r.status_code != 200:
             raise Exception(f"OpenAI API returned status code {r.status_code}: {r.text}")
         return r.json()
 
-    return exponential_backoff(_fn)
+    return exponential_backoff(_fn, max_retries=retry_count, retry_delay=retry_delay)
 
 
 model_registry.register(
     model=Model(
         collection_name="openai",
         id="openai-completion",
         fn=openai_completion,
         description="Given a prompt, the model will return one or more predicted completions, and can also return the probabilities of alternative tokens at each position.",
         usage=["usage", "total_tokens"],
     ),
 )
 
 
 def openai_chat(
-    openai_api_key: Secret,
     model: str,
     messages: List[Dict[str, str]],
+    openai_api_key: Secret = Secret(""),
     temperature: float = 1.0,
     top_p: float = 1.0,
     n: int = 1,
     stop: Union[str, List[str]] = "",
     max_tokens: int = 1024,
     presence_penalty: float = 0.0,
     frequency_penalty: float = 0.0,
     logit_bias: dict = {},
     user: str = "",
     *,
-    retry_count: int = 5,
-    max_retry_delay: int = 5,
+    retry_count: int = 3,
+    retry_delay: int = 1,
 ) -> Any:
     """
     Returns a JSON object containing the OpenAI's API chat response.
 
     Args:
         model: ID of the model to use. See the model endpoint compatibility table for details on which models work with the Chat API.
         messages: A list of messages describing the conversation so far, each item contains the folowing keys
             role: The role of the author of this message. One of system, user, or assistant.
             content: The contents of the message.
             name: Optional. The name of the author of this message. May contain a-z, A-Z, 0-9, and underscores, with a maximum length of 64 characters.
+        openai_api_key (Secret): The OpenAI API key. Defaults to "" or the OPENAI_TOKEN environment variable.
         temperature: Optional. What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. We generally recommend altering this or top_p but not both. Defaults to 1.
         top_p: Optional. An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass. So 0.1 means only the tokens comprising the top 10% probability mass are considered. We generally recommend altering this or temperature but not both. Defaults to 1.
         n: Optional. How many chat completion choices to generate for each input message. Defaults to 1.
         stop: Optional. Up to 4 sequences where the API will stop generating further tokens.
         max_tokens: Optional. The maximum number of tokens to generate in the chat completion. The total length of input tokens and generated tokens is limited by the model's context length. Defaults to infinity.
         presence_penalty: Optional. Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far, increasing the model's likelihood to talk about new topics. See more information about frequency and presence penalties. Defaults to 0.
         frequency_penalty: Optional. Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim. See more information about frequency and presence penalties. Defaults to 0.
         logit_bias: Optional. Modify the likelihood of specified tokens appearing in the completion. Accepts a json object that maps tokens (specified by their token ID in the tokenizer) to an associated bias value from -100 to 100. Mathematically, the bias is added to the logits generated by the model prior to sampling. The exact effect will vary per model, but values between -1 and 1 should decrease or increase likelihood of selection; values like -100 or 100 should result in a ban or exclusive selection of the relevant
         user: Optional. A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. Defaults to None.
 
     Returns:
         Any: The completion(s) generated by the API.
     """
+    if not openai_api_key:
+        openai_api_key = Secret(Env.OPENAI_TOKEN("")).value
+    if not openai_api_key:
+        raise Exception("OpenAI API key not found. Please set OPENAI_TOKEN environment variable or pass through function")
 
     def _fn():
         r = requests.post(
             "https://api.openai.com/v1/chat/completions",
             headers={
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {openai_api_key}",
@@ -157,19 +171,21 @@
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "logit_bias": logit_bias,
                 "user": user,
             },
         )
+        if r.status_code == 401:
+            raise UnAuthException(r.text)
         if r.status_code != 200:
             raise Exception(f"OpenAI API returned status code {r.status_code}: {r.text}")
         return r.json()
 
-    return exponential_backoff(_fn)
+    return exponential_backoff(_fn, max_retries=retry_count, retry_delay=retry_delay)
 
 
 model_registry.register(
     model=Model(
         collection_name="openai",
         id="openai-chat",
         fn=openai_chat,
```

### Comparing `chainfury-0.1.1/chainfury/components/stability/__init__.py` & `chainfury-1.2.0/chainfury/components/stability/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import List, Dict, Union, Tuple
+from typing import List, Dict, Union, Tuple, Optional
 
 from chainfury import Secret, model_registry, exponential_backoff, Model
 
 
 def stability_text_to_image(
     stability_api_key: Secret,
     text_prompts: List[Dict[str, Union[str, float]]],
     height: int = 512,
     width: int = 512,
     cfg_scale: float = 7,
     clip_guidance_preset: str = "NONE",
-    sampler: str = None,
+    sampler: str = None,  # type: ignore # see components README.md
     samples: int = 1,
     seed: int = 0,
     steps: int = 50,
-    style_preset: str = None,
-    extras: Dict[str, Union[str, int, float]] = None,
+    style_preset: str = None,  # type: ignore # see components README.md
+    extras: Dict[str, Union[str, int, float]] = None,  # type: ignore # see components README.md
 ) -> List[str]:
     """
     Generate an image from text prompts using the Stability API.
 
     Args:
         text_prompts (List[Dict[str, Union[str, float]]]): An array of text prompts to use for generation. Given a text prompt with the text "A lighthouse on a cliff" and a weight of 0.5, it would be represented as:
             [{"text": "A lighthouse on a cliff", "weight": 0.5}]
@@ -37,15 +37,14 @@
         steps (int): Number of diffusion steps to run. Default: 50.
         style_preset (str): Pass in a style preset to guide the image model towards a particular style. This list of style presets is subject to change.
         extras (Dict[str, Union[str, int, float]]): Extra parameters passed to the engine. These parameters are used for in-development or experimental features and may change without warning, so please use with caution.
 
     Returns:
         List[str]: A list of base64-encoded PNG images.
     """
-
     pass
 
 
 model_registry.register(
     model=Model(
         collection_name="stabilityai",
         id="stability-text-to-image",
@@ -69,55 +68,60 @@
     steps: int = 50,
     style_preset: str = "",
     extras: dict = {},
 ) -> List[bytes]:
     """
     Generate an image using the Stability AI API.
 
-    Parameters:
-    - text_prompts: A list of tuples, each containing a text prompt and a weight. The text prompts will be used for generation.
-    - init_image: An image used to initialize the diffusion process, in lieu of random noise.
-    - init_image_mode: Whether to use image_strength or step_schedule_* to control how much influence the init_image has on the result. Default is "IMAGE_STRENGTH".
-    - image_strength: How much influence the init_image has on the diffusion process. Values close to 1 will yield images very similar to the init_image while values close to 0 will yield images wildly different than the init_image. Default is 0.35.
-    - cfg_scale: How strictly the diffusion process adheres to the prompt text (higher values keep your image closer to your prompt). Default is 7.
-    - clip_guidance_preset: A preset to guide the diffusion process towards a particular style. Default is "NONE".
-    - sampler: Which sampler to use for the diffusion process. If this value is omitted, an appropriate sampler will be selected automatically.
-    - samples: Number of images to generate. Default is 1.
-    - seed: Random noise seed (omit this option or use 0 for a random seed). Default is 0.
-    - steps: Number of diffusion steps to run. Default is 50.
-    - style_preset: Pass in a style preset to guide the diffusion process towards a particular style. Default is "".
-    - extras: Extra parameters passed to the engine. These parameters are used for in-development or experimental features and may change without warning, so please use with caution. Default is an empty dictionary.
+    Args:
+        text_prompts (List[Tuple[str, float]]): A list of tuples, each containing a text prompt and a weight. The text prompts will be used for generation.
+        init_image (bytes): An image used to initialize the diffusion process, in lieu of random noise.
+        init_image_mode (str): Whether to use image_strength or step_schedule_* to control how much influence the init_image has on the result. Default is "IMAGE_STRENGTH".
+        image_strength (float): How much influence the init_image has on the diffusion process. Values close to 1 will yield images very similar to the init_image while values close to 0 will yield images wildly different than the init_image. Default is 0.35.
+        cfg_scale (int): How strictly the diffusion process adheres to the prompt text (higher values keep your image closer to your prompt). Default is 7.
+        clip_guidance_preset (str): A preset to guide the diffusion process towards a particular style. Default is "NONE".
+        sampler (str): Which sampler to use for the diffusion process. If this value is omitted, an appropriate sampler will be selected automatically.
+        samples (int): Number of images to generate. Default is 1.
+        seed (int): Random noise seed (omit this option or use 0 for a random seed). Default is 0.
+        steps (int): Number of diffusion steps to run. Default is 50.
+        style_preset (str): Pass in a style preset to guide the diffusion process towards a particular style. Default is "".
+        extras (dict): Extra parameters passed to the engine. These parameters are used for in-development or experimental features and may change without warning, so please use with caution. Default is an empty dictionary.
 
     Returns:
-    - A list of bytes representing the generated images.
+        List[bytes]: A list of base64-encoded PNG images.
     """
     pass
 
 
 model_registry.register(
     model=Model(
         collection_name="stabilityai",
         id="stability-image-to-image",
         fn=stability_image_to_image,
         description="Modify an image based on a text prompt",
     )
 )
 
 
-def stability_image_to_image_upscale(stability_api_key: Secret, image: bytes, width: int = None, height: int = None) -> bytes:
+def stability_image_to_image_upscale(
+    stability_api_key: Secret,
+    image: bytes,
+    width: int = None,  # type: ignore # see components README.md
+    height: int = None,  # type: ignore # see components README.md
+) -> bytes:
     """
     Upscales an image to a specified width or height.
 
     Args:
-    image (bytes): The image to upscale.
-    width (int, optional): Desired width of the output image. Only one of width or height may be specified.
-    height (int, optional): Desired height of the output image. Only one of width or height may be specified.
+        image (bytes): The image to upscale.
+        width (int, optional): Desired width of the output image. Only one of width or height may be specified.
+        height (int, optional): Desired height of the output image. Only one of width or height may be specified.
 
     Returns:
-    bytes: The upscaled image.
+        bytes: The upscaled image.
     """
     pass
 
 
 model_registry.register(
     model=Model(
         collection_name="stabilityai",
@@ -135,20 +139,20 @@
     stability_api_key: Secret,
     text_prompts: List[Dict[str, float]],
     init_image: bytes,
     mask_source: str,
     mask_image: bytes,
     cfg_scale: float = 7,
     clip_guidance_preset: str = "NONE",
-    sampler: str = None,
+    sampler: str = None,  # type: ignore # see components README.md
     samples: int = 1,
     seed: int = 0,
     steps: int = 50,
-    style_preset: str = None,
-    extras: dict = None,
+    style_preset: str = None,  # type: ignore # see components README.md
+    extras: dict = None,  # type: ignore # see components README.md
 ) -> bytes:
     """
     Generates an image based on text prompts and an initial image. Returns the generated image as bytes.
 
     Args:
         text_prompts (List[Dict[str, Union[str, float]]]): An array of text prompts to use for generation. Each prompt is a dictionary with the following keys:
             'text': str -- The prompt text to use.
```

### Comparing `chainfury-0.1.1/pyproject.toml` & `chainfury-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool.poetry]
 name = "chainfury"
-version = "0.1.1"
+version = "1.2.0"
 description = "ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs."
 authors = ["NimbleBox Engineering <engineering@nimblebox.ai>"]
 license = "Apache V2.0"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/ChainFury"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "0.5.0"
 Jinja2 = "3.1.2"
-jinja2schema="0.1.4"
+jinja2schema = "0.1.4"
+pydantic = "^1.10.7"
+requests = "^2.28.2"
 
 [tool.poetry.scripts]
 chainfury = "chainfury.cli:main"
+cf = "chainfury.cli:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chainfury-0.1.1/setup.py` & `chainfury-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,36 @@
 ['chainfury',
  'chainfury.components',
  'chainfury.components.ai_actions',
  'chainfury.components.functional',
  'chainfury.components.nbx',
  'chainfury.components.openai',
  'chainfury.components.redis',
+ 'chainfury.components.serper',
  'chainfury.components.stability']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Jinja2==3.1.2', 'fire==0.5.0', 'jinja2schema==0.1.4']
+['Jinja2==3.1.2',
+ 'fire==0.5.0',
+ 'jinja2schema==0.1.4',
+ 'pydantic>=1.10.7,<2.0.0',
+ 'requests>=2.28.2,<3.0.0']
 
 entry_points = \
-{'console_scripts': ['chainfury = chainfury.cli:main']}
+{'console_scripts': ['cf = chainfury.cli:main',
+                     'chainfury = chainfury.cli:main']}
 
 setup_kwargs = {
     'name': 'chainfury',
-    'version': '0.1.1',
+    'version': '1.2.0',
     'description': 'ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs.',
-    'long_description': '# 🦋 ChainFury\n\n[![linkcheck](https://img.shields.io/badge/Workflow-Passing-darkgreen)](https://github.com/NimbleBoxAI/ChainFury/actions)\n[![Downloads](https://static.pepy.tech/badge/chainfury)](https://pepy.tech/project/chainfury)\n[![linkcheck](https://img.shields.io/badge/Site-🦋ChainFury-lightblue)](https://chainfury.nbox.ai)\n[![License: Apache](https://img.shields.io/badge/License-Apache%20v2.0-red)](https://github.com/NimbleBoxAI/ChainFury/blob/main/LICENSE) \n[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/NimbleBoxAI.svg?style=social&label=Follow%20%40NimbleBoxAI)](https://twitter.com/NimbleBoxAI)\n[![](https://dcbadge.vercel.app/api/server/KhF38hrAJ2?compact=true&style=flat)](https://discord.com/invite/KhF38hrAJ2)\n\n<img src="./docs/1.png" align="center"/>\n\n🦋 Build complex chat apps using LLMs in 4 clicks ⚡️ [Try it out here](https://chainfury.nbox.ai/)\n\nChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs. \n\nWith a simple GUI inspired by [LangFlow](https://github.com/logspace-ai/langflow), ChainFury enables you to chain components of [LangChain](https://github.com/hwchase17/langchain) together, allowing you to embed more complex chat applications with a simple JS snippet.\n\nChainFury supports a range of features, including but not limited to:\n\n- Recording all prompts and responses and storing them in a database\n- Collecting metrics like response latency\n- Querying OpenAI\'s API to obtain a rating for the response, which it stores in the database\n- Separate scoring mechanism per ChatBot to easily view performance in a dashboard\n- [Plugins](./server/plugins/) to extend the functionality of ChainFury with callbacks\n\n---\n\n<img src="./docs/2.png" align="center"/>\n\n---\nInstalling ChainFury is easy, with two methods available. We suggest using **the Docker method.**\n\n## Method 1: Docker\n\nThe easiest way to install ChainFury is to use Docker. You can use the following command to run ChainFury:\n\n```bash\ndocker build . -f Dockerfile -t chainfury:latest\n\ndocker run --env OPENAI_API_KEY=<your_key_here> -p 8000:8000 chainfury:latest\n```\n\nNow you can access the app on [localhost:8000](http://localhost:8000/ui/).\n\n<details>\n<summary>Optional environment variable for Database</summary>\nYou can also pass a Database URL to the docker container using the `DATABASE_URL` environment variable. If you do not pass a database URL, ChainFury will use a SQLite database.\n\nExample:\n\n```bash\ndocker run -it -E DATABASE_URL="mysql+pymysql://<user>:<password>@127.0.0.1:3306/<database>" -p 8000:8000 chainfury\n```\n</details>\n\n\n---\n## Method 2: Manual\n<details>\n<summary>For this, you will need to build the frontend and and then run the backend. The frontend can be built using the following command:</summary>\n\n```bash\ncd client\nyarn install\nyarn build\n```\n\nTo copy the frontend to the backend, run the following command:\n\n```bash\ncd ..\ncp -r client/dist/ server/static/\nmkdir -p ./server/templates\ncp ./client/dist/index.html ./server/templates/index.html\n```\n\nNow you can install the backend dependencies and run the server. We recommend using Python 3.9 virtual environment for this:\n\n```bash\npython3 -m venv venv\nsource venv/bin/activate\npip install -r requirements.txt\ncd server\npython3 -m uvicorn app:app --log-level=debug --host 0.0.0.0 --port 8000 --workers 1\n```\n</details>\n<!-- collapsable -->\n\n<details>\n<summary>How to run</summary>\n\nAssuming you are in `server` directory, you can run the server using the following command:\n\n```bash\npython3 server.py --port 8000 --config_plugins=\'["echo"]\'\n```\n</details>\n\nNow you can access the app on [localhost:8000](http://localhost:8000/ui/).\n\n---\n\n<img src="./docs/3.png" align="center"/>\n\n---\n\n1. Start the server by using the docker file provided or by using the manual method.\n\n2. Log into ChainFury by entering username = “admin” and password = “admin”\n\n3. Click on create chatbot\n\n4. Use one of the pre-configured chatbots or use the elements to create a custom chatbot.\n\n5. Save & create your chatbot and start chatting with it by clicking the chat on the bottom-right. You can see chatbot statistics and feedback metrics in your ChainFury dashboard.\n\n\n---\n\n<img src="./docs/5.png" align="center"/>\n\n---\n\nThere are six main areas that LangChain is designed to help with.\n\nChainFury consists of the same concepts to build LLM ChatBots. The components are, in increasing order of complexity:\n\n| Glossary | LangChain    | ChainFury    |\n| --- | --- | --- |\n| 📃 LLMs and Prompts | Prompt management, prompt optimization, generic interface for all LLMs, and common utilities for working with LLMs   | Easy prompt management with GUI elements\n| 🔗 Chains | Chains are sequences of calls (whether to an LLM or a different utility). LangChain provides a standard interface for chains, lots of integrations with other tools, and end-to-end chains for common applications | Easy chain management with GUI |\n| 📚 Data Augmented Generation | Data Augmented Generation involves specific types of chains that first interact with an external datasource to fetch data to use in the generation step. Examples of this include summarization of long pieces of text and question/answering over specific data sources | Coming soon |\n| 🤖 Agents | Agents involve an LLM making decisions about which Actions to take, taking that Action, seeing an Observation, and repeating that until done. LangChain provides a standard interface for agents, a selection of agents to choose from, and examples of end to end agents| Easy agent management with GUI |\n| 🧠 Memory | Memory is the concept of persisting state between calls of a chain/agent. LangChain provides a standard interface for memory, a collection of memory implementations, and examples of chains/agents that use memory | Memory modules are supported, persistant memory coming soon |\n| 🧐 Evaluation | [BETA] Generative models are notoriously hard to evaluate with traditional metrics. One new way of evaluating them is using language models themselves to do the evaluation. LangChain provides some prompts/chains for assisting in this | Auto evaluation of all prompts though OpenAI APIs |\n\n\n---\n\n<img src="./docs/4.png" align="center"/>\n\n---\nChainFury is an open-source project, and is currently in the alpha stage. We are open to contributions to the project in the form of features, infrastructure or documentation.\n\n- To contribute to this project, please follow a ["fork and pull request"](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) workflow. Please do not try to push directly to this repo unless you are maintainer.\n\n- Our [issues](https://github.com/NimbleBoxAI/ChainFury/issues) page is kept up to date with bugs, improvements, and feature requests.\n\n- If you\'re looking for help with your code, consider posting a question on the [GitHub Discussions board](https://github.com/NimbleBoxAI/ChainFury/discussions), so that more people can benefit from it.\n\n- **Describing your issue:** Try to provide as many details as possible. What exactly goes wrong? How is it failing? Is there an error? "XY doesn\'t work" usually isn\'t that helpful for tracking down problems. Always remember to include the code you ran and if possible, extract only the relevant parts and don\'t just dump your entire script. This will make it easier for us to reproduce the error.\n\n- **Sharing long blocks of code or logs:** If you need to include long code, logs or tracebacks, you can wrap them in `<details>` and `</details>`. This [collapses the content](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/details) so it only becomes visible on click, making the issue easier to read and follow.\n\n',
+    'long_description': '# 🦋 ChainFury\n\n[![linkcheck](https://img.shields.io/badge/Workflow-Passing-darkgreen)](https://github.com/NimbleBoxAI/ChainFury/actions)\n[![Downloads](https://static.pepy.tech/badge/chainfury)](https://pepy.tech/project/chainfury)\n[![linkcheck](https://img.shields.io/badge/Site-🦋ChainFury-lightblue)](https://chainfury.nbox.ai)\n[![License: Apache](https://img.shields.io/badge/License-Apache%20v2.0-red)](https://github.com/NimbleBoxAI/ChainFury/blob/main/LICENSE) \n[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/NimbleBoxAI.svg?style=social&label=Follow%20%40NimbleBoxAI)](https://twitter.com/NimbleBoxAI)\n[![](https://dcbadge.vercel.app/api/server/KhF38hrAJ2?compact=true&style=flat)](https://discord.com/invite/KhF38hrAJ2)\n\n<img src="./docs/1.png" align="center"/>\n\n🦋 Build complex chat apps using LLMs in 4 clicks ⚡️ [Try it out here](https://chainfury.nbox.ai/)\n\nChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs. \n\n[ChainFury- Create LLM ChatBots in 4 clicks!](https://medium.com/@chandranih/chainfury-create-llm-chatbots-in-4-clicks-3663538db8c6)\n\n[Why the Fury? Building a new flow engine from scratch](https://blog.nimblebox.ai/new-flow-engine-from-scratch)\n\nWith a simple GUI inspired by [LangFlow](https://github.com/logspace-ai/langflow), ChainFury enables you to chain components of [LangChain](https://github.com/hwchase17/langchain) together, allowing you to embed more complex chat applications with a simple JS snippet.\n\nChainFury supports a range of features, including but not limited to:\n\n- Recording all prompts and responses and storing them in a database\n- Collecting metrics like response latency\n- Querying OpenAI\'s API to obtain a rating for the response, which it stores in the database\n- Separate scoring mechanism per ChatBot to easily view performance in a dashboard\n- [Plugins](./server/plugins/) to extend the functionality of ChainFury with callbacks\n\n---\n\n<img src="./docs/2.png" align="center"/>\n\n---\nInstalling ChainFury is easy, with two methods available. We suggest using **the Docker method.**\n\n## Method 1: Docker\n\nThe easiest way to install ChainFury is to use Docker. You can use the following command to run ChainFury:\n\n```bash\ndocker build . -f Dockerfile -t chainfury:latest\n\ndocker run --env OPENAI_API_KEY=<your_key_here> -p 8000:8000 chainfury:latest\n```\n\nNow you can access the app on [localhost:8000](http://localhost:8000/ui/).\n\n<details>\n<summary>Optional environment variable for Database</summary>\nYou can also pass a Database URL to the docker container using the `DATABASE_URL` environment variable. If you do not pass a database URL, ChainFury will use a SQLite database.\n\nExample:\n\n```bash\ndocker run -it -E DATABASE_URL="mysql+pymysql://<user>:<password>@127.0.0.1:3306/<database>" -p 8000:8000 chainfury\n```\n</details>\n\n\n---\n## Method 2: Manual\n<details>\n<summary>For this, you will need to build the frontend and and then run the backend. The frontend can be built using the following command:</summary>\n\n```bash\ncd client\nyarn install\nyarn build\ncd ..\n```\n\nTo copy the frontend to the backend, run the following command:\n\n```bash\ncp -r client/dist/ server/static/\nmkdir -p ./server/templates\ncp ./client/dist/index.html ./server/templates/index.html\n```\n\nNow you can install the backend dependencies and run the server. We recommend using Python 3.9 virtual environment for this:\n\n```bash\npython3 -m venv venv\nsource venv/bin/activate\npip install -r requirements.txt\ncd server\npython3 -m uvicorn app:app --log-level=debug --host 0.0.0.0 --port 8000 --workers 1\n```\n</details>\n<!-- collapsable -->\n\n<details>\n<summary>How to run</summary>\n\nAssuming you are in `server` directory, you can run the server using the following command:\n\n```bash\npython3 server.py --port 8000 --config_plugins=\'["echo"]\'\n```\n</details>\n\nNow you can access the app on [localhost:8000](http://localhost:8000/ui/).\n\n---\n\n<img src="./docs/3.png" align="center"/>\n\n---\n\n1. Start the server by using the docker file provided or by using the manual method.\n\n2. Log into ChainFury by entering username = “admin” and password = “admin”\n\n3. Click on create chatbot\n\n4. Use one of the pre-configured chatbots or use the elements to create a custom chatbot.\n\n5. Save & create your chatbot and start chatting with it by clicking the chat on the bottom-right. You can see chatbot statistics and feedback metrics in your ChainFury dashboard.\n\n\n---\n\n<img src="./docs/5.png" align="center"/>\n\n---\n\nThere are six main areas that LangChain is designed to help with.\n\nChainFury consists of the same concepts to build LLM ChatBots. The components are, in increasing order of complexity:\n\n| Glossary | LangChain    | ChainFury    |\n| --- | --- | --- |\n| 📃 LLMs and Prompts | Prompt management, prompt optimization, generic interface for all LLMs, and common utilities for working with LLMs   | Easy prompt management with GUI elements\n| 🔗 Chains | Chains are sequences of calls (whether to an LLM or a different utility). LangChain provides a standard interface for chains, lots of integrations with other tools, and end-to-end chains for common applications | Easy chain management with GUI |\n| 📚 Data Augmented Generation | Data Augmented Generation involves specific types of chains that first interact with an external datasource to fetch data to use in the generation step. Examples of this include summarization of long pieces of text and question/answering over specific data sources | Coming soon |\n| 🤖 Agents | Agents involve an LLM making decisions about which Actions to take, taking that Action, seeing an Observation, and repeating that until done. LangChain provides a standard interface for agents, a selection of agents to choose from, and examples of end to end agents| Easy agent management with GUI |\n| 🧠 Memory | Memory is the concept of persisting state between calls of a chain/agent. LangChain provides a standard interface for memory, a collection of memory implementations, and examples of chains/agents that use memory | Memory modules are supported, persistant memory coming soon |\n| 🧐 Evaluation | [BETA] Generative models are notoriously hard to evaluate with traditional metrics. One new way of evaluating them is using language models themselves to do the evaluation. LangChain provides some prompts/chains for assisting in this | Auto evaluation of all prompts though OpenAI APIs |\n\n\n---\n\n<img src="./docs/4.png" align="center"/>\n\n---\nChainFury is an open-source project, and is currently in the alpha stage. We are open to contributions to the project in the form of features, infrastructure or documentation.\n\n- To contribute to this project, please follow a ["fork and pull request"](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) workflow. Please do not try to push directly to this repo unless you are maintainer.\n\n- Our [issues](https://github.com/NimbleBoxAI/ChainFury/issues) page is kept up to date with bugs, improvements, and feature requests.\n\n- If you\'re looking for help with your code, consider posting a question on the [GitHub Discussions board](https://github.com/NimbleBoxAI/ChainFury/discussions), so that more people can benefit from it.\n\n- **Describing your issue:** Try to provide as many details as possible. What exactly goes wrong? How is it failing? Is there an error? "XY doesn\'t work" usually isn\'t that helpful for tracking down problems. Always remember to include the code you ran and if possible, extract only the relevant parts and don\'t just dump your entire script. This will make it easier for us to reproduce the error.\n\n- **Sharing long blocks of code or logs:** If you need to include long code, logs or tracebacks, you can wrap them in `<details>` and `</details>`. This [collapses the content](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/details) so it only becomes visible on click, making the issue easier to read and follow.\n\n',
     'author': 'NimbleBox Engineering',
     'author_email': 'engineering@nimblebox.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/NimbleBoxAI/ChainFury',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `chainfury-0.1.1/PKG-INFO` & `chainfury-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: chainfury
-Version: 0.1.1
+Version: 1.2.0
 Summary: ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs.
 Home-page: https://github.com/NimbleBoxAI/ChainFury
 License: Apache V2.0
 Author: NimbleBox Engineering
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (==3.1.2)
 Requires-Dist: fire (==0.5.0)
 Requires-Dist: jinja2schema (==0.1.4)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/NimbleBoxAI/ChainFury
 Description-Content-Type: text/markdown
 
 # 🦋 ChainFury
 
 [![linkcheck](https://img.shields.io/badge/Workflow-Passing-darkgreen)](https://github.com/NimbleBoxAI/ChainFury/actions)
 [![Downloads](https://static.pepy.tech/badge/chainfury)](https://pepy.tech/project/chainfury)
@@ -29,14 +31,18 @@
 
 <img src="./docs/1.png" align="center"/>
 
 🦋 Build complex chat apps using LLMs in 4 clicks ⚡️ [Try it out here](https://chainfury.nbox.ai/)
 
 ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs. 
 
+[ChainFury- Create LLM ChatBots in 4 clicks!](https://medium.com/@chandranih/chainfury-create-llm-chatbots-in-4-clicks-3663538db8c6)
+
+[Why the Fury? Building a new flow engine from scratch](https://blog.nimblebox.ai/new-flow-engine-from-scratch)
+
 With a simple GUI inspired by [LangFlow](https://github.com/logspace-ai/langflow), ChainFury enables you to chain components of [LangChain](https://github.com/hwchase17/langchain) together, allowing you to embed more complex chat applications with a simple JS snippet.
 
 ChainFury supports a range of features, including but not limited to:
 
 - Recording all prompts and responses and storing them in a database
 - Collecting metrics like response latency
 - Querying OpenAI's API to obtain a rating for the response, which it stores in the database
@@ -79,20 +85,20 @@
 <details>
 <summary>For this, you will need to build the frontend and and then run the backend. The frontend can be built using the following command:</summary>
 
 ```bash
 cd client
 yarn install
 yarn build
+cd ..
 ```
 
 To copy the frontend to the backend, run the following command:
 
 ```bash
-cd ..
 cp -r client/dist/ server/static/
 mkdir -p ./server/templates
 cp ./client/dist/index.html ./server/templates/index.html
 ```
 
 Now you can install the backend dependencies and run the server. We recommend using Python 3.9 virtual environment for this:
```

