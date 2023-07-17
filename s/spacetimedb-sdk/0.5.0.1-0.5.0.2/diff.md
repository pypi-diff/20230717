# Comparing `tmp/spacetimedb_sdk-0.5.0.1.tar.gz` & `tmp/spacetimedb_sdk-0.5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetimedb_sdk-0.5.0.1.tar", last modified: Fri Jul 14 16:06:47 2023, max compression
+gzip compressed data, was "spacetimedb_sdk-0.5.0.2.tar", last modified: Mon Jul 17 21:17:09 2023, max compression
```

## Comparing `spacetimedb_sdk-0.5.0.1.tar` & `spacetimedb_sdk-0.5.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:47.532444 spacetimedb_sdk-0.5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 16:06:47.532444 spacetimedb_sdk-0.5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:06:47.532444 spacetimedb_sdk-0.5.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:47.528444 spacetimedb_sdk-0.5.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:47.532444 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/client_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetime_websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetimedb_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23365 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetimedb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:47.532444 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 16:06:47.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-14 16:06:47.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:06:47.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 16:06:47.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 16:06:47.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:09.609229 spacetimedb_sdk-0.5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 21:17:09.609229 spacetimedb_sdk-0.5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:17:09.609229 spacetimedb_sdk-0.5.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:09.605229 spacetimedb_sdk-0.5.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/gen_lazydocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:09.605229 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/client_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetime_websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetimedb_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetimedb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:09.609229 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 21:17:09.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-17 21:17:09.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:17:09.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 21:17:09.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 21:17:09.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/top_level.txt
```

### Comparing `spacetimedb_sdk-0.5.0.1/pyproject.toml` & `spacetimedb_sdk-0.5.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     {name = "Derek Brinkmann", email = "derek@clockworklabs.io"},
 ]
 
 dependencies = [
     "websocket-client",
     "configparser",
 ]
-version = "0.5.0.1"
+version = "0.5.0.2"
 readme = "README.md"
 
 # urls
 # Should describe where to find useful info for your project
 [project.urls]
 homepage = "https://spacetimedb.com"
 repository = "https://github.com/clockworklabs/spacetimedb-python-sdk"
```

### Comparing `spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/client_cache.py` & `spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/client_cache.py`

 * *Files identical despite different names*

### Comparing `spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/local_config.py` & `spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/local_config.py`

 * *Files identical despite different names*

### Comparing `spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetime_websocket_client.py` & `spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetime_websocket_client.py`

 * *Files identical despite different names*

### Comparing `spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetimedb_client.py` & `spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetimedb_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,60 @@
 import json
 import queue
 
 from spacetimedb_sdk.spacetime_websocket_client import WebSocketClient
 from spacetimedb_sdk.client_cache import ClientCache
 
 
+class Identity:
+    """
+    Represents a user identity. This is a wrapper around the Uint8Array that is recieved from SpacetimeDB.
+
+    Attributes:
+        data (bytes): The identity data.
+    """
+
+    def __init__(self, data):
+        self.data = bytes(data)  # Ensure data is always bytes
+
+    @staticmethod
+    def from_string(string):
+        """
+        Returns an Identity object with the data attribute set to the byte representation of the input string.
+
+        Args:
+            string (str): The input string.
+
+        Returns:
+            Identity: The Identity object.
+        """
+        return Identity(bytes.fromhex(string))
+
+    @staticmethod
+    def from_bytes(data):
+        """
+        Returns an Identity object with the data attribute set to the input bytes.
+
+        Args:
+            data (bytes): The input bytes.
+
+        Returns:
+            Identity: The Identity object.
+        """
+        return Identity(data)
+
+    # override to_string
+    def __str__(self):
+        return self.data.decode("utf-8")
+
+    # override = operator
+    def __eq__(self, other):
+        return isinstance(other, Identity) and self.data == other.data
+
+
 class DbEvent:
     """
     Represents a database event.
 
     Attributes:
         table_name (str): The name of the table associated with the event.
         row_pk (str): The primary key of the affected row.
@@ -82,15 +128,15 @@
         reducer (str): The reducer used for the transaction.
         args (dict): Additional arguments for the transaction.
         events (List[DbEvent]): List of DBEvents that were committed.
     """
 
     def __init__(
         self,
-        caller_identity: str,
+        caller_identity: Identity,
         status: str,
         message: str,
         reducer_name: str,
         args: Dict,
     ):
         super().__init__("TransactionUpdate")
         self.reducer_event = ReducerEvent(
@@ -112,15 +158,15 @@
         auth_token: str,
         host: str,
         address_or_name: str,
         ssl_enabled: bool,
         autogen_package: ModuleType,
         on_connect: Callable[[], None] = None,
         on_disconnect: Callable[[str], None] = None,
-        on_identity: Callable[[bytes], None] = None,
+        on_identity: Callable[[str, Identity], None] = None,
         on_error: Callable[[str], None] = None,
     ):
         """
         Create a network manager instance.
 
         Args:
             auth_token (str): This is the token generated by SpacetimeDB that matches the user's identity. If None, token will be generated
@@ -362,27 +408,27 @@
 
     def _on_message(self, data):
         # print("_on_message data: " + data)
         message = json.loads(data)
         if "IdentityToken" in message:
             # is this safe to do in the message thread?
             token = message["IdentityToken"]["token"]
-            identity = bytes.fromhex(message["IdentityToken"]["identity"])
+            identity = Identity.from_string(message["IdentityToken"]["identity"])
             self.message_queue.put(_IdentityReceivedMessage(token, identity))
         elif "SubscriptionUpdate" in message or "TransactionUpdate" in message:
             clientapi_message = None
             table_updates = None
             if "SubscriptionUpdate" in message:
                 clientapi_message = _SubscriptionUpdateMessage()
                 table_updates = message["SubscriptionUpdate"]["table_updates"]
             if "TransactionUpdate" in message:
                 spacetime_message = message["TransactionUpdate"]
                 # DAB Todo: We need reducer codegen to parse the args
                 clientapi_message = TransactionUpdateMessage(
-                    bytes.fromhex(spacetime_message["event"]["caller_identity"]),
+                    Identity.from_string(spacetime_message["event"]["caller_identity"]),
                     spacetime_message["event"]["status"],
                     spacetime_message["event"]["message"],
                     spacetime_message["event"]["function_call"]["reducer"],
                     json.loads(spacetime_message["event"]["function_call"]["args"]),
                 )
                 table_updates = message["TransactionUpdate"]["subscription_update"][
                     "table_updates"
@@ -457,26 +503,30 @@
                                 if (
                                     db_event.row_op == "insert"
                                     and other_db_event.row_op == "delete"
                                 ):
                                     # this is a row update so we need to replace the insert
                                     db_event.row_op = "update"
                                     db_event.old_pk = other_db_event.row_pk
+                                    db_event.old_value = other_db_event.old_value
                                     primary_key_row_ops[primary_key_value] = db_event
                                 elif (
                                     db_event.row_op == "delete"
                                     and other_db_event.row_op == "insert"
                                 ):
                                     # the insert was the row update so just upgrade it to update
                                     primary_key_row_ops[
                                         primary_key_value
                                     ].row_op = "update"
                                     primary_key_row_ops[
                                         primary_key_value
                                     ].old_pk = db_event.row_pk
+                                    primary_key_row_ops[
+                                        primary_key_value
+                                    ].old_value = db_event.old_value
                                 else:
                                     print(
                                         f"Error: duplicate primary key {table_name}:{primary_key_value}"
                                     )
                             else:
                                 primary_key_row_ops[primary_key_value] = db_event
```

