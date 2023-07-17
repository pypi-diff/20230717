# Comparing `tmp/yellowbox-0.8.4.tar.gz` & `tmp/yellowbox-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowbox-0.8.4.tar", max compression
+gzip compressed data, was "yellowbox-0.8.5.tar", max compression
```

## Comparing `yellowbox-0.8.4.tar` & `yellowbox-0.8.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1081 2023-07-10 14:48:16.923393 yellowbox-0.8.4/LICENSE
--rw-r--r--   0        0        0     1265 2023-07-10 14:48:16.923393 yellowbox-0.8.4/README.md
--rw-r--r--   0        0        0     4879 2023-07-10 14:48:16.923393 yellowbox-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      728 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/__init__.py
--rw-r--r--   0        0        0      236 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/_pytest.py
--rw-r--r--   0        0        0       22 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/_version.py
--rw-r--r--   0        0        0      546 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/clients.py
--rw-r--r--   0        0        0    10257 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/containers.py
--rw-r--r--   0        0        0        0 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/__init__.py
--rw-r--r--   0        0        0     2348 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/aerospike.py
--rw-r--r--   0        0        0     4642 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/azure_storage.py
--rw-r--r--   0        0        0     6025 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/fake_gcs.py
--rw-r--r--   0        0        0    10016 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/http_server.py
--rw-r--r--   0        0        0     5116 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/kafka.py
--rw-r--r--   0        0        0    10090 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/logstash.py
--rw-r--r--   0        0        0     2404 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/mssql.py
--rw-r--r--   0        0        0     3726 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/postgresql.py
--rw-r--r--   0        0        0     4619 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/rabbit_mq.py
--rw-r--r--   0        0        0     3234 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/redis.py
--rw-r--r--   0        0        0     7692 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/sql_base.py
--rw-r--r--   0        0        0     5597 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/vault.py
--rw-r--r--   0        0        0      813 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/__init__.py
--rw-r--r--   0        0        0     4005 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/class_endpoint.py
--rw-r--r--   0        0        0    13917 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/endpoints.py
--rw-r--r--   0        0        0    15196 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/http_request_capture.py
--rw-r--r--   0        0        0     7772 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/request_capture.py
--rw-r--r--   0        0        0     3812 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/util.py
--rw-r--r--   0        0        0    12586 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/webserver.py
--rw-r--r--   0        0        0    19729 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/ws_request_capture.py
--rw-r--r--   0        0        0    14228 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/websocket.py
--rw-r--r--   0        0        0     3456 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/image_build.py
--rw-r--r--   0        0        0     3104 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/networks.py
--rw-r--r--   0        0        0        0 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/py.typed
--rw-r--r--   0        0        0     3543 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/retry.py
--rw-r--r--   0        0        0      578 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/service.py
--rw-r--r--   0        0        0     7596 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/subclasses.py
--rw-r--r--   0        0        0     2003 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/utils.py
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 yellowbox-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-17 13:43:56.956096 yellowbox-0.8.5/LICENSE
+-rw-r--r--   0        0        0     1265 2023-07-17 13:43:56.956096 yellowbox-0.8.5/README.md
+-rw-r--r--   0        0        0     4879 2023-07-17 13:43:56.960096 yellowbox-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0      728 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/__init__.py
+-rw-r--r--   0        0        0      236 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/_pytest.py
+-rw-r--r--   0        0        0       22 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/_version.py
+-rw-r--r--   0        0        0      546 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/clients.py
+-rw-r--r--   0        0        0    10257 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/containers.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/extras/__init__.py
+-rw-r--r--   0        0        0     2348 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/extras/aerospike.py
+-rw-r--r--   0        0        0     4642 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/extras/azure_storage.py
+-rw-r--r--   0        0        0     6025 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/extras/fake_gcs.py
+-rw-r--r--   0        0        0    10016 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/extras/http_server.py
+-rw-r--r--   0        0        0     5116 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/extras/kafka.py
+-rw-r--r--   0        0        0    10090 2023-07-17 13:43:56.960096 yellowbox-0.8.5/yellowbox/extras/logstash.py
+-rw-r--r--   0        0        0     2404 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/mssql.py
+-rw-r--r--   0        0        0     3726 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/postgresql.py
+-rw-r--r--   0        0        0     4619 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/rabbit_mq.py
+-rw-r--r--   0        0        0     3234 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/redis.py
+-rw-r--r--   0        0        0     7692 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/sql_base.py
+-rw-r--r--   0        0        0     5597 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/vault.py
+-rw-r--r--   0        0        0      813 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/webserver/__init__.py
+-rw-r--r--   0        0        0     4005 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/webserver/class_endpoint.py
+-rw-r--r--   0        0        0    13917 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/webserver/endpoints.py
+-rw-r--r--   0        0        0    15196 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/webserver/http_request_capture.py
+-rw-r--r--   0        0        0     7772 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/webserver/request_capture.py
+-rw-r--r--   0        0        0     3812 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/webserver/util.py
+-rw-r--r--   0        0        0    12586 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/webserver/webserver.py
+-rw-r--r--   0        0        0    19729 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/webserver/ws_request_capture.py
+-rw-r--r--   0        0        0    14228 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/extras/websocket.py
+-rw-r--r--   0        0        0     3456 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/image_build.py
+-rw-r--r--   0        0        0     3104 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/networks.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/py.typed
+-rw-r--r--   0        0        0     3543 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/retry.py
+-rw-r--r--   0        0        0      578 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/service.py
+-rw-r--r--   0        0        0     7697 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/subclasses.py
+-rw-r--r--   0        0        0     2003 2023-07-17 13:43:56.964096 yellowbox-0.8.5/yellowbox/utils.py
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 yellowbox-0.8.5/PKG-INFO
```

### Comparing `yellowbox-0.8.4/LICENSE` & `yellowbox-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/README.md` & `yellowbox-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/pyproject.toml` & `yellowbox-0.8.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yellowbox"
-version = "0.8.4"
+version = "0.8.5"
 description = ""
 authors = ["biocatch ltd"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/biocatchltd/yellowbox"
 
 [tool.poetry.dependencies]
```

### Comparing `yellowbox-0.8.4/yellowbox/__init__.py` & `yellowbox-0.8.5/yellowbox/__init__.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/clients.py` & `yellowbox-0.8.5/yellowbox/clients.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/containers.py` & `yellowbox-0.8.5/yellowbox/containers.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/aerospike.py` & `yellowbox-0.8.5/yellowbox/extras/aerospike.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/azure_storage.py` & `yellowbox-0.8.5/yellowbox/extras/azure_storage.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/fake_gcs.py` & `yellowbox-0.8.5/yellowbox/extras/fake_gcs.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/http_server.py` & `yellowbox-0.8.5/yellowbox/extras/http_server.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/kafka.py` & `yellowbox-0.8.5/yellowbox/extras/kafka.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/logstash.py` & `yellowbox-0.8.5/yellowbox/extras/logstash.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/mssql.py` & `yellowbox-0.8.5/yellowbox/extras/mssql.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/postgresql.py` & `yellowbox-0.8.5/yellowbox/extras/postgresql.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/rabbit_mq.py` & `yellowbox-0.8.5/yellowbox/extras/rabbit_mq.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/redis.py` & `yellowbox-0.8.5/yellowbox/extras/redis.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/sql_base.py` & `yellowbox-0.8.5/yellowbox/extras/sql_base.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/vault.py` & `yellowbox-0.8.5/yellowbox/extras/vault.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/webserver/__init__.py` & `yellowbox-0.8.5/yellowbox/extras/webserver/__init__.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/webserver/class_endpoint.py` & `yellowbox-0.8.5/yellowbox/extras/webserver/class_endpoint.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/webserver/endpoints.py` & `yellowbox-0.8.5/yellowbox/extras/webserver/endpoints.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/webserver/http_request_capture.py` & `yellowbox-0.8.5/yellowbox/extras/webserver/http_request_capture.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/webserver/request_capture.py` & `yellowbox-0.8.5/yellowbox/extras/webserver/request_capture.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/webserver/util.py` & `yellowbox-0.8.5/yellowbox/extras/webserver/util.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/webserver/webserver.py` & `yellowbox-0.8.5/yellowbox/extras/webserver/webserver.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/webserver/ws_request_capture.py` & `yellowbox-0.8.5/yellowbox/extras/webserver/ws_request_capture.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/extras/websocket.py` & `yellowbox-0.8.5/yellowbox/extras/websocket.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/image_build.py` & `yellowbox-0.8.5/yellowbox/image_build.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/networks.py` & `yellowbox-0.8.5/yellowbox/networks.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/retry.py` & `yellowbox-0.8.5/yellowbox/retry.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/service.py` & `yellowbox-0.8.5/yellowbox/service.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/yellowbox/subclasses.py` & `yellowbox-0.8.5/yellowbox/subclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def _single_endpoint(self) -> Container:
         return self.container
 
 
 SelfRunMixin = TypeVar("SelfRunMixin", bound="RunMixin")
 
 
-class RunMixin(ContainerService, ABC):
+class RunMixin:
     @classmethod
     def service_name(cls):
         return cls.__name__
 
     @classmethod
     @contextmanager
     def run(
@@ -145,33 +145,33 @@
             spinner: whether or not to use a yaspin spinner
             retry_spec: forwarded to cls.start
             network: connect service to network
             **kwargs: all keyword arguments are forwarded to the class's constructor
         """
         yaspin_spinner = _get_spinner(spinner)
         with yaspin_spinner(f"Fetching {cls.service_name()} ..."):
-            service = cls(docker_client, **kwargs)
+            service = cls(docker_client, **kwargs)  # type: ignore[call-arg]
 
         connect_network: ContextManager[None]
         if network:
             connect_network = networks_mod.connect(network, service)
         else:
             connect_network = nullcontext()
 
         with connect_network:
             with yaspin_spinner(f"Waiting for {cls.service_name()} to start..."):
-                service.start(retry_spec=retry_spec)
-            with service:
+                service.start(retry_spec=retry_spec)  # type: ignore[attr-defined]
+            with service:  # type: ignore[attr-defined]
                 yield service
 
 
 SelfARunMixin = TypeVar("SelfARunMixin", bound="AsyncRunMixin")
 
 
-class AsyncRunMixin(ContainerService, ABC):
+class AsyncRunMixin(ABC):
     @classmethod
     def service_name(cls):
         return cls.__name__
 
     @abstractmethod
     async def astart(self, retry_spec: Optional[RetrySpec] = None) -> None:
         """
@@ -179,15 +179,15 @@
         """
 
     async def astop(self, *args, **kwargs) -> None:
         """
         Stop the service synchronously, but block and wait for shutdown asynchronously.
         """
         loop = get_running_loop()
-        func = partial(self.stop, *args, **kwargs)
+        func = partial(self.stop, *args, **kwargs)  # type: ignore[attr-defined]
         await loop.run_in_executor(None, func)
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *args):
         await self.astop()
@@ -212,15 +212,15 @@
             retry_spec: forwarded to cls.start
             network: connect service to network
             **kwargs: all keyword arguments are forwarded to the class's constructor
         """
 
         yaspin_spinner = _get_spinner(verbose)
         with yaspin_spinner(f"Fetching {cls.service_name()} ..."):
-            service = cls(docker_client, **kwargs)
+            service = cls(docker_client, **kwargs)  # type: ignore[call-arg]
 
         connect_network: ContextManager[None]
         if network:
             connect_network = networks_mod.connect(network, service)
         else:
             connect_network = nullcontext()
```

### Comparing `yellowbox-0.8.4/yellowbox/utils.py` & `yellowbox-0.8.5/yellowbox/utils.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.4/PKG-INFO` & `yellowbox-0.8.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowbox
-Version: 0.8.4
+Version: 0.8.5
 Summary: 
 Home-page: https://github.com/biocatchltd/yellowbox
 License: MIT
 Author: biocatch ltd
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

