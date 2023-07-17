# Comparing `tmp/androidtvremote2-0.0.8.tar.gz` & `tmp/androidtvremote2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androidtvremote2-0.0.8.tar", last modified: Thu May  4 11:44:10 2023, max compression
+gzip compressed data, was "androidtvremote2-0.0.9.tar", last modified: Sat May 27 00:09:13 2023, max compression
```

## Comparing `androidtvremote2-0.0.8.tar` & `androidtvremote2-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:10.218464 androidtvremote2-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/src/androidtvremote2/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15577 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/androidtv_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/certificate_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/polo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    19528 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/remotemessage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-04 11:44:10.000000 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 11:44:10.000000 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:44:10.000000 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 11:44:10.000000 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 11:44:10.000000 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/tests/test_androidtv_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:09:13.197309 androidtvremote2-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-27 00:09:13.197309 androidtvremote2-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-27 00:09:13.197309 androidtvremote2-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:09:13.193309 androidtvremote2-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:09:13.193309 androidtvremote2-0.0.9/src/androidtvremote2/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/androidtv_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/certificate_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/polo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19528 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/remotemessage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:09:13.197309 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-27 00:09:13.000000 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-27 00:09:13.000000 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:09:13.000000 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-27 00:09:13.000000 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 00:09:13.000000 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:09:13.197309 androidtvremote2-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/tests/test_androidtv_remote.py
```

### Comparing `androidtvremote2-0.0.8/LICENSE` & `androidtvremote2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.8/PKG-INFO` & `androidtvremote2-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: androidtvremote2
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for interacting with Android TV using the Android TV Remote protocol v2
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/androidtvremote2
 Project-URL: Bug Tracker, https://github.com/tronikos/androidtvremote2/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `androidtvremote2-0.0.8/README.md` & `androidtvremote2-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.8/pyproject.toml` & `androidtvremote2-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "androidtvremote2"
-version = "0.0.8"
+version = "0.0.9"
 license = {text = "Apache-2.0"}
 authors = [
     { name="tronikos", email="tronikos@gmail.com" },
 ]
 description = "A Python library for interacting with Android TV using the Android TV Remote protocol v2"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -59,21 +59,21 @@
     "UP",  # pyupgrade
     "W",  # pycodestyle
 ]
 
 ignore = [
     "D203",  # 1 blank line required before class docstring
     "D213",  # Multi-line docstring summary should start at the second line
+    # keep-runtime-annotations
+    'UP006', # Non PEP585 annotations
+    'UP007', # Non PEP604 annotations
 ]
 
 [tool.ruff.flake8-pytest-style]
 fixture-parentheses = false
 
-[tool.ruff.pyupgrade]
-keep-runtime-typing = true
-
 [tool.ruff.per-file-ignores]
 # Allow for demo script to write to stdout
 "demo.py" = ["T201"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
```

### Comparing `androidtvremote2-0.0.8/src/androidtvremote2/androidtv_remote.py` & `androidtvremote2-0.0.9/src/androidtvremote2/androidtv_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         self._api_port = api_port
         self._pair_port = pair_port
         self._loop = loop or asyncio.get_running_loop()
         self._transport = None
         self._remote_message_protocol: RemoteProtocol | None = None
         self._pairing_message_protocol: PairingProtocol | None = None
         self._reconnect_task: asyncio.Task | None = None
+        self._ssl_context: ssl.SSLContext | None = None
         self._is_on_updated_callbacks: list[Callable] = []
         self._current_app_updated_callbacks: list[Callable] = []
         self._volume_info_updated_callbacks: list[Callable] = []
         self._is_available_updated_callbacks: list[Callable] = []
 
         def is_on_updated(is_on: bool):
             for callback in self._is_on_updated_callbacks:
@@ -167,20 +168,21 @@
     async def async_connect(self):
         """Connect to an Android TV.
 
         :raises CannotConnect: if couldn't connect, e.g. invalid IP address.
         :raises ConnectionClosed: if connection was lost while waiting for the remote to start.
         :raises InvalidAuth: if pairing is needed first.
         """
-        ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
-        try:
-            ssl_context.load_cert_chain(self._certfile, self._keyfile)
-        except FileNotFoundError as exc:
-            LOGGER.debug("Missing certificate. Error: %s", exc)
-            raise InvalidAuth from exc
+        if self._ssl_context is None:
+            self._ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+            try:
+                self._ssl_context.load_cert_chain(self._certfile, self._keyfile)
+            except FileNotFoundError as exc:
+                LOGGER.debug("Missing certificate. Error: %s", exc)
+                raise InvalidAuth from exc
         on_con_lost = self._loop.create_future()
         on_remote_started = self._loop.create_future()
         try:
             (
                 self._transport,
                 self._remote_message_protocol,
             ) = await self._loop.create_connection(
@@ -190,15 +192,15 @@
                     self._on_is_on_updated,
                     self._on_current_app_updated,
                     self._on_volume_info_updated,
                     self._loop,
                 ),
                 self.host,
                 self._api_port,
-                ssl=ssl_context,
+                ssl=self._ssl_context,
             )
         except OSError as exc:
             LOGGER.debug(
                 "Couldn't connect to %s:%s. Error: %s", self.host, self._api_port, exc
             )
             raise CannotConnect(
                 f"Couldn't connect to {self.host}:{self._api_port}"
@@ -233,15 +235,15 @@
             while self._remote_message_protocol:
                 await asyncio.sleep(delay_seconds)
                 try:
                     await self.async_connect()
                     self._on_is_available_updated(True)
                     break
                 except CannotConnect as exc:
-                    delay_seconds = min(2 * delay_seconds, 300)
+                    delay_seconds = min(2 * delay_seconds, 30)
                     LOGGER.debug(
                         "Couldn't reconnect to %s. Will retry in %s seconds. Error: %s",
                         self.host,
                         delay_seconds,
                         exc,
                     )
                 except InvalidAuth as exc:
@@ -274,15 +276,15 @@
             self._pairing_message_protocol = None
 
     async def async_get_name_and_mac(self) -> tuple[str, str]:
         """Connect to the Android TV and get its name and MAC address from its certificate.
 
         :raises CannotConnect: if couldn't connect, e.g. invalid IP address.
         """
-        ssl_context = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
+        ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
         try:
             _, writer = await asyncio.open_connection(
                 self.host, self._api_port, ssl=ssl_context
             )
         except OSError as exc:
             LOGGER.debug(
                 "Couldn't connect to %s:%s. %s", self.host, self._api_port, exc
```

### Comparing `androidtvremote2-0.0.8/src/androidtvremote2/base.py` & `androidtvremote2-0.0.9/src/androidtvremote2/base.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.8/src/androidtvremote2/certificate_generator.py` & `androidtvremote2-0.0.9/src/androidtvremote2/certificate_generator.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.8/src/androidtvremote2/pairing.py` & `androidtvremote2-0.0.9/src/androidtvremote2/pairing.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.8/src/androidtvremote2/polo_pb2.py` & `androidtvremote2-0.0.9/src/androidtvremote2/polo_pb2.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.8/src/androidtvremote2/remote.py` & `androidtvremote2-0.0.9/src/androidtvremote2/remote.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.8/src/androidtvremote2/remotemessage_pb2.py` & `androidtvremote2-0.0.9/src/androidtvremote2/remotemessage_pb2.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.8/src/androidtvremote2.egg-info/PKG-INFO` & `androidtvremote2-0.0.9/src/androidtvremote2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: androidtvremote2
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for interacting with Android TV using the Android TV Remote protocol v2
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/androidtvremote2
 Project-URL: Bug Tracker, https://github.com/tronikos/androidtvremote2/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `androidtvremote2-0.0.8/src/androidtvremote2.egg-info/SOURCES.txt` & `androidtvremote2-0.0.9/src/androidtvremote2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.8/src/demo.py` & `androidtvremote2-0.0.9/src/demo.py`

 * *Files identical despite different names*

