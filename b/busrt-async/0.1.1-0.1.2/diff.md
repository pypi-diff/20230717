# Comparing `tmp/busrt_async-0.1.1.tar.gz` & `tmp/busrt_async-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busrt_async-0.1.1.tar", last modified: Fri Sep 30 22:31:09 2022, max compression
+gzip compressed data, was "busrt_async-0.1.2.tar", last modified: Mon Jul 17 14:58:39 2023, max compression
```

## Comparing `busrt_async-0.1.1.tar` & `busrt_async-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-09-30 22:31:09.933799 busrt_async-0.1.1/
--rw-r--r--   0 divisor   (1000) root         (0)     1086 2022-09-30 19:58:29.000000 busrt_async-0.1.1/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)     4393 2022-09-30 22:31:09.933799 busrt_async-0.1.1/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)     3896 2022-09-30 19:58:29.000000 busrt_async-0.1.1/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-09-30 22:31:09.933799 busrt_async-0.1.1/busrt_async/
--rw-r--r--   0 divisor   (1000) root         (0)       49 2022-09-30 22:31:08.000000 busrt_async-0.1.1/busrt_async/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)     9834 2022-09-30 22:31:08.000000 busrt_async-0.1.1/busrt_async/client.py
--rw-r--r--   0 divisor   (1000) root         (0)     8066 2022-09-30 22:31:08.000000 busrt_async-0.1.1/busrt_async/rpc.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-09-30 22:31:09.933799 busrt_async-0.1.1/busrt_async.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)     4393 2022-09-30 22:31:09.000000 busrt_async-0.1.1/busrt_async.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      231 2022-09-30 22:31:09.000000 busrt_async-0.1.1/busrt_async.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2022-09-30 22:31:09.000000 busrt_async-0.1.1/busrt_async.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       12 2022-09-30 22:31:09.000000 busrt_async-0.1.1/busrt_async.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2022-09-30 22:31:09.933799 busrt_async-0.1.1/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)      731 2022-09-30 22:31:08.000000 busrt_async-0.1.1/setup.py
+drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-07-17 14:58:39.898748 busrt_async-0.1.2/
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)     5542 2023-07-17 14:58:39.898748 busrt_async-0.1.2/PKG-INFO
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)     3896 2022-09-30 23:27:42.000000 busrt_async-0.1.2/README.md
+drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-07-17 14:58:39.898748 busrt_async-0.1.2/busrt_async/
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)       49 2023-07-17 14:58:35.000000 busrt_async-0.1.2/busrt_async/__init__.py
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)     9834 2023-07-17 14:58:35.000000 busrt_async-0.1.2/busrt_async/client.py
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)     8066 2023-07-17 14:58:35.000000 busrt_async-0.1.2/busrt_async/rpc.py
+drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-07-17 14:58:39.898748 busrt_async-0.1.2/busrt_async.egg-info/
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)     5542 2023-07-17 14:58:39.000000 busrt_async-0.1.2/busrt_async.egg-info/PKG-INFO
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)      223 2023-07-17 14:58:39.000000 busrt_async-0.1.2/busrt_async.egg-info/SOURCES.txt
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)        1 2023-07-17 14:58:39.000000 busrt_async-0.1.2/busrt_async.egg-info/dependency_links.txt
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)       12 2023-07-17 14:58:39.000000 busrt_async-0.1.2/busrt_async.egg-info/top_level.txt
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)       38 2023-07-17 14:58:39.898748 busrt_async-0.1.2/setup.cfg
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)      731 2023-07-17 14:58:35.000000 busrt_async-0.1.2/setup.py
```

### Comparing `busrt_async-0.1.1/PKG-INFO` & `busrt_async-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: busrt_async
-Version: 0.1.1
-Summary: Python client for BUS/RT (async)
-Home-page: https://github.com/alttch/busrt
-Author: Bohemia Automation / Altertech
-Author-email: div@altertech.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Communications
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python async client for BUS/RT
 
 The module contains Python sync client for [BUS/RT](https://github.com/alttch/busrt)
 
 ## Installation
 
 ```shell
@@ -155,9 +139,7 @@
         'test.client.python.async.rpc',
         busrt_async.rpc.Request('test', msgpack.dumps(params)))
     reply = await result.wait_completed()
     print(msgpack.loads(reply.get_payload(), raw=False))
 
 asyncio.run(main())
 ```
-
-
```

### Comparing `busrt_async-0.1.1/README.md` & `busrt_async-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,145 +1,160 @@
-# Python async client for BUS/RT
-
-The module contains Python sync client for [BUS/RT](https://github.com/alttch/busrt)
-
-## Installation
-
-```shell
-pip3 install busrt_async
-```
-
-## Usage examples
-
-### Listener
-
-```python
-import busrt_async
-import asyncio
-
-# frame handler
-async def on_frame(frame):
-    print('Frame:', hex(frame.type), frame.sender, frame.topic, frame.payload)
-
-
-async def main():
-    name = 'test.client.python.async'
-    # create new BUS/RT client and connect
-    bus = busrt_async.client.Client('/tmp/busrt.sock', name)
-    bus.on_frame = on_frame
-    await bus.connect()
-    # subscribe to all topics
-    result = await bus.subscribe('#')
-    print(hex(await result.wait_completed()))
-    # wait for frames
-    print(f'listening for messages to {name}...')
-    while bus.is_connected():
-        await asyncio.sleep(0.1)
-
-asyncio.run(main())
-```
-
-### Sender
-
-```python
-import busrt_async
-import asyncio
-
-async def main():
-    name = 'test.client.python.async_sender'
-    bus = busrt_async.client.Client('/tmp/busrt.sock', name)
-    await bus.connect()
-    # send a regular message
-    result = await bus.send('test.client.python.async',
-                            busrt_async.client.Frame('hello'))
-    print(hex(await result.wait_completed()))
-    # send a broadcast message
-    result = await bus.send(
-        'test.*',
-        busrt_async.client.Frame('hello everyone',
-                                 tp=busrt_async.client.OP_BROADCAST))
-    print(hex(await result.wait_completed()))
-    # publish to a topic with zero QoS (no confirmation required)
-    await bus.send(
-        'test/topic',
-        busrt_async.client.Frame('something',
-                                 tp=busrt_async.client.OP_PUBLISH,
-                                 qos=0))
-
-asyncio.run(main())
-```
-
-## RPC layer
-
-### Handler
-
-```python
-import busrt_async
-import asyncio
-import msgpack
-
-# frame handler (topics/broadcasts)
-async def on_frame(frame):
-    print('Frame:', hex(frame.type), frame.sender, frame.topic, frame.payload)
-
-# RPC notification handler
-async def on_notification(event):
-    print('Notification:', event.frame.sender, event.get_payload())
-
-# RPC call handler
-async def on_call(event):
-    # consider payload is encoded in msgpack
-    print('Call:', event.frame.sender, event.method,
-          msgpack.loads(event.get_payload(), raw=False))
-    # msgpack reply
-    return msgpack.dumps({'ok': True})
-
-async def main():
-    name = 'test.client.python.async.rpc'
-    # create new BUS/RT client and connect
-    bus = busrt_async.client.Client('/tmp/busrt.sock', name)
-    await bus.connect()
-    # subscribe to all topics
-    result = await bus.subscribe('#')
-    print(hex(await result.wait_completed()))
-    # init rpc
-    rpc = busrt_async.rpc.Rpc(bus)
-    rpc.on_frame = on_frame
-    rpc.on_notification = on_notification
-    rpc.on_call = on_call
-    # wait for frames
-    print(f'listening for messages/calls to {name}...')
-    while rpc.is_connected():
-        await asyncio.sleep(0.1)
-
-asyncio.run(main())
-```
-
-### Caller
-
-```python
-import busrt_async
-import msgpack
-import asyncio
-
-async def main():
-    name = 'test.client.python.async.rpc.caller'
-    # create new BUS/RT client and connect
-    bus = busrt_async.client.Client('/tmp/busrt.sock', name)
-    await bus.connect()
-    # init rpc
-    rpc = busrt_async.rpc.Rpc(bus)
-    params = {'hello': 123}
-    # call a method, no reply required
-    result = await rpc.call0(
-        'test.client.python.async.rpc',
-        busrt_async.rpc.Request('test', msgpack.dumps(params)))
-    print(hex(await result.wait_completed()))
-    # call a method and wait for the reply
-    result = await rpc.call(
-        'test.client.python.async.rpc',
-        busrt_async.rpc.Request('test', msgpack.dumps(params)))
-    reply = await result.wait_completed()
-    print(msgpack.loads(reply.get_payload(), raw=False))
-
-asyncio.run(main())
-```
+Metadata-Version: 2.1
+Name: busrt_async
+Version: 0.1.2
+Summary: Python client for BUS/RT (async)
+Home-page: https://github.com/alttch/busrt
+Author: Bohemia Automation / Altertech
+Author-email: div@altertech.com
+License: MIT
+Description: # Python async client for BUS/RT
+        
+        The module contains Python sync client for [BUS/RT](https://github.com/alttch/busrt)
+        
+        ## Installation
+        
+        ```shell
+        pip3 install busrt_async
+        ```
+        
+        ## Usage examples
+        
+        ### Listener
+        
+        ```python
+        import busrt_async
+        import asyncio
+        
+        # frame handler
+        async def on_frame(frame):
+            print('Frame:', hex(frame.type), frame.sender, frame.topic, frame.payload)
+        
+        
+        async def main():
+            name = 'test.client.python.async'
+            # create new BUS/RT client and connect
+            bus = busrt_async.client.Client('/tmp/busrt.sock', name)
+            bus.on_frame = on_frame
+            await bus.connect()
+            # subscribe to all topics
+            result = await bus.subscribe('#')
+            print(hex(await result.wait_completed()))
+            # wait for frames
+            print(f'listening for messages to {name}...')
+            while bus.is_connected():
+                await asyncio.sleep(0.1)
+        
+        asyncio.run(main())
+        ```
+        
+        ### Sender
+        
+        ```python
+        import busrt_async
+        import asyncio
+        
+        async def main():
+            name = 'test.client.python.async_sender'
+            bus = busrt_async.client.Client('/tmp/busrt.sock', name)
+            await bus.connect()
+            # send a regular message
+            result = await bus.send('test.client.python.async',
+                                    busrt_async.client.Frame('hello'))
+            print(hex(await result.wait_completed()))
+            # send a broadcast message
+            result = await bus.send(
+                'test.*',
+                busrt_async.client.Frame('hello everyone',
+                                         tp=busrt_async.client.OP_BROADCAST))
+            print(hex(await result.wait_completed()))
+            # publish to a topic with zero QoS (no confirmation required)
+            await bus.send(
+                'test/topic',
+                busrt_async.client.Frame('something',
+                                         tp=busrt_async.client.OP_PUBLISH,
+                                         qos=0))
+        
+        asyncio.run(main())
+        ```
+        
+        ## RPC layer
+        
+        ### Handler
+        
+        ```python
+        import busrt_async
+        import asyncio
+        import msgpack
+        
+        # frame handler (topics/broadcasts)
+        async def on_frame(frame):
+            print('Frame:', hex(frame.type), frame.sender, frame.topic, frame.payload)
+        
+        # RPC notification handler
+        async def on_notification(event):
+            print('Notification:', event.frame.sender, event.get_payload())
+        
+        # RPC call handler
+        async def on_call(event):
+            # consider payload is encoded in msgpack
+            print('Call:', event.frame.sender, event.method,
+                  msgpack.loads(event.get_payload(), raw=False))
+            # msgpack reply
+            return msgpack.dumps({'ok': True})
+        
+        async def main():
+            name = 'test.client.python.async.rpc'
+            # create new BUS/RT client and connect
+            bus = busrt_async.client.Client('/tmp/busrt.sock', name)
+            await bus.connect()
+            # subscribe to all topics
+            result = await bus.subscribe('#')
+            print(hex(await result.wait_completed()))
+            # init rpc
+            rpc = busrt_async.rpc.Rpc(bus)
+            rpc.on_frame = on_frame
+            rpc.on_notification = on_notification
+            rpc.on_call = on_call
+            # wait for frames
+            print(f'listening for messages/calls to {name}...')
+            while rpc.is_connected():
+                await asyncio.sleep(0.1)
+        
+        asyncio.run(main())
+        ```
+        
+        ### Caller
+        
+        ```python
+        import busrt_async
+        import msgpack
+        import asyncio
+        
+        async def main():
+            name = 'test.client.python.async.rpc.caller'
+            # create new BUS/RT client and connect
+            bus = busrt_async.client.Client('/tmp/busrt.sock', name)
+            await bus.connect()
+            # init rpc
+            rpc = busrt_async.rpc.Rpc(bus)
+            params = {'hello': 123}
+            # call a method, no reply required
+            result = await rpc.call0(
+                'test.client.python.async.rpc',
+                busrt_async.rpc.Request('test', msgpack.dumps(params)))
+            print(hex(await result.wait_completed()))
+            # call a method and wait for the reply
+            result = await rpc.call(
+                'test.client.python.async.rpc',
+                busrt_async.rpc.Request('test', msgpack.dumps(params)))
+            reply = await result.wait_completed()
+            print(msgpack.loads(reply.get_payload(), raw=False))
+        
+        asyncio.run(main())
+        ```
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Communications
+Description-Content-Type: text/markdown
```

### Comparing `busrt_async-0.1.1/busrt_async/client.py` & `busrt_async-0.1.2/busrt_async/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self.socket_lock = asyncio.Lock()
         self.mgmt_lock = asyncio.Lock()
         self.connected = False
         self.frames = {}
         self.timeout = 1
 
     async def connect(self):
-        with await self.mgmt_lock:
+        async with self.mgmt_lock:
             if self.path.endswith('.sock') or self.path.endswith(
                     '.socket') or self.path.endswith(
                         '.ipc') or self.path.startswith('/'):
                 reader, writer = await asyncio.open_unix_connection(
                     self.path, limit=self.buf_size)
             else:
                 host, port = self.path.rsplit(':', maxsplit=2)
@@ -84,25 +84,25 @@
                 raise RuntimeError(f'Server response: {hex(buf[0])}')
             self.writer = writer
             self.connected = True
             self.pinger_fut = asyncio.ensure_future(self._t_pinger())
             self.reader_fut = asyncio.ensure_future(self._t_reader(reader))
 
     async def handle_daemon_exception(self, e):
-        with await self.mgmt_lock:
+        async with self.mgmt_lock:
             if self.connected:
                 await self._disconnect()
                 import traceback
                 logger.error(traceback.format_exc())
 
     async def _t_pinger(self):
         try:
             while True:
                 await asyncio.sleep(self.ping_interval)
-                with await self.socket_lock:
+                async with self.socket_lock:
                     self.writer.write(PING_FRAME)
                     await asyncio.wait_for(self.writer.drain(),
                                            timeout=self.timeout)
         except Exception as e:
             asyncio.ensure_future(self.handle_daemon_exception(e))
 
     async def _t_reader(self, reader):
@@ -165,28 +165,28 @@
                     buf_size if buf_size < self.buf_size else self.buf_size)
                 data += chunk
             except asyncio.IncompleteReadError:
                 await asyncio.sleep(0.01)
         return data
 
     async def disconnect(self):
-        with await self.mgmt_lock:
+        async with self.mgmt_lock:
             await self._disconnect()
 
     async def _disconnect(self):
         self.connected = False
         self.writer.close()
         if self.reader_fut is not None:
             self.reader_fut.cancel()
         if self.pinger_fut is not None:
             self.pinger_fut.cancel()
 
     async def send(self, target=None, frame=None):
         try:
-            with await self.socket_lock:
+            async with self.socket_lock:
                 self.frame_id += 1
                 if self.frame_id > 0xffff_ffff:
                     self.frame_id = 1
                 frame_id = self.frame_id
                 o = ClientFrame(frame.qos)
                 if frame.qos & 0b1 != 0:
                     self.frames[frame_id] = o
```

### Comparing `busrt_async-0.1.1/busrt_async/rpc.py` & `busrt_async-0.1.2/busrt_async/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     def call0(self, target, request):
         request.header = RPC_REQUEST_HEADER + b'\x00\x00\x00\x00' + \
                 request.method + b'\x00'
         return self.client.send(target, request)
 
     async def call(self, target, request):
-        with await self.call_lock:
+        async with self.call_lock:
             call_id = self.call_id + 1
             if call_id == 0xffff_ffff:
                 self.call_id = 0
             else:
                 self.call_id = call_id
         call_event = RpcCallEvent()
         self.calls[call_id] = call_event
```

### Comparing `busrt_async-0.1.1/busrt_async.egg-info/PKG-INFO` & `busrt_async-0.1.2/busrt_async.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,163 +1,160 @@
 Metadata-Version: 2.1
 Name: busrt-async
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for BUS/RT (async)
 Home-page: https://github.com/alttch/busrt
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: MIT
+Description: # Python async client for BUS/RT
+        
+        The module contains Python sync client for [BUS/RT](https://github.com/alttch/busrt)
+        
+        ## Installation
+        
+        ```shell
+        pip3 install busrt_async
+        ```
+        
+        ## Usage examples
+        
+        ### Listener
+        
+        ```python
+        import busrt_async
+        import asyncio
+        
+        # frame handler
+        async def on_frame(frame):
+            print('Frame:', hex(frame.type), frame.sender, frame.topic, frame.payload)
+        
+        
+        async def main():
+            name = 'test.client.python.async'
+            # create new BUS/RT client and connect
+            bus = busrt_async.client.Client('/tmp/busrt.sock', name)
+            bus.on_frame = on_frame
+            await bus.connect()
+            # subscribe to all topics
+            result = await bus.subscribe('#')
+            print(hex(await result.wait_completed()))
+            # wait for frames
+            print(f'listening for messages to {name}...')
+            while bus.is_connected():
+                await asyncio.sleep(0.1)
+        
+        asyncio.run(main())
+        ```
+        
+        ### Sender
+        
+        ```python
+        import busrt_async
+        import asyncio
+        
+        async def main():
+            name = 'test.client.python.async_sender'
+            bus = busrt_async.client.Client('/tmp/busrt.sock', name)
+            await bus.connect()
+            # send a regular message
+            result = await bus.send('test.client.python.async',
+                                    busrt_async.client.Frame('hello'))
+            print(hex(await result.wait_completed()))
+            # send a broadcast message
+            result = await bus.send(
+                'test.*',
+                busrt_async.client.Frame('hello everyone',
+                                         tp=busrt_async.client.OP_BROADCAST))
+            print(hex(await result.wait_completed()))
+            # publish to a topic with zero QoS (no confirmation required)
+            await bus.send(
+                'test/topic',
+                busrt_async.client.Frame('something',
+                                         tp=busrt_async.client.OP_PUBLISH,
+                                         qos=0))
+        
+        asyncio.run(main())
+        ```
+        
+        ## RPC layer
+        
+        ### Handler
+        
+        ```python
+        import busrt_async
+        import asyncio
+        import msgpack
+        
+        # frame handler (topics/broadcasts)
+        async def on_frame(frame):
+            print('Frame:', hex(frame.type), frame.sender, frame.topic, frame.payload)
+        
+        # RPC notification handler
+        async def on_notification(event):
+            print('Notification:', event.frame.sender, event.get_payload())
+        
+        # RPC call handler
+        async def on_call(event):
+            # consider payload is encoded in msgpack
+            print('Call:', event.frame.sender, event.method,
+                  msgpack.loads(event.get_payload(), raw=False))
+            # msgpack reply
+            return msgpack.dumps({'ok': True})
+        
+        async def main():
+            name = 'test.client.python.async.rpc'
+            # create new BUS/RT client and connect
+            bus = busrt_async.client.Client('/tmp/busrt.sock', name)
+            await bus.connect()
+            # subscribe to all topics
+            result = await bus.subscribe('#')
+            print(hex(await result.wait_completed()))
+            # init rpc
+            rpc = busrt_async.rpc.Rpc(bus)
+            rpc.on_frame = on_frame
+            rpc.on_notification = on_notification
+            rpc.on_call = on_call
+            # wait for frames
+            print(f'listening for messages/calls to {name}...')
+            while rpc.is_connected():
+                await asyncio.sleep(0.1)
+        
+        asyncio.run(main())
+        ```
+        
+        ### Caller
+        
+        ```python
+        import busrt_async
+        import msgpack
+        import asyncio
+        
+        async def main():
+            name = 'test.client.python.async.rpc.caller'
+            # create new BUS/RT client and connect
+            bus = busrt_async.client.Client('/tmp/busrt.sock', name)
+            await bus.connect()
+            # init rpc
+            rpc = busrt_async.rpc.Rpc(bus)
+            params = {'hello': 123}
+            # call a method, no reply required
+            result = await rpc.call0(
+                'test.client.python.async.rpc',
+                busrt_async.rpc.Request('test', msgpack.dumps(params)))
+            print(hex(await result.wait_completed()))
+            # call a method and wait for the reply
+            result = await rpc.call(
+                'test.client.python.async.rpc',
+                busrt_async.rpc.Request('test', msgpack.dumps(params)))
+            reply = await result.wait_completed()
+            print(msgpack.loads(reply.get_payload(), raw=False))
+        
+        asyncio.run(main())
+        ```
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Communications
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python async client for BUS/RT
-
-The module contains Python sync client for [BUS/RT](https://github.com/alttch/busrt)
-
-## Installation
-
-```shell
-pip3 install busrt_async
-```
-
-## Usage examples
-
-### Listener
-
-```python
-import busrt_async
-import asyncio
-
-# frame handler
-async def on_frame(frame):
-    print('Frame:', hex(frame.type), frame.sender, frame.topic, frame.payload)
-
-
-async def main():
-    name = 'test.client.python.async'
-    # create new BUS/RT client and connect
-    bus = busrt_async.client.Client('/tmp/busrt.sock', name)
-    bus.on_frame = on_frame
-    await bus.connect()
-    # subscribe to all topics
-    result = await bus.subscribe('#')
-    print(hex(await result.wait_completed()))
-    # wait for frames
-    print(f'listening for messages to {name}...')
-    while bus.is_connected():
-        await asyncio.sleep(0.1)
-
-asyncio.run(main())
-```
-
-### Sender
-
-```python
-import busrt_async
-import asyncio
-
-async def main():
-    name = 'test.client.python.async_sender'
-    bus = busrt_async.client.Client('/tmp/busrt.sock', name)
-    await bus.connect()
-    # send a regular message
-    result = await bus.send('test.client.python.async',
-                            busrt_async.client.Frame('hello'))
-    print(hex(await result.wait_completed()))
-    # send a broadcast message
-    result = await bus.send(
-        'test.*',
-        busrt_async.client.Frame('hello everyone',
-                                 tp=busrt_async.client.OP_BROADCAST))
-    print(hex(await result.wait_completed()))
-    # publish to a topic with zero QoS (no confirmation required)
-    await bus.send(
-        'test/topic',
-        busrt_async.client.Frame('something',
-                                 tp=busrt_async.client.OP_PUBLISH,
-                                 qos=0))
-
-asyncio.run(main())
-```
-
-## RPC layer
-
-### Handler
-
-```python
-import busrt_async
-import asyncio
-import msgpack
-
-# frame handler (topics/broadcasts)
-async def on_frame(frame):
-    print('Frame:', hex(frame.type), frame.sender, frame.topic, frame.payload)
-
-# RPC notification handler
-async def on_notification(event):
-    print('Notification:', event.frame.sender, event.get_payload())
-
-# RPC call handler
-async def on_call(event):
-    # consider payload is encoded in msgpack
-    print('Call:', event.frame.sender, event.method,
-          msgpack.loads(event.get_payload(), raw=False))
-    # msgpack reply
-    return msgpack.dumps({'ok': True})
-
-async def main():
-    name = 'test.client.python.async.rpc'
-    # create new BUS/RT client and connect
-    bus = busrt_async.client.Client('/tmp/busrt.sock', name)
-    await bus.connect()
-    # subscribe to all topics
-    result = await bus.subscribe('#')
-    print(hex(await result.wait_completed()))
-    # init rpc
-    rpc = busrt_async.rpc.Rpc(bus)
-    rpc.on_frame = on_frame
-    rpc.on_notification = on_notification
-    rpc.on_call = on_call
-    # wait for frames
-    print(f'listening for messages/calls to {name}...')
-    while rpc.is_connected():
-        await asyncio.sleep(0.1)
-
-asyncio.run(main())
-```
-
-### Caller
-
-```python
-import busrt_async
-import msgpack
-import asyncio
-
-async def main():
-    name = 'test.client.python.async.rpc.caller'
-    # create new BUS/RT client and connect
-    bus = busrt_async.client.Client('/tmp/busrt.sock', name)
-    await bus.connect()
-    # init rpc
-    rpc = busrt_async.rpc.Rpc(bus)
-    params = {'hello': 123}
-    # call a method, no reply required
-    result = await rpc.call0(
-        'test.client.python.async.rpc',
-        busrt_async.rpc.Request('test', msgpack.dumps(params)))
-    print(hex(await result.wait_completed()))
-    # call a method and wait for the reply
-    result = await rpc.call(
-        'test.client.python.async.rpc',
-        busrt_async.rpc.Request('test', msgpack.dumps(params)))
-    reply = await result.wait_completed()
-    print(msgpack.loads(reply.get_payload(), raw=False))
-
-asyncio.run(main())
-```
-
-
```

### Comparing `busrt_async-0.1.1/setup.py` & `busrt_async-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

