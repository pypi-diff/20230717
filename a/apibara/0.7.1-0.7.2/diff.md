# Comparing `tmp/apibara-0.7.1.tar.gz` & `tmp/apibara-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apibara-0.7.1.tar", max compression
+gzip compressed data, was "apibara-0.7.2.tar", max compression
```

## Comparing `apibara-0.7.1.tar` & `apibara-0.7.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     1342 2023-01-18 12:16:07.977321 apibara-0.7.1/README.rst
--rw-r--r--   0        0        0     1073 2023-07-14 20:14:53.243486 apibara-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.124336 apibara-0.7.1/src/apibara/__init__.py
--rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.7.1/src/apibara/cursor.py
--rw-r--r--   0        0        0      160 2023-01-15 18:52:09.124336 apibara-0.7.1/src/apibara/indexer/__init__.py
--rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.7.1/src/apibara/indexer/configuration.py
--rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.7.1/src/apibara/indexer/indexer.py
--rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.7.1/src/apibara/indexer/info.py
--rw-r--r--   0        0        0    10890 2023-07-14 20:14:20.212037 apibara-0.7.1/src/apibara/indexer/runner.py
--rw-r--r--   0        0        0    10502 2023-06-08 12:55:13.026953 apibara-0.7.1/src/apibara/indexer/storage.py
--rw-r--r--   0        0        0      697 2023-07-14 19:57:51.972597 apibara-0.7.1/src/apibara/protocol/__init__.py
--rw-r--r--   0        0        0     3596 2023-07-14 19:57:51.971597 apibara-0.7.1/src/apibara/protocol/client.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/protocol/proto/__init__.py
--rw-r--r--   0        0        0     3107 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/protocol/proto/stream_pb2.py
--rw-r--r--   0        0        0     9814 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/protocol/proto/stream_pb2.pyi
--rw-r--r--   0        0        0     2517 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/protocol/proto/stream_pb2_grpc.py
--rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/protocol/proto/stream_pb2_grpc.pyi
--rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/__init__.py
--rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/cursor.py
--rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/felt.py
--rw-r--r--   0        0        0    14725 2023-03-16 21:14:54.127582 apibara-0.7.1/src/apibara/starknet/filter.py
--rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/indexer.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/__init__.py
--rw-r--r--   0        0        0     7836 2023-07-08 12:11:24.025439 apibara-0.7.1/src/apibara/starknet/proto/filter_pb2.py
--rw-r--r--   0        0        0    12814 2023-07-08 12:11:24.025439 apibara-0.7.1/src/apibara/starknet/proto/filter_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/filter_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/filter_pb2_grpc.pyi
--rw-r--r--   0        0        0    11734 2023-07-14 19:57:51.968597 apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2.py
--rw-r--r--   0        0        0    20085 2023-07-08 12:11:24.025439 apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2_grpc.py
--rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1096 2023-06-30 17:37:45.778732 apibara-0.7.1/src/apibara/starknet/proto/types_pb2.py
--rw-r--r--   0        0        0      732 2023-06-30 17:37:45.775732 apibara-0.7.1/src/apibara/starknet/proto/types_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 apibara-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-31 15:41:14.195812 apibara-0.7.2/LICENSE.txt
+-rw-r--r--   0        0        0     1342 2023-03-31 15:41:14.195812 apibara-0.7.2/README.rst
+-rw-r--r--   0        0        0     1073 2023-07-17 17:00:35.412895 apibara-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-31 15:41:14.195812 apibara-0.7.2/src/apibara/__init__.py
+-rw-r--r--   0        0        0      514 2023-03-31 15:41:14.195812 apibara-0.7.2/src/apibara/cursor.py
+-rw-r--r--   0        0        0      160 2023-04-14 02:19:36.816437 apibara-0.7.2/src/apibara/indexer/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-14 02:19:36.816437 apibara-0.7.2/src/apibara/indexer/configuration.py
+-rw-r--r--   0        0        0     2393 2023-04-14 02:19:36.816437 apibara-0.7.2/src/apibara/indexer/indexer.py
+-rw-r--r--   0        0        0     1026 2023-04-14 02:19:36.816437 apibara-0.7.2/src/apibara/indexer/info.py
+-rw-r--r--   0        0        0    11043 2023-07-17 17:00:35.412895 apibara-0.7.2/src/apibara/indexer/runner.py
+-rw-r--r--   0        0        0    10502 2023-07-17 15:35:32.998834 apibara-0.7.2/src/apibara/indexer/storage.py
+-rw-r--r--   0        0        0      697 2023-07-17 15:49:47.686815 apibara-0.7.2/src/apibara/protocol/__init__.py
+-rw-r--r--   0        0        0     3596 2023-07-17 15:49:47.684815 apibara-0.7.2/src/apibara/protocol/client.py
+-rw-r--r--   0        0        0        0 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/protocol/proto/__init__.py
+-rw-r--r--   0        0        0     3107 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/protocol/proto/stream_pb2.py
+-rw-r--r--   0        0        0     9814 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/protocol/proto/stream_pb2.pyi
+-rw-r--r--   0        0        0     2517 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/protocol/proto/stream_pb2_grpc.py
+-rw-r--r--   0        0        0      878 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/protocol/proto/stream_pb2_grpc.pyi
+-rw-r--r--   0        0        0      264 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/__init__.py
+-rw-r--r--   0        0        0     1038 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/cursor.py
+-rw-r--r--   0        0        0     1375 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/felt.py
+-rw-r--r--   0        0        0    14725 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/filter.py
+-rw-r--r--   0        0        0      404 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/indexer.py
+-rw-r--r--   0        0        0        0 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/__init__.py
+-rw-r--r--   0        0        0     7836 2023-07-17 15:35:32.998834 apibara-0.7.2/src/apibara/starknet/proto/filter_pb2.py
+-rw-r--r--   0        0        0    12814 2023-07-17 15:35:32.998834 apibara-0.7.2/src/apibara/starknet/proto/filter_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/filter_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/filter_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11734 2023-07-17 15:49:47.736816 apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2.py
+-rw-r--r--   0        0        0    20085 2023-07-17 15:35:32.998834 apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2_grpc.py
+-rw-r--r--   0        0        0      100 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1096 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/types_pb2.py
+-rw-r--r--   0        0        0      732 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/types_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 apibara-0.7.2/PKG-INFO
```

### Comparing `apibara-0.7.1/LICENSE.txt` & `apibara-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/README.rst` & `apibara-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/pyproject.toml` & `apibara-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apibara"
-version = "0.7.1"
+version = "0.7.2"
 description = "Apibara cliend SDK. Stream and transform on-chain data with Python."
 authors = ["Francesco Ceccon <francesco@apibara.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 homepage = "https://www.apibara.com"
 repository= "https://github.com/apibara/python-sdk"
 keywords = [
```

### Comparing `apibara-0.7.1/src/apibara/cursor.py` & `apibara-0.7.2/src/apibara/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/indexer/indexer.py` & `apibara-0.7.2/src/apibara/indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/indexer/info.py` & `apibara-0.7.2/src/apibara/indexer/info.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/indexer/runner.py` & `apibara-0.7.2/src/apibara/indexer/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,31 +52,35 @@
     ----------
     reset_state:
         flag to restart the indexer from the beginning.
     config:
         options to set the input stream and connection string.
     client_options:
         list of options passed to the gRPC channel.
+    timeout:
+        custom timeout for a message to arrive.
     """
 
     def __init__(
         self,
         *,
         reset_state: bool = False,
         config: Optional[IndexerRunnerConfiguration] = None,
         client_options: Optional[List[Tuple[str, Any]]] = None,
+        timeout: Optional[int] = None,
     ) -> None:
         if config is None:
             config = IndexerRunnerConfiguration()
         if client_options is None:
             client_options = DEFAULT_CLIENT_OPTIONS
         self._reset_state = reset_state
         self._config = config
         self._indexer_id = None
         self._indexer_storage = None
+        self._timeout = timeout
         self._client_options = client_options
 
     async def run(self, indexer: Indexer, *, ctx: Optional[UserContext] = None):
         """Run the indexer until stopped."""
         self._check_config()
         self._setup_storage(indexer)
         self._maybe_reset_state()
@@ -116,15 +120,15 @@
                 reconnect = await indexer.handle_reconnect(exc, self._retry_count)
 
                 if not reconnect.reconnect:
                     raise
 
     async def _connect_and_stream(self, indexer: Indexer, ctx: Optional[UserContext]):
         channel = self._channel()
-        (client, stream) = StreamService(channel).stream_data()
+        (client, stream) = StreamService(channel).stream_data(timeout=self._timeout)
 
         config = indexer.initial_configuration()
         has_stored = self._indexer_storage.update_with_stored_configuration(config)
         if has_stored:
             # invalidate old pending data, if any
             self._indexer_storage.invalidate(config.starting_cursor)
```

### Comparing `apibara-0.7.1/src/apibara/indexer/storage.py` & `apibara-0.7.2/src/apibara/indexer/storage.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/protocol/__init__.py` & `apibara-0.7.2/src/apibara/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/protocol/client.py` & `apibara-0.7.2/src/apibara/protocol/client.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/protocol/proto/stream_pb2.py` & `apibara-0.7.2/src/apibara/protocol/proto/stream_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/protocol/proto/stream_pb2.pyi` & `apibara-0.7.2/src/apibara/protocol/proto/stream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/protocol/proto/stream_pb2_grpc.py` & `apibara-0.7.2/src/apibara/protocol/proto/stream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/protocol/proto/stream_pb2_grpc.pyi` & `apibara-0.7.2/src/apibara/protocol/proto/stream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/starknet/cursor.py` & `apibara-0.7.2/src/apibara/starknet/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/starknet/felt.py` & `apibara-0.7.2/src/apibara/starknet/felt.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/starknet/filter.py` & `apibara-0.7.2/src/apibara/starknet/filter.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/starknet/proto/filter_pb2.py` & `apibara-0.7.2/src/apibara/starknet/proto/filter_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/starknet/proto/filter_pb2.pyi` & `apibara-0.7.2/src/apibara/starknet/proto/filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2.py` & `apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2.pyi` & `apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/starknet/proto/types_pb2.py` & `apibara-0.7.2/src/apibara/starknet/proto/types_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/src/apibara/starknet/proto/types_pb2.pyi` & `apibara-0.7.2/src/apibara/starknet/proto/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.1/PKG-INFO` & `apibara-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apibara
-Version: 0.7.1
+Version: 0.7.2
 Summary: Apibara cliend SDK. Stream and transform on-chain data with Python.
 Home-page: https://www.apibara.com
 License: Apache-2.0
 Keywords: ethereum,web3,starknet
 Author: Francesco Ceccon
 Author-email: francesco@apibara.com
 Requires-Python: >=3.8,<3.11
```

