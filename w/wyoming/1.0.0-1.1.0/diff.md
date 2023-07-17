# Comparing `tmp/wyoming-1.0.0.tar.gz` & `tmp/wyoming-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming-1.0.0.tar", last modified: Tue Jul 11 22:14:33 2023, max compression
+gzip compressed data, was "wyoming-1.1.0.tar", last modified: Mon Jul 17 16:09:05 2023, max compression
```

## Comparing `wyoming-1.0.0.tar` & `wyoming-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-11 22:14:33.807593 wyoming-1.0.0/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      674 2023-07-11 22:14:33.807593 wyoming-1.0.0/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-11 22:14:33.807593 wyoming-1.0.0/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      879 2023-07-11 22:14:33.000000 wyoming-1.0.0/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-11 22:14:33.807593 wyoming-1.0.0/wyoming/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       40 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1586 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/asr.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5718 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/audio.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1938 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/client.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4104 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/event.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1283 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/handle.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3066 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/info.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2692 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/intent.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4358 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/server.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      428 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/snd.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2038 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/tts.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-11 22:14:33.807593 wyoming-1.0.0/wyoming/util/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/util/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2192 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/util/dataclasses_json.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1263 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/vad.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1293 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming/wake.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-11 22:14:33.807593 wyoming-1.0.0/wyoming.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      674 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      408 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        8 2023-07-11 22:14:33.000000 wyoming-1.0.0/wyoming.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:09:05.633287 wyoming-1.1.0/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      674 2023-07-17 16:09:05.633287 wyoming-1.1.0/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-17 16:09:05.633287 wyoming-1.1.0/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      879 2023-07-17 16:09:05.000000 wyoming-1.1.0/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:09:05.633287 wyoming-1.1.0/wyoming/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       40 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1586 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/asr.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5718 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/audio.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1938 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/client.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5439 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/event.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1283 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/handle.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3066 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/info.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2692 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/intent.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4363 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/server.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      428 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/snd.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2038 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/tts.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:09:05.633287 wyoming-1.1.0/wyoming/util/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/util/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2352 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/util/dataclasses_json.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1263 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/vad.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1293 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming/wake.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:09:05.633287 wyoming-1.1.0/wyoming.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      674 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      408 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        8 2023-07-17 16:09:05.000000 wyoming-1.1.0/wyoming.egg-info/top_level.txt
```

### Comparing `wyoming-1.0.0/PKG-INFO` & `wyoming-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wyoming
-Version: 1.0.0
+Version: 1.1.0
 Summary: Protocol for Rhasspy Voice Assistant
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Description: UNKNOWN
 Keywords: voice assistant rhasspy
```

### Comparing `wyoming-1.0.0/setup.py` & `wyoming-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 from setuptools import setup
 
 # -----------------------------------------------------------------------------
 
 setup(
     name="wyoming",
-    version="1.0.0",
+    version="1.1.0",
     description="Protocol for Rhasspy Voice Assistant",
     url="http://github.com/rhasspy/rhasspy3",
     author="Michael Hansen",
     author_email="mike@rhasspy.org",
     license="MIT",
     packages=["wyoming", "wyoming.util"],
     classifiers=[
```

### Comparing `wyoming-1.0.0/wyoming/asr.py` & `wyoming-1.1.0/wyoming/asr.py`

 * *Files identical despite different names*

### Comparing `wyoming-1.0.0/wyoming/audio.py` & `wyoming-1.1.0/wyoming/audio.py`

 * *Files identical despite different names*

### Comparing `wyoming-1.0.0/wyoming/client.py` & `wyoming-1.1.0/wyoming/client.py`

 * *Files identical despite different names*

### Comparing `wyoming-1.0.0/wyoming/event.py` & `wyoming-1.1.0/wyoming/event.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 import sys
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any, BinaryIO, Dict, Iterable, Optional
 
 _TYPE = "type"
 _DATA = "data"
+_DATA_LENGTH = "data_length"
 _PAYLOAD_LENGTH = "payload_length"
 _NEWLINE = "\n".encode()
+_VERSION = "version"
+_VERSION_NUMBER = "1.1"
 
 
 @dataclass
 class Event:
     type: str
     data: Dict[str, Any] = field(default_factory=dict)
     payload: Optional[bytes] = None
@@ -57,64 +60,69 @@
 async def async_read_event(reader: asyncio.StreamReader) -> Optional[Event]:
     try:
         json_line = await reader.readline()
         if not json_line:
             return None
 
         event_dict = json.loads(json_line)
+        data_length = event_dict.get(_DATA_LENGTH)
+        if (data_length is not None) and (data_length > 0):
+            # Merge data
+            data_bytes = await reader.readexactly(data_length)
+            data_dict = event_dict.get(_DATA, {})
+            data_dict.update(json.loads(data_bytes))
+            event_dict[_DATA] = data_dict
+
         payload_length = event_dict.get(_PAYLOAD_LENGTH)
 
         payload: Optional[bytes] = None
-        if payload_length is not None:
+        if (payload_length is not None) and (payload_length > 0):
             payload = await reader.readexactly(payload_length)
 
         return Event(
             type=event_dict[_TYPE], data=event_dict.get(_DATA), payload=payload
         )
     except (KeyboardInterrupt, ValueError):
         pass
 
     return None
 
 
 async def async_write_event(event: Event, writer: asyncio.StreamWriter):
     event_dict: Dict[str, Any] = event.to_dict()
+    event_dict[_VERSION] = _VERSION_NUMBER
+
+    data_dict = event_dict.pop(_DATA, None)
+    data_bytes: Optional[bytes] = None
+    if data_dict:
+        data_bytes = json.dumps(data_dict, ensure_ascii=False).encode("utf-8")
+        event_dict[_DATA_LENGTH] = len(data_bytes)
+
     if event.payload:
         event_dict[_PAYLOAD_LENGTH] = len(event.payload)
 
     json_line = json.dumps(event_dict, ensure_ascii=False)
 
     try:
         writer.writelines((json_line.encode(), _NEWLINE))
 
+        if data_bytes:
+            writer.write(data_bytes)
+
         if event.payload:
             writer.write(event.payload)
 
         await writer.drain()
     except KeyboardInterrupt:
         pass
 
 
 async def async_write_events(events: Iterable[Event], writer: asyncio.StreamWriter):
-    coros = []
-    for event in events:
-        event_dict: Dict[str, Any] = event.to_dict()
-        if event.payload:
-            event_dict[_PAYLOAD_LENGTH] = len(event.payload)
-
-        json_line = json.dumps(event_dict, ensure_ascii=False)
-        writer.writelines((json_line.encode(), _NEWLINE))
-
-        if event.payload:
-            writer.write(event.payload)
-
-        coros.append(writer.drain())
-
     try:
-        await asyncio.gather(*coros)
+        await asyncio.gather(*(async_write_event(event, writer) for event in events))
     except KeyboardInterrupt:
         pass
 
 
 def read_event(reader: Optional[BinaryIO] = None) -> Optional[Event]:
     if reader is None:
         reader = sys.stdin.buffer
@@ -122,19 +130,32 @@
     try:
         json_line = reader.readline()
 
         if not json_line:
             return None
 
         event_dict = json.loads(json_line)
+        data_length = event_dict.get(_DATA_LENGTH)
+        if (data_length is not None) and (data_length > 0):
+            # Merge data
+            data_bytes = reader.read(data_length)
+            while len(data_bytes) < data_length:
+                data_bytes += reader.read(data_length - len(data_bytes))
+
+            data_dict = event_dict.get(_DATA, {})
+            data_dict.update(json.loads(data_bytes))
+            event_dict[_DATA] = data_dict
+
         payload_length = event_dict.get(_PAYLOAD_LENGTH)
 
         payload: Optional[bytes] = None
         if payload_length is not None:
             payload = reader.read(payload_length)
+            while len(payload) < payload_length:
+                payload += reader.read(payload_length - len(payload))
 
         return Event(
             type=event_dict[_TYPE], data=event_dict.get(_DATA), payload=payload
         )
     except (KeyboardInterrupt, ValueError):
         pass
 
@@ -142,21 +163,32 @@
 
 
 def write_event(event: Event, writer: Optional[BinaryIO] = None):
     if writer is None:
         writer = sys.stdout.buffer
 
     event_dict: Dict[str, Any] = event.to_dict()
+    event_dict[_VERSION] = _VERSION_NUMBER
+
+    data_dict = event_dict.pop(_DATA, None)
+    data_bytes: Optional[bytes] = None
+    if data_dict:
+        data_bytes = json.dumps(data_dict, ensure_ascii=False).encode("utf-8")
+        event_dict[_DATA_LENGTH] = len(data_bytes)
+
     if event.payload:
         event_dict[_PAYLOAD_LENGTH] = len(event.payload)
 
     json_line = json.dumps(event_dict, ensure_ascii=False)
 
     try:
         writer.writelines((json_line.encode(), _NEWLINE))
 
+        if data_bytes:
+            writer.write(data_bytes)
+
         if event.payload:
             writer.write(event.payload)
 
         writer.flush()
     except KeyboardInterrupt:
         pass
```

### Comparing `wyoming-1.0.0/wyoming/handle.py` & `wyoming-1.1.0/wyoming/handle.py`

 * *Files identical despite different names*

### Comparing `wyoming-1.0.0/wyoming/info.py` & `wyoming-1.1.0/wyoming/info.py`

 * *Files identical despite different names*

### Comparing `wyoming-1.0.0/wyoming/intent.py` & `wyoming-1.1.0/wyoming/intent.py`

 * *Files identical despite different names*

### Comparing `wyoming-1.0.0/wyoming/server.py` & `wyoming-1.1.0/wyoming/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import sys
 from abc import ABC, abstractmethod
 from functools import partial
 from pathlib import Path
 from typing import Callable, Set, Union
+from urllib.parse import urlparse
 
 from .event import Event, async_get_stdin, async_read_event, async_write_event
 
 
 class AsyncEventHandler(ABC):
     """Base class for async Wyoming event handler."""
 
@@ -53,24 +54,25 @@
 
     @abstractmethod
     async def run(self, handler_factory: HandlerFactory) -> None:
         pass
 
     @staticmethod
     def from_uri(uri: str) -> "AsyncServer":
-        if uri.startswith("unix://"):
-            socket_path = uri[len("unix://") :]
-            return AsyncUnixServer(socket_path)
+        result = urlparse(uri)
 
-        if uri.startswith("tcp://"):
-            host, port_str = uri[len("tcp://") :].split(":")
+        if result.scheme == "unix":
+            return AsyncUnixServer(result.path)
+
+        if result.scheme == "tcp":
+            host, port_str = result.netloc.split(":")
             port = int(port_str)
             return AsyncTcpServer(host, port)
 
-        if uri.startswith("stdio://"):
+        if result.scheme == "stdio":
             return AsyncStdioServer()
 
         raise ValueError("Only 'stdio://', 'unix://', or 'tcp://' are supported")
 
     async def _handler_callback(
         self,
         handler_factory: HandlerFactory,
```

### Comparing `wyoming-1.0.0/wyoming/tts.py` & `wyoming-1.1.0/wyoming/tts.py`

 * *Files identical despite different names*

### Comparing `wyoming-1.0.0/wyoming/util/dataclasses_json.py` & `wyoming-1.1.0/wyoming/util/dataclasses_json.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> Any:
         """Parse dataclasses recursively."""
         kwargs: Dict[str, Any] = {}
 
         cls_fields = {field.name: field for field in fields(cls)}
         for key, value in data.items():
+            if key not in cls_fields:
+                # Skip unknown fields
+                continue
+
             field = cls_fields[key]
             if is_dataclass(field.type):
                 assert issubclass(field.type, DataClassJsonMixin), field.type
                 kwargs[key] = field.type.from_dict(value)
             else:
                 kwargs[key] = _decode(value, field.type)
 
-        # Fill in optional fields
+        # Fill in optional fields with None
         for field in cls_fields.values():
-            if (
-                (field.name not in kwargs)
-                and hasattr(field.type, "__args__")
-                and (type(None) in field.type.__args__)
-            ):
+            if (field.name not in kwargs) and _is_optional(field.type):
                 kwargs[field.name] = None
 
         return cls(**kwargs)
 
     def to_dict(self) -> Dict[str, Any]:
         """Alias for asdict."""
         return asdict(self)
@@ -59,7 +59,12 @@
             value_type = target_type.__args__[1]
             return {
                 map_key: _decode(map_value, value_type)
                 for map_key, map_value in value.items()
             }
 
     return value
+
+
+def _is_optional(target_type: Type):
+    """True if type is Optional"""
+    return hasattr(target_type, "__args__") and (type(None) in target_type.__args__)
```

### Comparing `wyoming-1.0.0/wyoming/vad.py` & `wyoming-1.1.0/wyoming/vad.py`

 * *Files identical despite different names*

### Comparing `wyoming-1.0.0/wyoming/wake.py` & `wyoming-1.1.0/wyoming/wake.py`

 * *Files identical despite different names*

### Comparing `wyoming-1.0.0/wyoming.egg-info/PKG-INFO` & `wyoming-1.1.0/wyoming.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wyoming
-Version: 1.0.0
+Version: 1.1.0
 Summary: Protocol for Rhasspy Voice Assistant
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Description: UNKNOWN
 Keywords: voice assistant rhasspy
```

