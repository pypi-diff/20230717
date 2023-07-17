# Comparing `tmp/oms-mqclient-2.3.1.tar.gz` & `tmp/oms-mqclient-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.3.1.tar", last modified: Thu Jul 13 00:03:28 2023, max compression
+gzip compressed data, was "oms-mqclient-2.3.2.tar", last modified: Mon Jul 17 21:02:07 2023, max compression
```

## Comparing `oms-mqclient-2.3.1.tar` & `oms-mqclient-2.3.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.497490 oms-mqclient-2.3.1/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2651 2023-07-13 00:03:28.497490 oms-mqclient-2.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.489489 oms-mqclient-2.3.1/mqclient/
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5972 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.489489 oms-mqclient-2.3.1/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13450 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    13421 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    15335 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1791 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/broker_clients/utils.py
--rw-r--r--   0 root         (0) root         (0)      375 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    24455 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.489489 oms-mqclient-2.3.1/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2651 2023-07-13 00:03:28.000000 oms-mqclient-2.3.1/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-13 00:03:28.000000 oms-mqclient-2.3.1/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:03:28.000000 oms-mqclient-2.3.1/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      298 2023-07-13 00:03:28.000000 oms-mqclient-2.3.1/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-13 00:03:28.000000 oms-mqclient-2.3.1/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2708 2023-07-13 00:03:28.497490 oms-mqclient-2.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.485489 oms-mqclient-2.3.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.493490 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9038 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    35457 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    20234 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.493490 oms-mqclient-2.3.1/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.493490 oms-mqclient-2.3.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.493490 oms-mqclient-2.3.1/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5586 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:03:28.497490 oms-mqclient-2.3.1/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9196 2023-07-13 00:03:25.000000 oms-mqclient-2.3.1/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.970305 oms-mqclient-2.3.2/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-07-17 21:02:07.970305 oms-mqclient-2.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.962304 oms-mqclient-2.3.2/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14434 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    14181 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    16642 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_clients/utils.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    23738 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-07-17 21:02:07.000000 oms-mqclient-2.3.2/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-17 21:02:07.000000 oms-mqclient-2.3.2/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 21:02:07.000000 oms-mqclient-2.3.2/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      298 2023-07-17 21:02:07.000000 oms-mqclient-2.3.2/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 21:02:07.000000 oms-mqclient-2.3.2/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-07-17 21:02:07.970305 oms-mqclient-2.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.962304 oms-mqclient-2.3.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9038 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    35347 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    20234 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5586 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9196 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.3.1/LICENSE` & `oms-mqclient-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/PKG-INFO` & `oms-mqclient-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.3.1
+Version: 2.3.2
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.3.1/README.md` & `oms-mqclient-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/mqclient/__init__.py` & `oms-mqclient-2.3.2/mqclient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.3.1"
+__version__ = "2.3.2"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.3.1/mqclient/broker_client_interface.py` & `oms-mqclient-2.3.2/mqclient/broker_client_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,15 +102,21 @@
 # -----------------------------
 
 
 class RawQueue:
     """Raw queue object, to hold queue state."""
 
     def __init__(self) -> None:
-        pass
+        # `connection_can_have_multiple_unacked_messages=True` signifies
+        # that a sub is not acking/nacking a previous message before
+        # getting another (these previous messages are 'unacked').
+        # - By default, set this to `False`. This can be changed by
+        #     the encompassing `Queue` if unacked messages are expected.
+        # - Each broker client handles this setting slightly different.
+        self.connection_can_have_multiple_unacked_messages = False
 
     async def connect(self) -> None:
         """Set up connection."""
 
     async def close(self) -> None:
         """Close interface to queue."""
 
@@ -118,15 +124,15 @@
 class Pub(RawQueue):
     """Publisher queue."""
 
     async def send_message(
         self,
         msg: bytes,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Send a message on a queue."""
         raise NotImplementedError()
 
 
 class Sub(RawQueue):
     """Subscriber queue."""
@@ -142,43 +148,43 @@
         type."""
         raise NotImplementedError()
 
     async def get_message(
         self,
         timeout_millis: Optional[int],
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> Optional[Message]:
         """Get a single message from a queue."""
         raise NotImplementedError()
 
     async def ack_message(
         self,
         msg: Message,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Ack a message from the queue."""
         raise NotImplementedError()
 
     async def reject_message(
         self,
         msg: Message,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Reject (nack) a message from the queue."""
         raise NotImplementedError()
 
     def message_generator(  # NOTE: no `async` b/c it's abstract; overriding methods will need `async`
         self,
         timeout: int,
         propagate_error: bool,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> AsyncGenerator[Optional[Message], None]:
         """Yield Messages.
 
         Asynchronously generate messages with variable timeout.
         Yield `None` on `athrow()`.
 
         Keyword Arguments:
```

### Comparing `oms-mqclient-2.3.1/mqclient/broker_client_manager.py` & `oms-mqclient-2.3.2/mqclient/broker_client_manager.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.3.2/mqclient/broker_clients/apachepulsar.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,30 +121,42 @@
             raise ClosingFailedException("No producer to sub.")
         LOGGER.debug(log_msgs.CLOSED_PUB)
 
     async def send_message(
         self,
         msg: bytes,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Send a message on a queue."""
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
         if not self.producer:
             raise RuntimeError("queue is not connected")
 
+        def _send_msg():
+            # use wrapper function so connection references can be updated by reconnects
+            if not self.producer:
+                raise RuntimeError("queue is not connected")
+            return self.producer.send(msg)
+
         await utils.auto_retry_call(
-            func=functools.partial(
-                self.producer.send,
-                msg,
-            ),
+            func=_send_msg,
             retries=retries,
             retry_delay=retry_delay,
-            close=self.close,
-            connect=self.connect,
+            close=(
+                None
+                if self.connection_can_have_multiple_unacked_messages
+                else self.close
+            ),
+            connect=(
+                None
+                if self.connection_can_have_multiple_unacked_messages
+                else self.connect
+            ),
+            nonretriable_conditions=None,
             logger=LOGGER,
         )
         LOGGER.debug(log_msgs.SENT_MESSAGE)
 
 
 class PulsarSub(Pulsar, Sub):
     """Wrapper around pulsar.Consumer.
@@ -217,35 +229,46 @@
         else:
             return Message(id_, data)
 
     async def get_message(
         self,
         timeout_millis: Optional[int],
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> Optional[Message]:
         """Get a single message from a queue.
 
         To endlessly block until a message is available, set
         `timeout_millis=None`.
         """
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
         if not self.consumer:
             raise RuntimeError("queue is not connected")
 
+        def _get_msg():
+            # use wrapper function so connection references can be updated by reconnects
+            if not self.consumer:
+                raise RuntimeError("queue is not connected")
+            return self.consumer.receive(timeout_millis=timeout_millis)
+
         try:
             pulsar_msg = await utils.auto_retry_call(
-                func=functools.partial(
-                    self.consumer.receive,
-                    timeout_millis=timeout_millis,
-                ),
+                func=_get_msg,
                 retries=retries,
                 retry_delay=retry_delay,
-                close=self.close,
-                connect=self.connect,
+                close=(
+                    None
+                    if self.connection_can_have_multiple_unacked_messages
+                    else self.close
+                ),
+                connect=(
+                    None
+                    if self.connection_can_have_multiple_unacked_messages
+                    else self.connect
+                ),
                 logger=LOGGER,
                 nonretriable_conditions=lambda e: str(e) == "Pulsar error: TimeOut",
             )
         except Exception as e:
             # https://github.com/apache/pulsar/issues/3127
             # consumer timed out so there's nothing left in the tube
             if str(e) == "Pulsar error: TimeOut":
@@ -259,15 +282,15 @@
             LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
             return None
 
     async def ack_message(
         self,
         msg: Message,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Ack a message from the queue."""
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
         if not self.consumer:
             raise RuntimeError("queue is not connected")
 
         if isinstance(msg.msg_id, bytes):
@@ -278,25 +301,26 @@
         await utils.auto_retry_call(
             func=functools.partial(
                 self.consumer.acknowledge,
                 pulsar_msg,
             ),
             retries=retries,
             retry_delay=retry_delay,
-            close=self.close,
-            connect=self.connect,
+            close=None,
+            connect=None,
+            nonretriable_conditions=None,
             logger=LOGGER,
         )
         LOGGER.debug(f"{log_msgs.ACKED_MESSAGE} ({msg}).")
 
     async def reject_message(
         self,
         msg: Message,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Reject (nack) a message from the queue."""
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
         if not self.consumer:
             raise RuntimeError("queue is not connected")
 
         if isinstance(msg.msg_id, bytes):
@@ -307,26 +331,27 @@
         await utils.auto_retry_call(
             func=functools.partial(
                 self.consumer.negative_acknowledge,
                 pulsar_msg,
             ),
             retries=retries,
             retry_delay=retry_delay,
-            close=self.close,
-            connect=self.connect,
+            close=None,
+            connect=None,
+            nonretriable_conditions=None,
             logger=LOGGER,
         )
         LOGGER.debug(f"{log_msgs.NACKED_MESSAGE} ({msg}).")
 
     async def message_generator(
         self,
         timeout: int,
         propagate_error: bool,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> AsyncGenerator[Optional[Message], None]:
         """Yield Messages.
 
         Generate messages with variable timeout.
         Yield `None` on `throw()`.
 
         Keyword Arguments:
```

### Comparing `oms-mqclient-2.3.1/mqclient/broker_clients/nats.py` & `oms-mqclient-2.3.2/mqclient/broker_clients/nats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Back-end using NATS."""
 
 
-import functools
 import logging
 import math
 from typing import Any, AsyncGenerator, List, Optional, TypeVar, cast
 
 import nats
 
 from .. import broker_client_interface, log_msgs
@@ -98,31 +97,34 @@
         await super().close()
         LOGGER.debug(log_msgs.CLOSED_PUB)
 
     async def send_message(
         self,
         msg: bytes,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Send a message (publish)."""
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
         if not self.js:
             raise RuntimeError("JetStream is not connected")
 
+        async def _send_msg():
+            # use wrapper function so connection references can be updated by reconnects
+            if not self.js:
+                raise RuntimeError("JetStream is not connected")
+            return await self.js.publish(self.subject, msg)
+
         ack: nats.js.api.PubAck = await utils.auto_retry_call(
-            func=functools.partial(
-                self.js.publish,
-                self.subject,
-                msg,
-            ),
+            func=_send_msg,
             retries=retries,
             retry_delay=retry_delay,
             close=self.close,
             connect=self.connect,
+            nonretriable_conditions=None,
             logger=LOGGER,
         )
         LOGGER.debug(f"Sent Message w/ Ack: {ack}")
         LOGGER.debug(log_msgs.SENT_MESSAGE)
 
 
 class NATSSub(NATS, Sub):
@@ -181,34 +183,39 @@
         )
 
     async def _get_messages(
         self,
         timeout_millis: Optional[int],
         num_messages: int,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> List[Message]:
         """Get n messages.
 
         The subscriber pulls a specific number of messages. The actual
         number of messages pulled may be smaller than `num_messages`.
         """
         if not self._subscription:
             raise RuntimeError("Subscriber is not connected")
 
         if not timeout_millis:
             timeout_millis = DEFAULT_TIMEOUT_MILLIS
 
+        async def _get_msg():
+            # use wrapper function so connection references can be updated by reconnects
+            if not self._subscription:
+                raise RuntimeError("Subscriber is not connected")
+            return await self._subscription.fetch(
+                batch=num_messages,
+                timeout=int(math.ceil(timeout_millis / 1000)),
+            )
+
         try:
             nats_msgs: List[nats.aio.msg.Msg] = await utils.auto_retry_call(
-                func=functools.partial(
-                    self._subscription.fetch,
-                    batch=num_messages,
-                    timeout=int(math.ceil(timeout_millis / 1000)),
-                ),
+                func=_get_msg,
                 retries=retries,
                 retry_delay=retry_delay,
                 close=self.close,
                 connect=self.connect,
                 logger=LOGGER,
                 nonretriable_conditions=lambda e: isinstance(
                     e, nats.errors.TimeoutError
@@ -227,15 +234,15 @@
                 msgs.append(msg)
         return msgs
 
     async def get_message(
         self,
         timeout_millis: Optional[int],
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> Optional[Message]:
         """Get a message."""
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
         if not self._subscription:
             raise RuntimeError("Subscriber is not connected.")
 
         try:
@@ -252,15 +259,15 @@
             return None
 
     async def _gen_messages(
         self,
         timeout_millis: Optional[int],
         num_messages: int,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> AsyncGenerator[Message, None]:
         """Continuously generate messages until there are no more."""
         if not self._subscription:
             raise RuntimeError("Subscriber is not connected.")
 
         while True:
             msgs = await self._get_messages(
@@ -274,59 +281,69 @@
             for msg in msgs:
                 yield msg
 
     async def ack_message(
         self,
         msg: Message,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Ack a message from the queue."""
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
         if not self._subscription:
             raise RuntimeError("subscriber is not connected")
 
+        async def _ack_msg():
+            # use wrapper function so connection references can be updated by reconnects
+            return await self._from_message(msg).ack()
+
         # Acknowledges the received messages so they will not be sent again.
         await utils.auto_retry_call(
-            func=self._from_message(msg).ack,  # type: ignore[arg-type]
+            func=_ack_msg,
             retries=retries,
             retry_delay=retry_delay,
             close=self.close,
             connect=self.connect,
+            nonretriable_conditions=None,
             logger=LOGGER,
         )
         LOGGER.debug(f"{log_msgs.ACKED_MESSAGE} ({msg.msg_id!r}).")
 
     async def reject_message(
         self,
         msg: Message,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Reject (nack) a message from the queue."""
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
         if not self._subscription:
             raise RuntimeError("subscriber is not connected")
 
+        async def _nack_msg():
+            # use wrapper function so connection references can be updated by reconnects
+            return await self._from_message(msg).nak()  # yes, it's "nak"
+
         await utils.auto_retry_call(
-            func=self._from_message(msg).nak,  # type: ignore[arg-type]  # yes, it's "nak"
+            func=_nack_msg,
             retries=retries,
             retry_delay=retry_delay,
             close=self.close,
             connect=self.connect,
+            nonretriable_conditions=None,
             logger=LOGGER,
         )
         LOGGER.debug(f"{log_msgs.NACKED_MESSAGE} ({msg.msg_id!r}).")
 
     async def message_generator(
         self,
         timeout: int,
         propagate_error: bool,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> AsyncGenerator[Optional[Message], None]:
         """Yield Messages.
 
         Generate messages with variable timeout.
         Yield `None` on `throw()`.
 
         Keyword Arguments:
```

### Comparing `oms-mqclient-2.3.1/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.3.2/mqclient/broker_clients/rabbitmq.py`

 * *Files 9% similar despite different names*

```diff
@@ -167,43 +167,56 @@
         await super().close()
         LOGGER.debug(log_msgs.CLOSED_PUB)
 
     async def send_message(
         self,
         msg: bytes,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Send a message on a queue.
 
         Args:
             address (str): address of queue
             name (str): name of queue on address
 
         Returns:
             RawQueue: queue
         """
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
         if not self.channel:
             raise RuntimeError("queue is not connected")
 
-        await utils.auto_retry_call(
-            func=functools.partial(
-                self.channel.basic_publish,
+        def _send_msg():
+            # use wrapper function so connection references can be updated by reconnects
+            if not self.channel:
+                raise RuntimeError("queue is not connected")
+            return self.channel.basic_publish(
                 exchange="",
                 routing_key=self.queue,
                 body=msg,
-            ),
+            )
+
+        await utils.auto_retry_call(
+            func=_send_msg,
             nonretriable_conditions=lambda e: isinstance(
                 e, pika.exceptions.AMQPChannelError
             ),
             retries=retries,
             retry_delay=retry_delay,
-            close=self.close,
-            connect=self.connect,
+            close=(
+                None
+                if self.connection_can_have_multiple_unacked_messages
+                else self.close
+            ),
+            connect=(
+                None
+                if self.connection_can_have_multiple_unacked_messages
+                else self.connect
+            ),
             logger=LOGGER,
         )
         LOGGER.debug(log_msgs.SENT_MESSAGE)
 
 
 class RabbitMQSub(RabbitMQ, Sub):
     """Wrapper around queue with prefetch-queue QoS.
@@ -227,14 +240,18 @@
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
 
         if not self.channel:
             raise ConnectingFailedException("No channel to configure connection.")
 
         self.channel.basic_qos(prefetch_count=self.prefetch)
+        # https://www.rabbitmq.com/consumer-prefetch.html
+        #    Meaning of prefetch_count in RabbitMQ w/ global_qos=False:
+        #    applied separately to each new consumer on the channel
+        #
         # global_qos=False b/c using quorum queues
         # https://www.rabbitmq.com/quorum-queues.html#global-qos
 
         LOGGER.debug(log_msgs.CONNECTED_SUB)
 
     async def close(self) -> None:
         """Close connection.
@@ -260,35 +277,52 @@
         else:
             return Message(method_frame.delivery_tag, body)
 
     async def _iter_messages(
         self,
         timeout_millis: Optional[int],
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> AsyncIterator[Optional[Message]]:
         if not self.channel:
             raise RuntimeError("queue is not connected")
 
-        iterator = self.channel.consume(
-            self.queue,
-            inactivity_timeout=timeout_millis / 1000.0 if timeout_millis else None,
-        )
+        def _get_msg():
+            # use wrapper function so connection references can be updated by reconnects
+            if not self.channel:
+                raise RuntimeError("queue is not connected")
+            return next(
+                # pika smartly handles re-invocations
+                self.channel.consume(
+                    self.queue,
+                    inactivity_timeout=timeout_millis / 1000.0
+                    if timeout_millis
+                    else None,
+                )
+            )
 
         while True:
             try:
                 pika_msg = await utils.auto_retry_call(
-                    func=functools.partial(next, iterator),
+                    func=_get_msg,
                     nonretriable_conditions=lambda e: isinstance(
                         e, (pika.exceptions.AMQPChannelError, StopIteration)
                     ),
                     retries=retries,
                     retry_delay=retry_delay,
-                    close=self.close,
-                    connect=self.connect,
+                    close=(
+                        None
+                        if self.connection_can_have_multiple_unacked_messages
+                        else self.close
+                    ),
+                    connect=(
+                        None
+                        if self.connection_can_have_multiple_unacked_messages
+                        else self.connect
+                    ),
                     logger=LOGGER,
                 )
             except StopIteration:
                 LOGGER.debug(log_msgs.GETMSG_TIMEOUT_ERROR)
                 return
             if msg := RabbitMQSub._to_message(pika_msg[0], pika_msg[2]):  # type: ignore[index]
                 LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg.msg_id!r}).")
@@ -297,15 +331,15 @@
                 LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
                 yield None
 
     async def get_message(
         self,
         timeout_millis: Optional[int],
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> Optional[Message]:
         """Get a message from a queue."""
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
         if not self.channel:
             raise RuntimeError("queue is not connected")
 
         msg = None
@@ -317,15 +351,15 @@
 
         return msg
 
     async def ack_message(
         self,
         msg: Message,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Ack a message from the queue.
 
         Note that RabbitMQ acks messages in-order, so acking message 3
         of 3 in-progress messages will ack them all.
         """
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
@@ -333,30 +367,30 @@
             raise RuntimeError("queue is not connected")
 
         await utils.auto_retry_call(
             func=functools.partial(
                 self.channel.basic_ack,
                 msg.msg_id,
             ),
+            connect=None,
+            close=None,
             nonretriable_conditions=lambda e: isinstance(
                 e, pika.exceptions.AMQPChannelError
             ),
             retries=retries,
             retry_delay=retry_delay,
-            close=self.close,
-            connect=self.connect,
             logger=LOGGER,
         )
         LOGGER.debug(f"{log_msgs.ACKED_MESSAGE} ({msg.msg_id!r}).")
 
     async def reject_message(
         self,
         msg: Message,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> None:
         """Reject (nack) a message from the queue.
 
         Note that RabbitMQ acks messages in-order, so nacking message 3
         of 3 in-progress messages will nack them all.
         """
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
@@ -364,31 +398,31 @@
             raise RuntimeError("queue is not connected")
 
         await utils.auto_retry_call(
             func=functools.partial(
                 self.channel.basic_nack,
                 msg.msg_id,
             ),
+            close=None,
+            connect=None,
             nonretriable_conditions=lambda e: isinstance(
                 e, pika.exceptions.AMQPChannelError
             ),
             retries=retries,
             retry_delay=retry_delay,
-            close=self.close,
-            connect=self.connect,
             logger=LOGGER,
         )
         LOGGER.debug(f"{log_msgs.NACKED_MESSAGE} ({msg.msg_id!r}).")
 
     async def message_generator(
         self,
         timeout: int,
         propagate_error: bool,
         retries: int,
-        retry_delay: int,
+        retry_delay: float,
     ) -> AsyncGenerator[Optional[Message], None]:
         """Yield Messages.
 
         Generate messages with variable timeout.
         Yield `None` on `throw()`.
 
         Keyword Arguments:
```

### Comparing `oms-mqclient-2.3.1/mqclient/broker_clients/utils.py` & `oms-mqclient-2.3.2/mqclient/broker_clients/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,58 +2,61 @@
 
 
 import asyncio
 import inspect
 import logging
 from typing import Awaitable, Callable, Optional, TypeVar, Union
 
-from .. import log_msgs
-
 T = TypeVar("T")  # the callable/awaitable return type
 
 
+def _ci_test_retry_trigger(i: int) -> None:
+    pass
+
+
 async def auto_retry_call(
     func: Callable[[], Union[T, Awaitable[T]]],
     retries: int,
-    retry_delay: int,
-    close: Callable[[], Awaitable[None]],
-    connect: Callable[[], Awaitable[None]],
+    retry_delay: float,
     logger: logging.Logger,
-    nonretriable_conditions: Optional[Callable[[Exception], bool]] = None,
+    close: Optional[Callable[[], Awaitable[None]]],
+    connect: Optional[Callable[[], Awaitable[None]]],
+    nonretriable_conditions: Optional[Callable[[Exception], bool]],
 ) -> T:
     """Call `func` with auto-retries."""
-    retry_delay = max(retry_delay, 1)
+    retry_delay = max(retry_delay, 0.01)
     retries = max(retries, 0)
 
     for i in range(retries + 1):
-        if i > 0:
-            logger.debug(
-                f"{log_msgs.TRYCALL_CONNECTION_ERROR_TRY_AGAIN} (attempt #{i+1})..."
-            )
-
         try:
+            _ci_test_retry_trigger(i)  # only used for testing
             ret = func()
             if inspect.isawaitable(ret):
                 return await ret  # type: ignore[no-any-return]
             else:
                 return ret  # type: ignore[return-value]
         except Exception as e:
-            logger.error(e)
+            logger.exception(e)
             if nonretriable_conditions and nonretriable_conditions(e):
                 raise
             elif i == retries:
-                logger.debug(log_msgs.TRYCALL_CONNECTION_ERROR_MAX_RETRIES)
+                logger.info(
+                    f"[auto_retry_call()] {type(e)}. Reached max retries. Raising..."
+                )
                 raise
             else:
-                pass
+                logger.info(
+                    f"[auto_retry_call()] {type(e)}. Trying again. (attempt #{i+2})..."
+                )
 
         # close, wait, reconnect
-        try:
-            await close()  # the previous error could've been due to a closed connection
-        except:  # noqa: E722
-            pass
+        if close:
+            try:
+                await close()  # the previous error could've been due to a closed connection
+            except:  # noqa: E722
+                pass
         await asyncio.sleep(retry_delay)
-        await connect()
+        if connect:
+            await connect()
 
     # fall through -- this should not be reached in any situation
-    logger.debug(log_msgs.TRYCALL_CONNECTION_ERROR_MAX_RETRIES)
-    raise Exception("Max retries exceeded / connection error")
+    raise RuntimeError("unknown error in auto_retry_call()")
```

### Comparing `oms-mqclient-2.3.1/mqclient/queue.py` & `oms-mqclient-2.3.2/mqclient/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 """Queue class encapsulating a pub-sub messaging system."""
 
 import contextlib
-import functools
 import logging
 import os
 import sys
 import types
 import uuid
-from typing import (
-    Any,
-    AsyncGenerator,
-    AsyncIterator,
-    Awaitable,
-    Callable,
-    Dict,
-    Optional,
-    Type,
-)
+from typing import Any, AsyncGenerator, AsyncIterator, Dict, List, Optional, Type
 
 from . import broker_client_manager
 from . import telemetry as wtt
 from .broker_client_interface import AckException, Message, NackException, Pub, Sub
 from .config import (
     DEFAULT_EXCEPT_ERRORS,
     DEFAULT_PREFETCH,
@@ -67,15 +57,15 @@
         self,
         broker_client: str,
         address: str = "localhost",
         name: str = "",
         prefetch: int = DEFAULT_PREFETCH,
         timeout: int = DEFAULT_TIMEOUT,
         ack_timeout: Optional[int] = None,
-        retry_delay: int = DEFAULT_RETRY_DELAY,  # seconds
+        retry_delay: float = DEFAULT_RETRY_DELAY,  # seconds
         retries: int = DEFAULT_RETRIES,  # ex: 2 means 1 initial try and 2 retries
         except_errors: bool = DEFAULT_EXCEPT_ERRORS,
         auth_token: str = "",
     ) -> None:
         self._broker_client = broker_client_manager.get_broker_client(broker_client)
         self._address = address
         self._name = name if name else Queue.make_name()
@@ -91,15 +81,15 @@
         self._ack_timeout = ack_timeout
 
         # properties
         self._timeout = -1
         self.timeout = timeout
         self._retries = -1
         self.retries = retries
-        self._retry_delay = -1
+        self._retry_delay = -1.0
         self.retry_delay = retry_delay
 
         # publics
         self.except_errors = except_errors
 
     @staticmethod
     def make_name() -> str:
@@ -130,22 +120,22 @@
     def retries(self, val: int) -> None:
         LOGGER.debug(f"Setting retries to {val}")
         if val < 0:
             raise ValueError("retries must be non-negative")
         self._retries = val
 
     @property
-    def retry_delay(self) -> int:
+    def retry_delay(self) -> float:
         """Get the retry_delay value."""
         return self._retry_delay
 
     @retry_delay.setter
-    def retry_delay(self, val: int) -> None:
+    def retry_delay(self, val: float) -> None:
         LOGGER.debug(f"Setting retry_delay to {val}")
-        if val < 1:
+        if val <= 0:
             raise ValueError("retry_delay must be positive")
         self._retry_delay = val
 
     async def _create_pub_queue(self) -> Pub:
         """Wrap `self._broker_client.create_pub_queue()` with instance's
         config."""
         return await self._broker_client.create_pub_queue(
@@ -297,15 +287,15 @@
             "self._address",
             "self._name",
             "self._prefetch",
             "self.timeout",
         ]
     )
     async def open_sub_manual_acking(
-        self, use_prefetch_value: bool
+        self,
     ) -> AsyncGenerator["ManualQueueSubResource", None]:
         """Open a resource to receive messages from the queue as an iterator.
 
         This returns a context-manager with an iterator function `iter_messages()`.
         The iterator stops when no messages are received for `timeout` seconds.
         Multiple calls to `open_sub()` is okay, but reusing the returned
         instance is not.
@@ -315,21 +305,14 @@
         *Unlike `open_sub()`*, the caller is responsible for:
             - All acking and/or nacking
             - Any error handling
 
         **NOTE: unless you need to parallelize your message processing,
         use `open_sub()`**
 
-        Arguments:
-            `use_prefetch_value` - whether to use the prefetch value; `False` uses prefetch=0
-                Prefetching may be useful for short-running tasks,
-                where the bottleneck would be network delay.
-                NOTE: rabbitmq will not deliver more messages if
-                there are N un-acked messages (N = prefetch, N > 0)
-
         Examples:
             async with queue.open_sub_manual_acking() as sub:
                 async for msg in sub.iter_messages():
                     print(msg.data)
                     sub.ack(msg)
                     # if you choose not to nack on an error,
                     # the broker will take longer to redeliver
@@ -339,56 +322,22 @@
                     try:
                         process_message(msg.data)
                     except Exception:
                         await sub.nack(msg)
                     else:
                         await sub.ack(msg)
 
-            async with queue.open_sub_manual_acking(ack_pending_limit=5) as sub:
-                pending = []
-                async for msg in sub.iter_messages():
-                    try:
-                        process_message(msg.data)
-                        pending.append(msg)
-                    except Exception:
-                        await sub.nack(msg)
-
-                    if len(pending) == 3:
-                        for msg in pending:
-                            await sub.ack(msg)
-                        pending = []
-
-                for msg in pending:
-                    await sub.ack(msg)
-
         Returns:
             ManualQueueSubResource -- context manager w/ iterator function
         """
-        sub = await self._create_sub_queue(
-            # if prefetch=N (N>0), pika will not deliver more messages
-            #   if there are N un-acked messages
-            #
-            #   We could implement logic that checks if this condition is met
-            #   but that would go against the intention of the "manual" usage
-            prefetch_override=(None if use_prefetch_value else 0)
-        )
-
+        resource = ManualQueueSubResource(self)
         try:
-            yield ManualQueueSubResource(
-                functools.partial(
-                    sub.get_message,
-                    self.timeout * 1000,
-                    retries=self.retries,
-                    retry_delay=self.retry_delay,
-                ),
-                functools.partial(self._safe_ack, sub),
-                functools.partial(self._safe_nack, sub),
-            )
+            yield resource
         finally:
-            await sub.close()
+            await resource.close()
 
     @contextlib.asynccontextmanager  # needs to wrap @wtt stuff to span children correctly
     @wtt.spanned(
         these=[
             "self._broker_client",
             "self._address",
             "self._name",
@@ -469,15 +418,15 @@
 class EmptyQueueException(Exception):
     """Raised when the queue is empty."""
 
 
 class QueuePubResource:
     """A manager class around `Pub.send_message()`."""
 
-    def __init__(self, pub: Pub, retries: int, retry_delay: int):
+    def __init__(self, pub: Pub, retries: int, retry_delay: float):
         self.pub = pub
         self.retries = retries
         self.retry_delay = retry_delay
 
     @wtt.spanned(kind=wtt.SpanKind.PRODUCER)
     async def send(self, data: Any) -> None:
         """Send a message."""
@@ -489,51 +438,77 @@
             retry_delay=self.retry_delay,
         )
 
 
 class ManualQueueSubResource:
     """A manager class around `Sub.get_message()`."""
 
-    def __init__(
-        self,
-        get_message_function: Callable[[], Awaitable[Optional[Message]]],
-        ack_function: Callable[[Message], Awaitable[None]],
-        nack_function: Callable[[Message], Awaitable[None]],
-    ) -> None:
-        self._get_message = get_message_function
-        self._ack_function = ack_function
-        self._nack_function = nack_function
+    def __init__(self, queue: Queue) -> None:
+        self.queue = queue
+        self._subs: Dict[Sub, List[int]] = {}
 
     async def iter_messages(self) -> AsyncIterator[Message]:
         """Yield a message."""
 
         @wtt.spanned(
             kind=wtt.SpanKind.CONSUMER,
             carrier="msg.headers",
             carrier_relation=wtt.CarrierRelation.LINK,
         )
         def add_span_link(msg: Message) -> Message:
             return msg
 
         while True:
-            raw_msg = await self._get_message()
-            if not raw_msg:  # no message -> close and exit
-                return
+            for sub in self._subs:
+                if raw_msg := await self._get(sub):  # got message from sub -> done
+                    self._subs[sub].append(id(raw_msg))
+                    break
+            else:  # no sub gave a message (didn't break) -> try w/ new sub
+                newb = await self.queue._create_sub_queue()
+                # keep connection open for other unacked messages
+                newb.connection_can_have_multiple_unacked_messages = True
+                if not (raw_msg := await self._get(newb)):  # no message -> close & exit
+                    await newb.close()
+                    return
+                self._subs[newb] = [id(raw_msg)]
 
             msg = add_span_link(raw_msg)  # got a message -> link and proceed
             LOGGER.info(f"Received Message: {_message_size_message(msg)}")
             yield msg
 
+    async def _get(self, sub: Sub) -> Optional[Message]:
+        return await sub.get_message(
+            self.queue.timeout * 1000,
+            retries=self.queue.retries,
+            retry_delay=self.queue.retry_delay,
+        )
+
+    def _get_sub(self, msg: Message) -> Sub:
+        subs = [s for s, addrs in self._subs.items() if id(msg) in addrs]
+        if not subs:
+            raise ValueError("message cannot be mapped to a sub")
+        elif len(subs) != 1:
+            raise RuntimeError("message found in more than one sub")
+        else:
+            return subs[0]
+
     async def ack(self, msg: Message) -> None:
         """Acknowledge the message."""
-        await self._ack_function(msg)
+        sub = self._get_sub(msg)
+        await self.queue._safe_ack(sub, msg)
 
     async def nack(self, msg: Message) -> None:
-        """Acknowledge the message."""
-        await self._nack_function(msg)
+        """Reject/nack the message."""
+        sub = self._get_sub(msg)
+        await self.queue._safe_nack(sub, msg)
+
+    async def close(self) -> None:
+        """Close resource."""
+        for sub in self._subs:
+            await sub.close()
 
 
 class QueueSubResource:
     """An async context-manager generator, wraps `Sub.message_generator()`."""
 
     RUNTIME_ERROR_CONTEXT_STRING = (
         "'QueueSubResource' object's runtime "
```

### Comparing `oms-mqclient-2.3.1/mqclient/telemetry.py` & `oms-mqclient-2.3.2/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.3.2/oms_mqclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.3.1
+Version: 2.3.2
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.3.1/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.3.2/oms_mqclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/setup.cfg` & `oms-mqclient-2.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.3.2/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.3.2/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,66 @@
 """Run integration tests for given broker_client, on Queue class."""
 
 # pylint:disable=invalid-name,too-many-public-methods,redefined-outer-name,unused-import
 
 import asyncio
 import logging
+import random
 from multiprocessing.dummy import Pool as ThreadPool
 from typing import Any, List, Optional
+from unittest.mock import patch
 
 import asyncstdlib as asl
 import pytest
 from mqclient.queue import Queue
 
 from .utils import (
     DATA_LIST,
     _log_recv,
     _log_recv_multiple,
     _log_send,
     all_were_received,
 )
 
+#
+# retry stuff
+#
+
+
+CI_TEST_RETRY_TRIGGER = "mqclient.broker_clients.utils._ci_test_retry_trigger"
+
+
+class FailFirstTryException(Exception):
+    pass
+
+
+def fail_first_try(attempt: int) -> None:
+    if attempt == 0:
+        raise FailFirstTryException()
+
+
+#
+# tests
+#
+
 
 class PubSubQueue:
     """Integration test suite for Queue objects."""
 
     broker_client: str = ""
 
     ###########################################################################
     # tests 000 - 099:
     #
     # Testing scenarios with different numbers of sub and/or pubs
     # to see no data loss
     ###########################################################################
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_010(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, one sub."""
         all_recvd: List[Any] = []
 
         pub_sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         async with pub_sub.open_pub() as p:
             await p.send(DATA_LIST[0])
@@ -57,14 +81,15 @@
                 print(f"{i}: `{d}`")
                 all_recvd.append(_log_recv(d))
                 # assert d == DATA_LIST[i]  # we don't guarantee order
 
         assert all_were_received(all_recvd, [DATA_LIST[0]] + DATA_LIST)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_011(self, queue_name: str, auth_token: str) -> None:
         """Test an individual pub and an individual sub."""
         all_recvd: List[Any] = []
 
         pub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         async with pub.open_pub() as p:
             await p.send(DATA_LIST[0])
@@ -86,14 +111,15 @@
                 print(f"{i}: `{d}`")
                 all_recvd.append(_log_recv(d))
                 # assert d == DATA_LIST[i]  # we don't guarantee order
 
         assert all_were_received(all_recvd, [DATA_LIST[0]] + DATA_LIST)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_012(self, queue_name: str, auth_token: str) -> None:
         """Failure-test one pub, two subs (one subscribed to wrong queue)."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
@@ -110,14 +136,15 @@
         ).open_sub_one() as d:
             all_recvd.append(_log_recv(d))
             assert d == DATA_LIST[0]
 
         assert all_were_received(all_recvd, [DATA_LIST[0]])
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_020(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, ordered/alternatingly."""
         all_recvd: List[Any] = []
 
         # for each send, create and receive message via a new sub
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
@@ -158,38 +185,42 @@
         with ThreadPool(num_subs) as pool:
             received_data = pool.map(start_recv_thread, range(num_subs))
         all_recvd.extend(item for sublist in received_data for item in sublist)
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_021_fewer(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
 
         Fewer subs than messages.
         """
         await self._test_021(queue_name, len(DATA_LIST) // 2, auth_token)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_021_same(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
 
         Same number of subs as messages.
         """
         await self._test_021(queue_name, len(DATA_LIST), auth_token)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_021_more(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
 
         More subs than messages.
         """
         await self._test_021(queue_name, len(DATA_LIST) ** 2, auth_token)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_022(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
 
         Use the same number of subs as number of messages.
         """
         all_recvd: List[Any] = []
 
@@ -212,14 +243,15 @@
 
         with ThreadPool(len(DATA_LIST)) as pool:
             all_recvd = pool.map(start_recv_thread, range(len(DATA_LIST)))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_023(self, queue_name: str, auth_token: str) -> None:
         """Failure-test one pub, and too many subs.
 
         More subs than messages with `open_sub_one()` will raise an
         exception.
         """
         all_recvd: List[Any] = []
@@ -247,14 +279,15 @@
         # Extra Sub
         with pytest.raises(Exception):
             await recv_thread(-1)
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_030(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, one sub, ordered/alternatingly."""
         all_recvd: List[Any] = []
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
 
         for data in DATA_LIST:
@@ -272,14 +305,15 @@
 
             assert len(received_data) == 1
             assert data == received_data[0]
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_031(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, one sub, unordered (front-loaded sending)."""
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
             async with Queue(
                 self.broker_client, name=queue_name, auth_token=auth_token
@@ -292,14 +326,15 @@
         async with sub.open_sub() as gen:
             received_data = [m async for m in gen]
         all_recvd.extend(_log_recv_multiple(received_data))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_040(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, ordered/alternatingly.
 
         Use the same number of pubs as subs.
         """
         all_recvd: List[Any] = []
 
@@ -318,14 +353,15 @@
 
             assert len(received_data) == 1
             assert data == received_data[0]
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_041(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, unordered (front-loaded sending).
 
         Use the same number of pubs as subs.
         """
         all_recvd: List[Any] = []
 
@@ -341,14 +377,15 @@
                 self.broker_client, name=queue_name, auth_token=auth_token
             ).open_sub_one() as d:
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_042(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, unordered (front-loaded sending).
 
         Use the more pubs than subs.
         """
         all_recvd: List[Any] = []
 
@@ -364,14 +401,15 @@
                 sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
             async with sub.open_sub_one() as d:
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_043(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, unordered (front-loaded sending).
 
         Use the fewer pubs than subs.
         """
         all_recvd: List[Any] = []
 
@@ -388,14 +426,15 @@
                 self.broker_client, name=queue_name, auth_token=auth_token
             ).open_sub_one() as d:
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_050(self, queue_name: str, auth_token: str) -> None:
         """Test_20 with variable prefetching.
 
         One pub, multiple subs.
         """
         all_recvd: List[Any] = []
 
@@ -417,14 +456,15 @@
                     async with sub.open_sub_one() as d:
                         all_recvd.append(_log_recv(d))
                         assert d == data
 
         assert all_were_received(all_recvd, DATA_LIST * ((len(DATA_LIST) * 2) - 1))
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_051(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, with prefetching.
 
         Prefetching should have no visible affect.
         """
         all_recvd: List[Any] = []
 
@@ -457,14 +497,15 @@
     ###########################################################################
     # tests 100 - 199:
     #
     # Tests for open_sub()
     ###########################################################################
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_100(self, queue_name: str, auth_token: str) -> None:
         """Test open_sub() fail and recovery, with multiple open_sub()
         calls."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
@@ -498,14 +539,15 @@
                 all_recvd.append(_log_recv(d))
                 # assert d == DATA_LIST[i]  # we don't guarantee order
         assert reused
         print(all_recvd)
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_101(self, queue_name: str, auth_token: str) -> None:
         """Test open_sub() fail and recovery, with error propagation."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
@@ -543,14 +585,15 @@
                 all_recvd.append(_log_recv(d))
                 # assert d == DATA_LIST[i]  # we don't guarantee order
         assert reused
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_110__fail(self, queue_name: str, auth_token: str) -> None:
         """Failure-test open_sub() with reusing a 'QueueSubResource'
         instance."""
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
@@ -569,14 +612,15 @@
 
         # continue where we left off
         with pytest.raises(RuntimeError):
             async with recv_gen as gen:
                 assert 0  # we should never get here
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_120_break(self, queue_name: str, auth_token: str) -> None:
         """Test open_sub() with a `break` statement."""
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
@@ -601,28 +645,27 @@
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     ###########################################################################
     # tests 200 - 299:
     #
-    # Tests for open_sub_manual_acking(use_prefetch_value)
+    # Tests for open_sub_manual_acking()
     ###########################################################################
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     @pytest.mark.parametrize("sub_queue_prefetch", [None, 0, 1, 2, 50])
-    @pytest.mark.parametrize("use_prefetch_value", [False, True])
     async def test_200__ideal(
         self,
         queue_name: str,
         auth_token: str,
         sub_queue_prefetch: Optional[int],
-        use_prefetch_value: bool,
     ) -> None:
-        """Test open_sub_manual_acking(use_prefetch_value) ideal scenario."""
+        """Test open_sub_manual_acking() ideal scenario."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
@@ -638,36 +681,35 @@
         else:
             sub = Queue(
                 self.broker_client,
                 name=queue_name,
                 auth_token=auth_token,
             )
         sub.timeout = 1
-        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
+        async with sub.open_sub_manual_acking() as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 print(f"{i}: `{msg.data}`")
                 all_recvd.append(_log_recv(msg.data))
                 # assert msg.data == DATA_LIST[i]  # we don't guarantee order
                 await gen.ack(msg)
 
         print(all_recvd)
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     @pytest.mark.parametrize("sub_queue_prefetch", [None, 0, 1, 2, 50])
-    @pytest.mark.parametrize("use_prefetch_value", [False, True])
     async def test_202__delayed_mixed_acking_nacking(
         self,
         queue_name: str,
         auth_token: str,
         sub_queue_prefetch: Optional[int],
-        use_prefetch_value: bool,
     ) -> None:
-        """Test open_sub_manual_acking(use_prefetch_value) fail and immediate
-        recovery with multi-tasking, with mixed acking and nacking."""
+        """Test open_sub_manual_acking() fail and immediate recovery with
+        multi-tasking, with mixed acking and nacking."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
@@ -686,15 +728,15 @@
         else:
             sub = Queue(
                 self.broker_client,
                 name=queue_name,
                 auth_token=auth_token,
             )
         sub.timeout = 1
-        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
+        async with sub.open_sub_manual_acking() as gen:
             pending = []
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 try:
                     # DO WORK!
                     print(f"{i}: `{msg.data}`")
                     if i % 3 == 0:  # nack every 1/3
                         raise TestException()
@@ -709,45 +751,27 @@
                     print(f"nack {i}: `{msg.data}`")
                     await gen.nack(msg)
 
             for msg in pending:  # messages with index not %2 nor %3, (1,5,7,...)
                 await gen.ack(msg)
 
         print(all_recvd)
-        if (
-            self.broker_client == "rabbitmq"
-            and use_prefetch_value
-            and sub_queue_prefetch  # int, >0
-        ):  # acked every 1/2 before we got kicked out
-            try:
-                indexes_unacked = [
-                    x
-                    for x in range(int(len(DATA_LIST) * (3 / 2)))  # math.ceil?
-                    if not (x % 2 == 0 or x % 3 == 0)
-                ]
-                print(indexes_unacked)
-                assert i == indexes_unacked[sub_queue_prefetch - 1]  # 0-index
-            except IndexError:
-                assert i + 1 == len(DATA_LIST) * (3 / 2)
-            assert len(all_recvd) == i - (i // 3)  # len == i - # of nacks
-        else:
-            assert all_were_received(all_recvd)
+        assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     @pytest.mark.parametrize("sub_queue_prefetch", [None, 0, 1, 2, 50])
-    @pytest.mark.parametrize("use_prefetch_value", [False, True])
     async def test_204__post_ack(
         self,
         queue_name: str,
         auth_token: str,
         sub_queue_prefetch: Optional[int],
-        use_prefetch_value: bool,
     ) -> None:
-        """Test open_sub_manual_acking(use_prefetch_value) where messages
-        aren't acked until after all have been received."""
+        """Test open_sub_manual_acking() where messages aren't acked until
+        after all have been received."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
@@ -764,60 +788,54 @@
             sub = Queue(
                 self.broker_client,
                 name=queue_name,
                 auth_token=auth_token,
             )
         sub.timeout = 1
         to_ack = []
-        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
+        async with sub.open_sub_manual_acking() as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 print(f"{i}: `{msg.data}`")
                 all_recvd.append(_log_recv(msg.data))
                 to_ack.append(msg)
                 # assert msg.data == DATA_LIST[i]  # we don't guarantee order
 
-            for i, msg in enumerate(to_ack):
-                print(f"ack {i}: `{msg.data}`")
+            iter_em = list(enumerate(to_ack))
+            random.shuffle(iter_em)
+            for i, msg in iter_em:
+                print(f"ack {i} (shuffled): `{msg.data}`")
                 await gen.ack(msg)
 
         print(all_recvd)
-        if (
-            self.broker_client == "rabbitmq"
-            and use_prefetch_value
-            and sub_queue_prefetch  # int, >0
-        ):  # got kicked out when prefetch was met
-            assert len(all_recvd) == min(sub_queue_prefetch, len(DATA_LIST))
-        else:
-            assert all_were_received(all_recvd)
+        assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    @pytest.mark.parametrize("use_prefetch_value", [False, True])
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_210__immediate_recovery(
         self,
         queue_name: str,
         auth_token: str,
-        use_prefetch_value: bool,
     ) -> None:
-        """Test open_sub_manual_acking(use_prefetch_value) fail and immediate
-        recovery, with nacking."""
+        """Test open_sub_manual_acking() fail and immediate recovery, with
+        nacking."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
                 _log_send(d)
 
         class TestException(Exception):  # pylint: disable=C0115
             pass
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         sub.timeout = 1
-        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
+        async with sub.open_sub_manual_acking() as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 try:
                     # DO WORK!
                     print(f"{i}: `{msg.data}`")
                     if i == 2:
                         raise TestException()
                     all_recvd.append(_log_recv(msg.data))
@@ -827,23 +845,22 @@
                 else:
                     await gen.ack(msg)
 
         print(all_recvd)
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    @pytest.mark.parametrize("use_prefetch_value", [False, True])
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_220__posthoc_recovery(
         self,
         queue_name: str,
         auth_token: str,
-        use_prefetch_value: bool,
     ) -> None:
-        """Test open_sub_manual_acking(use_prefetch_value) fail and post-hoc
-        recovery, with nacking."""
+        """Test open_sub_manual_acking() fail and post-hoc recovery, with
+        nacking."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
@@ -852,15 +869,15 @@
         class TestException(Exception):  # pylint: disable=C0115
             pass
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         excepted = False
         sub.timeout = 1
         # sub.except_errors = False  # has no effect
-        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
+        async with sub.open_sub_manual_acking() as gen:
             try:
                 async for i, msg in asl.enumerate(gen.iter_messages()):
                     print(f"{i}: `{msg.data}`")
                     if i == 2:
                         raise TestException()
                     all_recvd.append(_log_recv(msg.data))
                     # assert msg.data == DATA_LIST[i]  # we don't guarantee order
@@ -871,35 +888,33 @@
         assert excepted
 
         logging.warning("Round 2!")
 
         # continue where we left off
         posthoc = False
         sub.timeout = 1
-        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
+        async with sub.open_sub_manual_acking() as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 print(f"{i}: `{msg.data}`")
                 posthoc = True
                 all_recvd.append(_log_recv(msg.data))
                 # assert msg.data == DATA_LIST[i]  # we don't guarantee order
                 await gen.ack(msg)
         assert posthoc
         print(all_recvd)
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    @pytest.mark.parametrize("use_prefetch_value", [False, True])
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_221__posthoc_recovery__fail(
         self,
         queue_name: str,
         auth_token: str,
-        use_prefetch_value: bool,
     ) -> None:
-        """Test open_sub_manual_acking(use_prefetch_value) fail, post-hoc
-        recovery, then fail.
+        """Test open_sub_manual_acking() fail, post-hoc recovery, then fail.
 
         Final fail is due to not nacking.
         """
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
@@ -911,15 +926,15 @@
         class TestException(Exception):  # pylint: disable=C0115
             pass
 
         errored_msg = None
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         excepted = False
-        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
+        async with sub.open_sub_manual_acking() as gen:
             try:
                 async for i, msg in asl.enumerate(gen.iter_messages()):
                     print(f"{i}: `{msg.data}`")
                     if i == 2:
                         errored_msg = msg.data
                         raise TestException()
                     all_recvd.append(_log_recv(msg.data))
@@ -931,15 +946,15 @@
         assert excepted
 
         logging.warning("Round 2!")
 
         # continue where we left off
         posthoc = False
         sub.timeout = 1
-        async with sub.open_sub_manual_acking(use_prefetch_value) as gen:
+        async with sub.open_sub_manual_acking() as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 print(f"{i}: `{msg.data}`")
                 posthoc = True
                 all_recvd.append(_log_recv(msg.data))
                 # assert msg.data == DATA_LIST[i]  # we don't guarantee order
                 await gen.ack(msg)
         assert posthoc
@@ -949,33 +964,32 @@
         # This is difficult to test -- all we can tell is if it is one of these scenarios
         print(all_recvd)
         assert all_were_received(all_recvd) or (
             all_were_received(all_recvd + [errored_msg])
         )
 
     @pytest.mark.asyncio
-    @pytest.mark.parametrize("use_prefetch_value", [False, True])
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_230__fail_bad_usage(
         self,
         queue_name: str,
         auth_token: str,
-        use_prefetch_value: bool,
     ) -> None:
-        """Failure-test open_sub_manual_acking(use_prefetch_value) with reusing
-        a 'QueueSubResource' instance."""
+        """Failure-test open_sub_manual_acking() with reusing a
+        'QueueSubResource' instance."""
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
                 _log_send(d)
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         sub.timeout = 1
-        recv_gen = sub.open_sub_manual_acking(use_prefetch_value)
+        recv_gen = sub.open_sub_manual_acking()
         async with recv_gen as gen:
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 print(f"{i}: `{msg.data}`")
                 # assert msg.data == DATA_LIST[i]  # we don't guarantee order
                 await gen.ack(msg)
 
         logging.warning("Round 2!")
```

### Comparing `oms-mqclient-2.3.1/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.3.2/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.3.2/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/tests/integrate/conftest.py` & `oms-mqclient-2.3.2/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/tests/integrate/test_nats.py` & `oms-mqclient-2.3.2/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/tests/integrate/test_pulsar.py` & `oms-mqclient-2.3.2/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.3.2/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.3.2/tests/unit/pulsar/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.1/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.3.2/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files identical despite different names*

