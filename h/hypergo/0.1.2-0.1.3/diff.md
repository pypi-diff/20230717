# Comparing `tmp/hypergo-0.1.2.tar.gz` & `tmp/hypergo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergo-0.1.2.tar", last modified: Thu Jul 13 18:09:05 2023, max compression
+gzip compressed data, was "hypergo-0.1.3.tar", last modified: Mon Jul 17 14:35:13 2023, max compression
```

## Comparing `hypergo-0.1.2.tar` & `hypergo-0.1.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.169165 hypergo-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.165165 hypergo-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.165165 hypergo-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 18:08:54.000000 hypergo-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-13 18:08:54.000000 hypergo-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 18:08:54.000000 hypergo-0.1.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-13 18:08:54.000000 hypergo-0.1.2/BACKLOG.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:08:54.000000 hypergo-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-13 18:09:05.169165 hypergo-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 18:08:54.000000 hypergo-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.169165 hypergo-0.1.2/hypergo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/azure_service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/azure_service_bus_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-13 18:08:54.000000 hypergo-0.1.2/hypergo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.169165 hypergo-0.1.2/hypergo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-13 18:09:05.000000 hypergo-0.1.2/hypergo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-13 18:09:05.000000 hypergo-0.1.2/hypergo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:09:05.000000 hypergo-0.1.2/hypergo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 18:09:05.000000 hypergo-0.1.2/hypergo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 18:09:05.000000 hypergo-0.1.2/hypergo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-07-13 18:08:54.000000 hypergo-0.1.2/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-13 18:08:54.000000 hypergo-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 18:08:54.000000 hypergo-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 18:09:05.169165 hypergo-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:05.169165 hypergo-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_dynamic_input_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_dynamic_routing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-13 18:08:54.000000 hypergo-0.1.2/tests/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.113808 hypergo-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.105808 hypergo-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.109808 hypergo-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 14:34:59.000000 hypergo-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-17 14:34:59.000000 hypergo-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 14:34:59.000000 hypergo-0.1.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-17 14:34:59.000000 hypergo-0.1.3/BACKLOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:59.000000 hypergo-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-17 14:35:13.113808 hypergo-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 14:34:59.000000 hypergo-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.109808 hypergo-0.1.3/hypergo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/azure_service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/azure_service_bus_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.113808 hypergo-0.1.3/hypergo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-17 14:35:13.000000 hypergo-0.1.3/hypergo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 14:35:13.000000 hypergo-0.1.3/hypergo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:35:13.000000 hypergo-0.1.3/hypergo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 14:35:13.000000 hypergo-0.1.3/hypergo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:35:13.000000 hypergo-0.1.3/hypergo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-07-17 14:34:59.000000 hypergo-0.1.3/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-17 14:34:59.000000 hypergo-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 14:34:59.000000 hypergo-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-17 14:35:13.113808 hypergo-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.113808 hypergo-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_dynamic_input_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_dynamic_routing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_utility.py
```

### Comparing `hypergo-0.1.2/.github/workflows/python-publish.yml` & `hypergo-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/.gitignore` & `hypergo-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/BACKLOG.md` & `hypergo-0.1.3/BACKLOG.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/hypergo/azure_service_bus_connection.py` & `hypergo-0.1.3/hypergo/azure_service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/hypergo/config.py` & `hypergo-0.1.3/hypergo/config.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/hypergo/executor.py` & `hypergo-0.1.3/hypergo/executor.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/hypergo/graph.py` & `hypergo-0.1.3/hypergo/graph.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/hypergo/message.py` & `hypergo-0.1.3/hypergo/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             "body": json.loads(message.get_body().decode("utf-8")),
             "routingkey": message.user_properties["routingkey"],
             "storagekey": cast(str, message.user_properties.get("storagekey")),
         }
 
     @staticmethod
     def from_http_request(request: func.HttpRequest) -> MessageType:
-        return {"body": request.get_json(), "routingkey": "http_request" + urlparse(request.url).path.replace("/", ".")}
+        return {"body": request.get_json(), "routingkey": "http.azurefunction" + urlparse(request.url).path.replace("/", ".")}
 
     @staticmethod
     def to_azure_service_bus_service_bus_message(message: MessageType) -> ServiceBusMessage:
         ret: ServiceBusMessage = ServiceBusMessage(
             body=json.dumps(message["body"]),
             application_properties={
                 "routingkey": message["routingkey"],
```

### Comparing `hypergo-0.1.2/hypergo/service_bus_connection.py` & `hypergo-0.1.3/hypergo/service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/hypergo/storage.py` & `hypergo-0.1.3/hypergo/storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/hypergo/utility.py` & `hypergo-0.1.3/hypergo/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class Utility:
     @staticmethod
     def deep_get(dic: Union[TypedDictType, Dict[str, Any]], key: str) -> Any:
         result = pydash.get(dic, key)
         if not result:
-            raise KeyError("Spec {key} not found in the dictionary")
+            raise KeyError(f"Spec {key}  not found in the dictionary")
         return result
 
     @staticmethod
     def deep_set(dic: Union[TypedDictType, Dict[str, Any]], key: str, val: Any) -> None:
         glom.assign(dic, key, val, missing=dict)
 
     @staticmethod
```

### Comparing `hypergo-0.1.2/hypergo/version.py` & `hypergo-0.1.3/hypergo/version.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/hypergo.egg-info/SOURCES.txt` & `hypergo-0.1.3/hypergo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/lint.sh` & `hypergo-0.1.3/lint.sh`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/tests/test.json` & `hypergo-0.1.3/tests/test.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/tests/test.yaml` & `hypergo-0.1.3/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/tests/test_dynamic_input_bindings.py` & `hypergo-0.1.3/tests/test_dynamic_input_bindings.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/tests/test_dynamic_routing_key.py` & `hypergo-0.1.3/tests/test_dynamic_routing_key.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/tests/test_local_storage.py` & `hypergo-0.1.3/tests/test_local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/tests/test_message.py` & `hypergo-0.1.3/tests/test_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,12 +11,12 @@
                 method='POST',
                 body='{"good": "json"}'.encode('utf-8'),
                 url='https://bgray-test.azurewebsites.net/api/HttpRequestHandler/other_tag?code=-i6NwCuDbR5-rjzNUt7w6hdyjti_5Ccs-yMoaIamIFMmAzFuPk3Xhw==',
                 params=None)
         result = Message.from_http_request(http_request)
 
         self.assertEqual(result['body'],  {'good': 'json'})
-        self.assertEqual(result['routingkey'], 'http_request.api.HttpRequestHandler.other_tag')
+        self.assertEqual(result['routingkey'], 'http.azurefunction.api.HttpRequestHandler.other_tag')
 
 if __name__ == '__main__':
     # Run the unit tests
     unittest.main()
```

### Comparing `hypergo-0.1.2/tests/test_storage.py` & `hypergo-0.1.3/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.2/tests/test_utility.py` & `hypergo-0.1.3/tests/test_utility.py`

 * *Files identical despite different names*

