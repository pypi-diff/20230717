# Comparing `tmp/edcpy-0.1.1a0.tar.gz` & `tmp/edcpy-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edcpy-0.1.1a0.tar", max compression
+gzip compressed data, was "edcpy-0.1.1a1.tar", max compression
```

## Comparing `edcpy-0.1.1a0.tar` & `edcpy-0.1.1a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      113 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/README.md
--rw-r--r--   0        0        0        0 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/__init__.py
--rw-r--r--   0        0        0     5959 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/backend.py
--rw-r--r--   0        0        0     5233 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/config.py
--rw-r--r--   0        0        0    10682 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/keycloak.py
--rw-r--r--   0        0        0     4019 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/messaging.py
--rw-r--r--   0        0        0        0 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/models/__init__.py
--rw-r--r--   0        0        0     1511 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/models/asset.py
--rw-r--r--   0        0        0      713 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/models/contract_definition.py
--rw-r--r--   0        0        0     1454 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/models/contract_negotiation.py
--rw-r--r--   0        0        0      803 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/models/data_plane_instance.py
--rw-r--r--   0        0        0      627 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/models/policy_definition.py
--rw-r--r--   0        0        0     2008 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/models/transfer_process.py
--rw-r--r--   0        0        0    11828 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/orchestrator.py
--rw-r--r--   0        0        0      245 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/edcpy/utils.py
--rw-r--r--   0        0        0      978 2023-07-14 09:48:11.819882 edcpy-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 edcpy-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/__init__.py
+-rw-r--r--   0        0        0     5959 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/backend.py
+-rw-r--r--   0        0        0     5233 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/config.py
+-rw-r--r--   0        0        0    10682 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/keycloak.py
+-rw-r--r--   0        0        0     4076 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/messaging.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/__init__.py
+-rw-r--r--   0        0        0     1511 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/asset.py
+-rw-r--r--   0        0        0      713 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/contract_definition.py
+-rw-r--r--   0        0        0     1454 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/contract_negotiation.py
+-rw-r--r--   0        0        0      803 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/data_plane_instance.py
+-rw-r--r--   0        0        0      627 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/policy_definition.py
+-rw-r--r--   0        0        0     2008 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/transfer_process.py
+-rw-r--r--   0        0        0    11828 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/orchestrator.py
+-rw-r--r--   0        0        0      245 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/utils.py
+-rw-r--r--   0        0        0      978 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 edcpy-0.1.1a1/PKG-INFO
```

### Comparing `edcpy-0.1.1a0/edcpy/backend.py` & `edcpy-0.1.1a1/edcpy/backend.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a0/edcpy/config.py` & `edcpy-0.1.1a1/edcpy/config.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a0/edcpy/keycloak.py` & `edcpy-0.1.1a1/edcpy/keycloak.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a0/edcpy/messaging.py` & `edcpy-0.1.1a1/edcpy/messaging.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     def http_method(self) -> str:
         ret = (
             self.auth_code_decoded.get("dad", {})
             .get("properties", {})
             .get("method", None)
         )
 
-        assert ret is not None, "Could not find HTTP method in auth code"
+        if ret is None:
+            raise Exception("Could not find HTTP method in auth code")
 
         return ret
 
     @property
     def request_args(self) -> dict:
         return {
             "method": self.http_method,
@@ -74,15 +75,17 @@
     http_push_queue_name: str = DEFAULT_HTTP_PUSH_QUEUE_NAME,
     http_pull_queue_routing_key: str = f"{BASE_HTTP_PULL_QUEUE_ROUTING_KEY}.#",
     http_push_queue_routing_key: str = f"{BASE_HTTP_PUSH_QUEUE_ROUTING_KEY}.#",
     http_pull_handler: Union[callable, None] = None,
     http_push_handler: Union[callable, None] = None,
 ) -> MessagingApp:
     rabbit_url = AppConfig.from_environ().rabbit_url
-    assert rabbit_url, "RabbitMQ URL is not set"
+
+    if not rabbit_url:
+        raise Exception("RabbitMQ URL is not set")
 
     _logger.info(f"Connecting to RabbitMQ at {rabbit_url}")
     broker = RabbitBroker(rabbit_url, logger=_logger)
     app = PropanApp(broker, logger=_logger)
 
     _logger.info(f"Declaring exchange {exchange_name}")
 
@@ -134,9 +137,9 @@
     try:
         msg_app = await start_messaging_app(*args, **kwargs)
         yield msg_app
     finally:
         try:
             await msg_app.broker.close()
             _logger.debug("Closed messaging app broker")
-        except:
+        except Exception:
             _logger.warning("Could not close messaging app broker", exc_info=True)
```

### Comparing `edcpy-0.1.1a0/edcpy/models/asset.py` & `edcpy-0.1.1a1/edcpy/models/asset.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a0/edcpy/models/contract_definition.py` & `edcpy-0.1.1a1/edcpy/models/contract_definition.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a0/edcpy/models/contract_negotiation.py` & `edcpy-0.1.1a1/edcpy/models/contract_negotiation.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a0/edcpy/models/data_plane_instance.py` & `edcpy-0.1.1a1/edcpy/models/data_plane_instance.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a0/edcpy/models/policy_definition.py` & `edcpy-0.1.1a1/edcpy/models/policy_definition.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a0/edcpy/models/transfer_process.py` & `edcpy-0.1.1a1/edcpy/models/transfer_process.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a0/edcpy/orchestrator.py` & `edcpy-0.1.1a1/edcpy/orchestrator.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a0/pyproject.toml` & `edcpy-0.1.1a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edcpy"
-version = "0.1.1a0"
+version = "0.1.1a1"
 description = "Package that provides a series of utilities to facilitate interaction with the Management and Control APIs of an EDC connector"
 authors = ["Andres Garcia Mangas <andres.garcia@fundacionctic.org>"]
 license = "EUPL-1.2"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `edcpy-0.1.1a0/PKG-INFO` & `edcpy-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edcpy
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: Package that provides a series of utilities to facilitate interaction with the Management and Control APIs of an EDC connector
 License: EUPL-1.2
 Author: Andres Garcia Mangas
 Author-email: andres.garcia@fundacionctic.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
```

