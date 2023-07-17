# Comparing `tmp/idem-random-0.2.1.tar.gz` & `tmp/idem-random-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-random-0.2.1.tar", last modified: Thu Jul  6 02:24:42 2023, max compression
+gzip compressed data, was "idem-random-1.0.0.tar", last modified: Mon Jul 17 15:16:07 2023, max compression
```

## Comparing `idem-random-0.2.1.tar` & `idem-random-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/
--rw-r--r--   0 root         (0) root         (0)    11329 2023-07-06 02:24:27.000000 idem-random-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3713 2023-07-06 02:24:42.512631 idem-random-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2912 2023-07-06 02:24:27.000000 idem-random-0.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/
--rw-r--r--   0 root         (0) root         (0)     1293 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/exec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/exec/random/
--rw-r--r--   0 root         (0) root         (0)     2049 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/exec/random/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/idem_random/
--rw-r--r--   0 root         (0) root         (0)      836 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/idem_random/init.py
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/states/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/states/random/
--rw-r--r--   0 root         (0) root         (0)     4968 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/states/random/id.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/states/random/integer.py
--rw-r--r--   0 root         (0) root         (0)     7323 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/states/random/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/tool/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/tool/random/
--rw-r--r--   0 root         (0) root         (0)      864 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/tool/random/id.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 02:24:41.000000 idem-random-0.2.1/idem_random/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3713 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      597 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 02:24:42.512631 idem-random-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2766 2023-07-06 02:24:27.000000 idem-random-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11329 2023-07-17 15:15:53.000000 idem-random-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-07-17 15:16:07.088203 idem-random-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-17 15:15:53.000000 idem-random-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/exec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/exec/random/
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/exec/random/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/idem_random/
+-rw-r--r--   0 root         (0) root         (0)      836 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/idem_random/init.py
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/states/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/states/random/
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/states/random/id.py
+-rw-r--r--   0 root         (0) root         (0)     5571 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/states/random/integer.py
+-rw-r--r--   0 root         (0) root         (0)     7290 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/states/random/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/tool/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/tool/random/
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/tool/random/id.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 15:16:06.000000 idem-random-1.0.0/idem_random/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      597 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 15:16:07.088203 idem-random-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-07-17 15:15:53.000000 idem-random-1.0.0/setup.py
```

### Comparing `idem-random-0.2.1/LICENSE` & `idem-random-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.1/PKG-INFO` & `idem-random-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-random
-Version: 0.2.1
+Version: 1.0.0
 Summary: Idem plugin for providing randomness
 Home-page: UNKNOWN
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-random-0.2.1/README.rst` & `idem-random-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.1/idem_random/conf.py` & `idem-random-1.0.0/idem_random/conf.py`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.1/idem_random/idem_random/init.py` & `idem-random-1.0.0/idem_random/idem_random/init.py`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.1/idem_random/states/random/id.py` & `idem-random-1.0.0/idem_random/states/random/id.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,68 @@
+"""State module for generating ids"""
 from typing import Any
 from typing import Dict
 
 import dict_tools.differ as differ
 
 
-async def present(
+def present(
     hub,
     ctx,
     name: str,
     length: int,
     resource_id: str = None,
     keepers: Dict[str, Any] = None,
     prefix: str = None,
 ) -> Dict[str, Any]:
     r"""
     This is a logical state and doesn't interact with any cloud providers.
     This state can be used in conjunction with any other state to generate
     random id with the provided configurations. State's configuration
-    data is stored in esm. If for a given state , the configuration changes
-    , a new random id is generated. If there are no configuration changes
-    , then the old id is retained.
+    data is stored in esm. If for a given state, the configuration changes,
+    a new random id is generated. If there are no configuration changes,
+    then the old id is retained.
+
+    The generated id is alphanumeric, starting with a letter.
 
     Args:
-        name(Text): An Idem name of the resource.
-        length(Integer): The number of random bytes to produce.
+        name(str): An Idem name of the resource.
+        length(int): The number of random characters to produce.
         resource_id(str, Optional): Unique random Id
-        keepers(Dict, optional): A list of arbitrary map of values that,
-            when changed, will trigger recreation of resource.
-        prefix(Text, optional): Arbitrary string to prefix the output value with. This string is supplied as-is, meaning
-            it is not guaranteed to be URL-safe or base64 encoded.
+        keepers(dict, Optional): A list of arbitrary map of values that,
+          when changed, will trigger recreation of resource.
+        prefix(str, Optional): Arbitrary string to prefix the output value with. This string is supplied as-is, meaning
+          it is not guaranteed to be URL-safe or base64 encoded.
 
     Request Syntax:
-        [random_id_state]:
-          random.id.present:
+
+    .. code-block:: sls
+
+      [random_id_state]:
+        random.id.present:
           - name: 'string'
           - length: 'int'
           - keepers:
-             'string': 'string'
+              'string': 'string'
           - prefix: 'string'
 
     Returns:
         Dict[str, Any]
 
-    Examples:
+    Example:
 
-        .. code-block:: sls
+    .. code-block:: sls
 
-            random_passwd_state:
-                random.id.present:
-                    - name: random_id
-                    - length: 2
-                    - keepers:
-                         name: random_id
-                    - prefix: random_prefix
+      random_passwd_state:
+        random.id.present:
+          - name: random_id
+          - length: 2
+          - keepers:
+              name: random_id
+          - prefix: random_prefix
     """
 
     result = dict(comment=[], old_state=None, new_state=None, name=name, result=True)
     config_map = dict(
         keepers=keepers,
         length=length,
         prefix=prefix,
@@ -67,14 +73,17 @@
             "config_map": config_map,
             "name": name,
             "output": resource_id,
             "resource_id": resource_id,
         }
         return result
 
+    if prefix is None:
+        prefix = ""
+
     before = ctx.get("old_state")
     if before:
         result["old_state"] = before
         config_map_old = before.get("config_map", {})
         config_map_new = config_map
 
         result["changes"] = differ.deep_diff(config_map_old, config_map_new)
@@ -89,17 +98,15 @@
                 "output": None,
             }
             if ctx.get("test"):
                 result["comment"].append(f"Would generate new random.random.id.")
 
                 return result
 
-            ret = hub.tool.random.id.generate_random_string(
-                length=length, prefix=prefix
-            )
+            ret = prefix + hub.tool.random.id.generate_random_id(length=length)
 
             result["new_state"]["output"] = ret
             result["comment"].append(f"Generated new random.random.id '{name}'.")
         else:
             result["comment"].append(
                 f"No config change detected for '{name}'. Old ID will be retained."
             )
@@ -113,51 +120,52 @@
             "name": name,
             "output": None,
         }
         if ctx.get("test"):
             result["comment"].append(f"Would generate random.random.id '{name}'.")
             return result
 
-        ret = hub.tool.random.id.generate_random_string(length=length, prefix=prefix)
+        ret = prefix + hub.tool.random.id.generate_random_id(length=length)
 
         result["new_state"]["output"] = ret
         result["new_state"]["resource_id"] = ret
         result["comment"].append(f"random.random.id '{name}' generated.")
     return result
 
 
-async def absent(
+def absent(
     hub,
     ctx,
     name: str,
 ) -> Dict[str, Any]:
 
     r"""
-
     This logical state is used to invalidate/delete the id.
 
     Args:
-        name(Text): An Idem name of the resource.
+        name(str): An Idem name of the resource.
 
     Request Syntax:
-        [random_id_state]:
-          random.id.present:
+
+    .. code-block:: sls
+
+      [random_id_state]:
+        random.id.absent:
           - name: 'string'
 
     Returns:
         Dict[str, Any]
 
-    Examples:
-
-        .. code-block:: sls
+    Example:
 
-            random_state01011:
-                random.id.absent:
-                    - name: rs01011
+    .. code-block:: sls
 
+      random_state01011:
+        random.id.absent:
+          - name: rs01011
     """
 
     result = dict(comment=[], old_state=None, new_state=None, name=name, result=True)
 
     before = ctx.get("old_state")
 
     result["old_state"] = before
```

### Comparing `idem-random-0.2.1/idem_random/states/random/integer.py` & `idem-random-1.0.0/idem_random/states/random/integer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+"""State module for generating random integers"""
 import copy
 import random
 from typing import Any
 from typing import Dict
 
 import dict_tools.differ as differ
 
 
-async def present(
+def present(
     hub,
     ctx,
     name: str,
     min: int,
     max: int,
     resource_id: int = None,
     keepers: Dict[str, Any] = None,
@@ -33,44 +34,47 @@
 
         max(int):
             The maximum inclusive value of the range.
 
         resource_id(int, Optional):
             Unique random Integer
 
-        keepers(Dict, Optional):
+        keepers(dict, Optional):
             Arbitrary map of values that, when changed, will trigger recreation of resource.
 
         seed(str, Optional):
             A custom seed to always produce the same value.
 
     Request Syntax:
-        [random_integer_state]:
-          random.integer.present:
+
+    .. code-block:: sls
+
+      [random_integer_state]:
+        random.integer.present:
           - name: 'string'
           - keepers:
-             'string': 'string'
+              'string': 'string'
           - min: 'int'
           - max: 'int'
           - seed: 'string'
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
-        .. code-block:: sls
+    .. code-block:: sls
 
-            random_integer_state:
-                random.integer.present:
-                    - name: random_integer
-                    - min: 0
-                    - max: 9
-                    - keepers:
-                         key: value
+      random_integer_state:
+        random.integer.present:
+          - name: random_integer
+          - min: 0
+          - max: 9
+          - keepers:
+              key: value
     """
 
     result = dict(comment=[], old_state=None, new_state=None, name=name, result=True)
     params = dict(
         min=min,
         max=max,
         seed=seed,
@@ -110,16 +114,24 @@
                 result["comment"].append(
                     f"Would generate new random.random.integer {name}."
                 )
 
                 return result
 
             if seed is not None:
-                random.seed(seed)
-            result["new_state"]["output"] = random.randint(min, max)
+                rand = random.Random(seed=seed)
+            else:
+                try:
+                    # prefer to use system random number generator
+                    rand = random.SystemRandom()
+                except NotImplementedError:
+                    # if that isn't available, fall back to pseudo-random number seeded by time
+                    rand = random.Random()
+
+            result["new_state"]["output"] = rand.randint(min, max)
             result["comment"].append(f"Generated new random.random.integer '{name}'.")
 
         else:
             result["comment"].append(
                 f"No config change detected for '{name}'. Old random integer will be retained."
             )
             result["new_state"] = copy.deepcopy(result["old_state"])
@@ -140,42 +152,44 @@
         result["new_state"]["output"] = random.randint(min, max)
         result["new_state"]["resource_id"] = result["new_state"]["output"]
         result["comment"].append(f"random.random.integer '{name}' generated.")
 
     return result
 
 
-async def absent(
+def absent(
     hub,
     ctx,
     name: str,
 ) -> Dict[str, Any]:
-
     r"""
 
     This logical state is used to invalidate/delete the random integer resource.
 
     Args:
-        name(Text): An Idem name of the resource.
+        name(str): An Idem name of the resource.
 
     Request Syntax:
-        [random_integer_state]:
-          random.integer.absent:
+
+    .. code-block:: sls
+
+      [random_integer_state]:
+        random.integer.absent:
           - name: 'string'
 
     Returns:
         Dict[str, Any]
 
-    Examples:
+    Example:
 
-        .. code-block:: sls
+    .. code-block:: sls
 
-            random_state01011:
-                random.integer.absent:
-                    - name: rs01011
+      random_state01011:
+        random.integer.absent:
+          - name: rs01011
 
     """
 
     result = dict(comment=[], old_state=None, new_state=None, name=name, result=True)
 
     before = ctx.get("old_state")
```

### Comparing `idem-random-0.2.1/idem_random/states/random/password.py` & `idem-random-1.0.0/idem_random/states/random/password.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+"""State module for generating random strings usable as passwords"""
 from typing import Any
 from typing import Dict
 
 import dict_tools.differ as differ
 
 
-async def present(
+def present(
     hub,
     ctx,
     name: str,
     length: int,
     resource_id: str = None,
     keepers: Dict[str, Any] = None,
     upper: bool = True,
@@ -38,72 +39,75 @@
 
         resource_id(str, Optional):
             Unique random password
 
         keepers(List, Optional):
             A list of arbitrary map of values that, when changed, will trigger recreation of resource.
 
-        lower(Boolean, Optional):
+        lower(bool, Optional):
             Include lowercase alphabet characters in the result. Default value is true.
 
         min_lower(int, Optional):
             Minimum number of lowercase alphabet characters in the result.Default value is 0.
 
         min_numeric(int, Optional):
             Minimum number of numeric characters in the result. Default value is 0.
 
         min_special(int, Optional):
             Minimum number of special characters in the result. efault value is 0.
 
         min_upper(int, Optional):
             Minimum number of uppercase alphabet characters in the result. Default value is 0.
 
-        numeric(Boolean, Optional):
+        numeric(bool, Optional):
             Include numeric characters in the result. Default value is true.
 
         override_special(str, Optional):
             Supply your own list of special characters to use for string generation. This overrides the default
             character list in the special argument. The special argument must still be set to true for any overwritten
             characters to be used in generation.
 
-        special(Boolean, Optional):
+        special(bool, Optional):
             Include special characters in the result. These are !@#$%&*()-_=+[]{}<>:?. Default value is true.
 
-        upper(Boolean, Optional):
+        upper(bool, Optional):
             Include uppercase alphabet characters in the result. Default value is true.
 
     Request Syntax:
-        [random_password_state]:
-          random.password.present:
+
+    .. code-block:: sls
+
+      [random_password_state]:
+        random.password.present:
           - name: 'string'
           - length: 'int'
           - keepers:
-             'string': 'string'
+              'string': 'string'
           - lower: 'boolean'
           - min_lower: 'int'
           - upper: 'boolean'
           - min_upper: 'int'
           - numeric: 'boolean'
           - min_numeric: 'int'
           - special: 'boolean'
           - override_special: 'string'
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
-        .. code-block:: sls
+    .. code-block:: sls
 
-            random_passwd_state:
-                random.password.present:
-                    - name: random_passwd
-                    - length: 13
-                    - keepers:
-                         key: value
+      random_passwd_state:
+        random.password.present:
+          - name: random_passwd
+          - length: 13
+          - keepers:
+              key: value
     """
 
     result = dict(comment=[], old_state=None, new_state=None, name=name, result=True)
     params = dict(
         upper=upper,
         min_upper=min_upper,
         lower=lower,
@@ -148,15 +152,15 @@
                 "output": None,
             }
             if ctx.get("test"):
                 result["comment"].append(f"Would generate new random.random.password.")
 
                 return result
 
-            ret = await hub.exec.random.password.generate_random_string(
+            ret = hub.exec.random.password.generate_random_string(
                 length=length, **params
             )
 
             if ret and ret["result"]:
                 result["new_state"]["output"] = ret["ret"]
                 result["comment"].append(
                     f"Generated new random.random.password '{name}'."
@@ -175,59 +179,60 @@
             "name": name,
             "output": None,
         }
         if ctx.get("test"):
             result["comment"].append(f"Would generate random.random.password '{name}'.")
             return result
 
-        ret = await hub.exec.random.password.generate_random_string(
-            length=length, **params
-        )
+        ret = hub.exec.random.password.generate_random_string(length=length, **params)
 
         if not ret or not ret["result"]:
             result["result"] = ret["result"]
             result["comment"].append(
                 f"Unable to generate random.random.password '{name}'."
             )
             return result
         result["new_state"]["output"] = ret["ret"]
         result["new_state"]["resource_id"] = result["new_state"]["output"]
         result["comment"].append(f"random.random.password '{name}' generated.")
 
     return result
 
 
-async def absent(
+def absent(
     hub,
     ctx,
     name: str,
 ) -> Dict[str, Any]:
 
     r"""
 
     This logical state is used to invalidate/delete the password.
 
     Args:
-        name(Text): An Idem name of the resource.
+        name(str): An Idem name of the resource.
 
     Request Syntax:
-        [random_password_state]:
-          random.password.present:
+
+    .. code-block:: sls
+
+      [random_password_state]:
+        random.password.absent:
           - name: 'string'
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
-        .. code-block:: sls
+    .. code-block:: sls
 
-            random_state01011:
-                random.password.absent:
-                    - name: rs01011
+      random_state01011:
+        random.password.absent:
+          - name: rs01011
 
     """
 
     result = dict(comment=[], old_state=None, new_state=None, name=name, result=True)
 
     before = ctx.get("old_state")
```

### Comparing `idem-random-0.2.1/idem_random.egg-info/PKG-INFO` & `idem-random-1.0.0/idem_random.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-random
-Version: 0.2.1
+Version: 1.0.0
 Summary: Idem plugin for providing randomness
 Home-page: UNKNOWN
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-random-0.2.1/idem_random.egg-info/SOURCES.txt` & `idem-random-1.0.0/idem_random.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.1/setup.py` & `idem-random-1.0.0/setup.py`

 * *Files identical despite different names*

