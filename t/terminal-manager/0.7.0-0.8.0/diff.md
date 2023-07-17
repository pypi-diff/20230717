# Comparing `tmp/terminal_manager-0.7.0.tar.gz` & `tmp/terminal_manager-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.7.0.tar", last modified: Sun Jul 16 06:08:01 2023, max compression
+gzip compressed data, was "terminal_manager-0.8.0.tar", last modified: Mon Jul 17 05:54:07 2023, max compression
```

## Comparing `terminal_manager-0.7.0.tar` & `terminal_manager-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.7.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.7.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-16 06:02:52.000000 terminal_manager-0.7.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:08:01.426293 terminal_manager-0.7.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/src/terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7058 2023-07-16 04:46:49.000000 terminal_manager-0.7.0/src/terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/collection.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5748 2023-07-16 04:40:07.000000 terminal_manager-0.7.0/src/terminal_manager/command.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/src/terminal_manager/default_collections/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/default_collections/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/default_collections/const.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4312 2023-07-16 04:02:15.000000 terminal_manager-0.7.0/src/terminal_manager/default_collections/linux.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-16 03:15:36.000000 terminal_manager-0.7.0/src/terminal_manager/default_collections/windows_cmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5374 2023-07-16 03:21:41.000000 terminal_manager-0.7.0/src/terminal_manager/default_collections/windows_ps.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/event.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/helpers.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8387 2023-07-16 04:39:12.000000 terminal_manager-0.7.0/src/terminal_manager/sensor.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/synchronizer.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/src/terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-16 06:08:01.000000 terminal_manager-0.7.0/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-16 06:08:01.000000 terminal_manager-0.7.0/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-16 06:08:01.000000 terminal_manager-0.7.0/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-16 06:08:01.000000 terminal_manager-0.7.0/src/terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-16 06:08:01.000000 terminal_manager-0.7.0/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 05:54:07.253274 terminal_manager-0.8.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.8.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-17 05:54:07.253274 terminal_manager-0.8.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.8.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-17 05:49:04.000000 terminal_manager-0.8.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-17 05:54:07.253274 terminal_manager-0.8.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 05:54:07.245274 terminal_manager-0.8.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 05:54:07.249274 terminal_manager-0.8.0/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     6982 2023-07-17 05:52:01.000000 terminal_manager-0.8.0/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     6322 2023-07-17 05:48:24.000000 terminal_manager-0.8.0/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 05:54:07.253274 terminal_manager-0.8.0/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4312 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5374 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/helpers.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8387 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-16 06:39:54.000000 terminal_manager-0.8.0/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 05:54:07.253274 terminal_manager-0.8.0/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-17 05:54:07.000000 terminal_manager-0.8.0/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-17 05:54:07.000000 terminal_manager-0.8.0/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-17 05:54:07.000000 terminal_manager-0.8.0/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-17 05:54:07.000000 terminal_manager-0.8.0/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-17 05:54:07.000000 terminal_manager-0.8.0/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.7.0/LICENSE` & `terminal_manager-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.7.0/PKG-INFO` & `terminal_manager-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: terminal_manager
-Version: 0.7.0
+Version: 0.8.0
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Terminal Manager
 
 ## Initialize
```

### Comparing `terminal_manager-0.7.0/pyproject.toml` & `terminal_manager-0.8.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.7.0"
+version = "0.8.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor devices"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
-  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 keywords = [ 
   "terminal", 
   "command line",
 ]
```

### Comparing `terminal_manager-0.7.0/src/terminal_manager/__init__.py` & `terminal_manager-0.8.0/src/terminal_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Terminal manager."""
 from __future__ import annotations
 
 import logging
 from collections.abc import Sequence
 from dataclasses import dataclass
-from time import time
 from typing import Any
 
 from .collection import Collection
 from .command import ActionCommand, Command, SensorCommand
 from .default_collections import ActionKey, SensorKey
 from .errors import CommandError
 from .event import Event
@@ -120,15 +119,15 @@
         self, command: Command, variables: dict | None = None
     ) -> CommandOutput:
         """Execute a command.
 
         Raises:
             CommandError
         """
-        await command.async_execute(self, variables)
+        return await command.async_execute(self, variables)
 
     async def async_run_action(
         self, key: str, variables: dict | None = None
     ) -> CommandOutput:
         """Run an action.
 
         Raises:
@@ -202,30 +201,26 @@
                 await sensor.async_set(self, values[i])
             except (TypeError, ValueError, CommandError):
                 if raise_errors:
                     raise
 
         return await self.async_poll_sensors(keys, raise_errors=raise_errors)
 
-    async def async_turn_off(self) -> None:
+    async def async_turn_off(self) -> CommandOutput:
         """Turn off by running the `TURN_OFF` action.
 
         Raises:
+            PermissionError
             CommandError
         """
-        if not (
-            ActionKey.TURN_OFF in self.action_commands_by_key and self.allow_turn_off
-        ):
-            return
+        if not self.allow_turn_off:
+            raise PermissionError("Not allowed to turn off")
 
-        await self.async_run_action(ActionKey.TURN_OFF)
+        return await self.async_run_action(ActionKey.TURN_OFF)
 
-    async def async_restart(self) -> None:
+    async def async_restart(self) -> CommandOutput:
         """Restart by running the `RESTART` action.
 
         Raises:
             CommandError
         """
-        if not ActionKey.RESTART in self.action_commands_by_key:
-            return
-
-        await self.async_run_action(ActionKey.RESTART)
+        return await self.async_run_action(ActionKey.RESTART)
```

### Comparing `terminal_manager-0.7.0/src/terminal_manager/collection.py` & `terminal_manager-0.8.0/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.7.0/src/terminal_manager/command.py` & `terminal_manager-0.8.0/src/terminal_manager/command.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from dataclasses import KW_ONLY, dataclass, field
-from string import Formatter, Template
+from string import Template
 from time import time
 from typing import TYPE_CHECKING
 
 from .errors import CommandError
 from .helpers import name_to_key
 from .sensor import Sensor
 
@@ -15,14 +15,31 @@
 
 SENSOR_DELIMITER = "@sensor"
 VARIABLE_DELIMITER = "@variable"
 SHORTCUTS = ["id", "value"]
 PLACEHOLDER_KEY = "_"
 
 
+# Not needed anymore after python 3.11
+class Template(Template):
+    def get_identifiers(self):
+        ids = []
+        for mo in self.pattern.finditer(self.template):
+            named = mo.group("named") or mo.group("braced")
+            if named is not None and named not in ids:
+                ids.append(named)
+            elif (
+                named is None
+                and mo.group("invalid") is None
+                and mo.group("escaped") is None
+            ):
+                raise ValueError("Unrecognized named group in pattern", self.pattern)
+        return ids
+
+
 class SensorTemplate(Template):
     delimiter = SENSOR_DELIMITER
 
 
 class VariableTemplate(Template):
     delimiter = VARIABLE_DELIMITER
```

### Comparing `terminal_manager-0.7.0/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.8.0/src/terminal_manager/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.7.0/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.8.0/src/terminal_manager/default_collections/linux.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.7.0/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.8.0/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.7.0/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.8.0/src/terminal_manager/default_collections/windows_ps.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.7.0/src/terminal_manager/event.py` & `terminal_manager-0.8.0/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.7.0/src/terminal_manager/sensor.py` & `terminal_manager-0.8.0/src/terminal_manager/sensor.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.7.0/src/terminal_manager/synchronizer.py` & `terminal_manager-0.8.0/src/terminal_manager/synchronizer.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.7.0/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.8.0/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: terminal-manager
-Version: 0.7.0
+Version: 0.8.0
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Terminal Manager
 
 ## Initialize
```

### Comparing `terminal_manager-0.7.0/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.8.0/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

