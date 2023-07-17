# Comparing `tmp/Icotest-DeviceServer-1.0.0.tar.gz` & `tmp/Icotest-DeviceServer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Icotest-DeviceServer-1.0.0.tar", last modified: Fri Sep 30 10:55:59 2022, max compression
+gzip compressed data, was "Icotest-DeviceServer-1.0.3.tar", last modified: Mon Jul 17 09:37:23 2023, max compression
```

## Comparing `Icotest-DeviceServer-1.0.0.tar` & `Icotest-DeviceServer-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,44 @@
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2022-09-30 10:55:59.709598 Icotest-DeviceServer-1.0.0/
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2022-09-30 10:55:59.665597 Icotest-DeviceServer-1.0.0/DeviceServer/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      983 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/__init__.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2022-09-30 10:55:59.673597 Icotest-DeviceServer-1.0.0/DeviceServer/api/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      139 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/api/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    81026 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/api/devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26176 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/api_client.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9709 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/configuration.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3731 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/exceptions.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2022-09-30 10:55:59.705598 Icotest-DeviceServer-1.0.0/DeviceServer/models/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      509 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/models/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8204 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/models/device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3263 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/models/inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4932 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/models/port.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4959 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/models/port_state.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12261 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/DeviceServer/rest.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2022-09-30 10:55:59.705598 Icotest-DeviceServer-1.0.0/Icotest_DeviceServer.egg-info/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5160 2022-09-30 10:55:59.000000 Icotest-DeviceServer-1.0.0/Icotest_DeviceServer.egg-info/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      711 2022-09-30 10:55:59.000000 Icotest-DeviceServer-1.0.0/Icotest_DeviceServer.egg-info/SOURCES.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2022-09-30 10:55:59.000000 Icotest-DeviceServer-1.0.0/Icotest_DeviceServer.egg-info/dependency_links.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2022-09-30 10:55:59.000000 Icotest-DeviceServer-1.0.0/Icotest_DeviceServer.egg-info/requires.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       13 2022-09-30 10:55:59.000000 Icotest-DeviceServer-1.0.0/Icotest_DeviceServer.egg-info/top_level.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2022-09-26 08:19:31.000000 Icotest-DeviceServer-1.0.0/LICENSE
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       35 2022-09-28 14:56:31.000000 Icotest-DeviceServer-1.0.0/MANIFEST.in
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5160 2022-09-30 10:55:59.709598 Icotest-DeviceServer-1.0.0/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3573 2022-09-30 10:54:45.000000 Icotest-DeviceServer-1.0.0/README.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2022-09-30 10:55:59.709598 Icotest-DeviceServer-1.0.0/docs/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      492 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/docs/Device.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    25442 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/docs/DevicesApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      333 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/docs/InlineResponse200.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      419 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/docs/Port.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      435 2022-09-28 13:18:40.000000 Icotest-DeviceServer-1.0.0/docs/PortState.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      825 2022-09-28 15:26:22.000000 Icotest-DeviceServer-1.0.0/pyproject.toml
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2022-09-30 10:55:59.709598 Icotest-DeviceServer-1.0.0/setup.cfg
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-07-17 09:37:23.886866 Icotest-DeviceServer-1.0.3/
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-07-17 09:37:23.882866 Icotest-DeviceServer-1.0.3/DeviceServer/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1350 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/__init__.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-07-17 09:37:23.882866 Icotest-DeviceServer-1.0.3/DeviceServer/api/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      139 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/api/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   188452 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/api/devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    27732 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/api_client.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    16123 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/configuration.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5080 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/exceptions.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-07-17 09:37:23.886866 Icotest-DeviceServer-1.0.3/DeviceServer/models/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      822 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/models/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8278 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/models/db_device_port.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5784 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/models/db_port_state.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12478 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/models/device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     7649 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/models/device_port.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3681 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/models/get_devices_led200_response.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     7051 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/models/host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5045 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/models/port_state.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4245 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/models/temp_range.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3867 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/models/temperature.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12609 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/DeviceServer/rest.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-07-17 09:37:23.886866 Icotest-DeviceServer-1.0.3/Icotest_DeviceServer.egg-info/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     7442 2023-07-17 09:37:23.000000 Icotest-DeviceServer-1.0.3/Icotest_DeviceServer.egg-info/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1017 2023-07-17 09:37:23.000000 Icotest-DeviceServer-1.0.3/Icotest_DeviceServer.egg-info/SOURCES.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-07-17 09:37:23.000000 Icotest-DeviceServer-1.0.3/Icotest_DeviceServer.egg-info/dependency_links.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       68 2023-07-17 09:37:23.000000 Icotest-DeviceServer-1.0.3/Icotest_DeviceServer.egg-info/requires.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       13 2023-07-17 09:37:23.000000 Icotest-DeviceServer-1.0.3/Icotest_DeviceServer.egg-info/top_level.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2023-07-17 09:21:22.000000 Icotest-DeviceServer-1.0.3/LICENSE
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       35 2022-09-28 14:56:31.000000 Icotest-DeviceServer-1.0.3/MANIFEST.in
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     7442 2023-07-17 09:37:23.886866 Icotest-DeviceServer-1.0.3/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5855 2023-07-17 09:35:56.000000 Icotest-DeviceServer-1.0.3/README.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-07-17 09:37:23.886866 Icotest-DeviceServer-1.0.3/docs/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      498 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/docs/DbDevicePort.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      430 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/docs/DbPortState.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      730 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/docs/Device.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      548 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/docs/DevicePort.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    55947 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/docs/DevicesApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      341 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/docs/GetDevicesLed200Response.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      435 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/docs/HostConfig.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      447 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/docs/PortState.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      371 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/docs/TempRange.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      324 2023-07-17 09:03:31.000000 Icotest-DeviceServer-1.0.3/docs/Temperature.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      737 2023-07-17 09:30:28.000000 Icotest-DeviceServer-1.0.3/pyproject.toml
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-07-17 09:37:23.886866 Icotest-DeviceServer-1.0.3/setup.cfg
```

### Comparing `Icotest-DeviceServer-1.0.0/DeviceServer/__init__.py` & `Icotest-DeviceServer-1.0.3/DeviceServer/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,34 +3,40 @@
 # flake8: noqa
 
 """
     DeviceServer
 
     DeviceServer API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.0.3
     Contact: david@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.0"
+__version__ = "1.0.3"
 
 # import apis into sdk package
 from DeviceServer.api.devices_api import DevicesApi
 
 # import ApiClient
 from DeviceServer.api_client import ApiClient
 from DeviceServer.configuration import Configuration
 from DeviceServer.exceptions import OpenApiException
 from DeviceServer.exceptions import ApiTypeError
 from DeviceServer.exceptions import ApiValueError
 from DeviceServer.exceptions import ApiKeyError
+from DeviceServer.exceptions import ApiAttributeError
 from DeviceServer.exceptions import ApiException
 # import models into sdk package
+from DeviceServer.models.db_device_port import DbDevicePort
+from DeviceServer.models.db_port_state import DbPortState
 from DeviceServer.models.device import Device
-from DeviceServer.models.inline_response200 import InlineResponse200
-from DeviceServer.models.port import Port
+from DeviceServer.models.device_port import DevicePort
+from DeviceServer.models.get_devices_led200_response import GetDevicesLed200Response
+from DeviceServer.models.host_config import HostConfig
 from DeviceServer.models.port_state import PortState
+from DeviceServer.models.temp_range import TempRange
+from DeviceServer.models.temperature import Temperature
```

### Comparing `Icotest-DeviceServer-1.0.0/DeviceServer/api_client.py` & `Icotest-DeviceServer-1.0.3/DeviceServer/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     DeviceServer
 
     DeviceServer API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.0.3
     Contact: david@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.3/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -117,17 +117,18 @@
 
     def set_default_header(self, header_name, header_value):
         self.default_headers[header_name] = header_value
 
     def __call_api(
             self, resource_path, method, path_params=None,
             query_params=None, header_params=None, body=None, post_params=None,
-            files=None, response_type=None, auth_settings=None,
+            files=None, response_types_map=None, auth_settings=None,
             _return_http_data_only=None, collection_formats=None,
-            _preload_content=True, _request_timeout=None, _host=None):
+            _preload_content=True, _request_timeout=None, _host=None,
+            _request_auth=None):
 
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
@@ -160,15 +161,17 @@
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(post_params,
                                                     collection_formats)
             post_params.extend(self.files_parameters(files))
 
         # auth setting
-        self.update_params_for_auth(header_params, query_params, auth_settings)
+        self.update_params_for_auth(
+            header_params, query_params, auth_settings,
+            request_auth=_request_auth)
 
         # body
         if body:
             body = self.sanitize_for_serialization(body)
 
         # request url
         if _host is None:
@@ -184,31 +187,33 @@
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout)
         except ApiException as e:
             e.body = e.body.decode('utf-8') if six.PY3 else e.body
             raise e
 
-        content_type = response_data.getheader('content-type')
-
         self.last_response = response_data
 
         return_data = response_data
 
         if not _preload_content:
             return return_data
 
+        response_type = response_types_map.get(response_data.status, None)
+
         if six.PY3 and response_type not in ["file", "bytes"]:
             match = None
+            content_type = response_data.getheader('content-type')
             if content_type is not None:
                 match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
             encoding = match.group(1) if match else "utf-8"
             response_data.data = response_data.data.decode(encoding)
 
         # deserialize response data
+
         if response_type:
             return_data = self.deserialize(response_data, response_type)
         else:
             return_data = None
 
         if _return_http_data_only:
             return (return_data)
@@ -293,16 +298,16 @@
 
         if type(klass) == str:
             if klass.startswith('list['):
                 sub_kls = re.match(r'list\[(.*)\]', klass).group(1)
                 return [self.__deserialize(sub_data, sub_kls)
                         for sub_data in data]
 
-            if klass.startswith('dict('):
-                sub_kls = re.match(r'dict\(([^,]*), (.*)\)', klass).group(2)
+            if klass.startswith('dict['):
+                sub_kls = re.match(r'dict\[([^,]*), (.*)\]', klass).group(2)
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in six.iteritems(data)}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
@@ -318,17 +323,18 @@
             return self.__deserialize_datetime(data)
         else:
             return self.__deserialize_model(data, klass)
 
     def call_api(self, resource_path, method,
                  path_params=None, query_params=None, header_params=None,
                  body=None, post_params=None, files=None,
-                 response_type=None, auth_settings=None, async_req=None,
-                 _return_http_data_only=None, collection_formats=None,
-                 _preload_content=True, _request_timeout=None, _host=None):
+                 response_types_map=None, auth_settings=None,
+                 async_req=None, _return_http_data_only=None,
+                 collection_formats=None,_preload_content=True,
+                  _request_timeout=None, _host=None, _request_auth=None):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async_req request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
@@ -350,41 +356,46 @@
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_token: dict, optional
         :return:
             If async_req parameter is True,
             the request will be called asynchronously.
             The method will return the request thread.
             If parameter async_req is False or missing,
             then the method will return the response directly.
         """
         if not async_req:
             return self.__call_api(resource_path, method,
                                    path_params, query_params, header_params,
                                    body, post_params, files,
-                                   response_type, auth_settings,
+                                   response_types_map, auth_settings,
                                    _return_http_data_only, collection_formats,
-                                   _preload_content, _request_timeout, _host)
+                                   _preload_content, _request_timeout, _host,
+                                   _request_auth)
 
         return self.pool.apply_async(self.__call_api, (resource_path,
                                                        method, path_params,
                                                        query_params,
                                                        header_params, body,
                                                        post_params, files,
-                                                       response_type,
+                                                       response_types_map,
                                                        auth_settings,
                                                        _return_http_data_only,
                                                        collection_formats,
                                                        _preload_content,
                                                        _request_timeout,
-                                                       _host))
+                                                       _host, _request_auth))
 
     def request(self, method, url, query_params=None, headers=None,
                 post_params=None, body=None, _preload_content=True,
                 _request_timeout=None):
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
             return self.rest_client.GET(url,
@@ -507,53 +518,76 @@
         accepts = [x.lower() for x in accepts]
 
         if 'application/json' in accepts:
             return 'application/json'
         else:
             return ', '.join(accepts)
 
-    def select_header_content_type(self, content_types):
+    def select_header_content_type(self, content_types, method=None, body=None):
         """Returns `Content-Type` based on an array of content_types provided.
 
         :param content_types: List of content-types.
+        :param method: http method (e.g. POST, PATCH).
+        :param body: http body to send.
         :return: Content-Type (e.g. application/json).
         """
         if not content_types:
-            return 'application/json'
+            return None
 
         content_types = [x.lower() for x in content_types]
 
+        if (method == 'PATCH' and
+                'application/json-patch+json' in content_types and
+                isinstance(body, list)):
+            return 'application/json-patch+json'
+
         if 'application/json' in content_types or '*/*' in content_types:
             return 'application/json'
         else:
             return content_types[0]
 
-    def update_params_for_auth(self, headers, querys, auth_settings):
+    def update_params_for_auth(self, headers, queries, auth_settings,
+                               request_auth=None):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
-        :param querys: Query parameters tuple list to be updated.
+        :param queries: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
+        :param request_auth: if set, the provided settings will
+                             override the token in the configuration.
         """
         if not auth_settings:
             return
 
+        if request_auth:
+            self._apply_auth_params(headers, queries, request_auth)
+            return
+
         for auth in auth_settings:
             auth_setting = self.configuration.auth_settings().get(auth)
             if auth_setting:
-                if auth_setting['in'] == 'cookie':
-                    headers['Cookie'] = auth_setting['value']
-                elif auth_setting['in'] == 'header':
-                    headers[auth_setting['key']] = auth_setting['value']
-                elif auth_setting['in'] == 'query':
-                    querys.append((auth_setting['key'], auth_setting['value']))
-                else:
-                    raise ApiValueError(
-                        'Authentication token must be in `query` or `header`'
-                    )
+                self._apply_auth_params(headers, queries, auth_setting)
+
+    def _apply_auth_params(self, headers, queries, auth_setting):
+        """Updates the request parameters based on a single auth_setting
+
+        :param headers: Header parameters dict to be updated.
+        :param queries: Query parameters tuple list to be updated.
+        :param auth_setting: auth settings for the endpoint
+        """
+        if auth_setting['in'] == 'cookie':
+            headers['Cookie'] = auth_setting['value']
+        elif auth_setting['in'] == 'header':
+            headers[auth_setting['key']] = auth_setting['value']
+        elif auth_setting['in'] == 'query':
+            queries.append((auth_setting['key'], auth_setting['value']))
+        else:
+            raise ApiValueError(
+                'Authentication token must be in `query` or `header`'
+            )
 
     def __deserialize_file(self, response):
         """Deserializes body to file
 
         Saves response body into a file in a temporary folder,
         using the filename from the `Content-Disposition` header if provided.
 
@@ -654,14 +688,15 @@
                 klass.openapi_types is not None and
                 isinstance(data, (list, dict))):
             for attr, attr_type in six.iteritems(klass.openapi_types):
                 if klass.attribute_map[attr] in data:
                     value = data[klass.attribute_map[attr]]
                     kwargs[attr] = self.__deserialize(value, attr_type)
 
+        kwargs["local_vars_configuration"] = self.configuration
         instance = klass(**kwargs)
 
         if has_discriminator:
             klass_name = instance.get_real_child_model(data)
             if klass_name:
                 instance = self.__deserialize(data, klass_name)
         return instance
```

### Comparing `Icotest-DeviceServer-1.0.0/DeviceServer/exceptions.py` & `Icotest-DeviceServer-1.0.3/DeviceServer/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     DeviceServer
 
     DeviceServer API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.0.3
     Contact: david@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
 
@@ -61,14 +61,33 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiValueError, self).__init__(full_msg)
 
 
+class ApiAttributeError(OpenApiException, AttributeError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Raised when an attribute reference or assignment fails.
+
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (None/list) the path to the exception in the
+                received_data dict
+        """
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiAttributeError, self).__init__(full_msg)
+
+
 class ApiKeyError(OpenApiException, KeyError):
     def __init__(self, msg, path_to_item=None):
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
@@ -106,14 +125,38 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
+class NotFoundException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(NotFoundException, self).__init__(status, reason, http_resp)
+
+
+class UnauthorizedException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+
+
+class ForbiddenException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ForbiddenException, self).__init__(status, reason, http_resp)
+
+
+class ServiceException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ServiceException, self).__init__(status, reason, http_resp)
+
+
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, six.integer_types):
             result += "[{0}]".format(pth)
         else:
```

### Comparing `Icotest-DeviceServer-1.0.0/DeviceServer/models/inline_response200.py` & `Icotest-DeviceServer-1.0.3/DeviceServer/models/get_devices_led200_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # coding: utf-8
 
 """
     DeviceServer
 
     DeviceServer API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.0.3
     Contact: david@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
+try:
+    from inspect import getfullargspec
+except ImportError:
+    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-
 import six
 
 from DeviceServer.configuration import Configuration
 
 
-class InlineResponse200(object):
+class GetDevicesLed200Response(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -38,84 +41,92 @@
     }
 
     attribute_map = {
         'state': 'state'
     }
 
     def __init__(self, state=None, local_vars_configuration=None):  # noqa: E501
-        """InlineResponse200 - a model defined in OpenAPI"""  # noqa: E501
+        """GetDevicesLed200Response - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
+            local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._state = None
         self.discriminator = None
 
         if state is not None:
             self.state = state
 
     @property
     def state(self):
-        """Gets the state of this InlineResponse200.  # noqa: E501
+        """Gets the state of this GetDevicesLed200Response.  # noqa: E501
 
 
-        :return: The state of this InlineResponse200.  # noqa: E501
+        :return: The state of this GetDevicesLed200Response.  # noqa: E501
         :rtype: bool
         """
         return self._state
 
     @state.setter
     def state(self, state):
-        """Sets the state of this InlineResponse200.
+        """Sets the state of this GetDevicesLed200Response.
 
 
-        :param state: The state of this InlineResponse200.  # noqa: E501
-        :type: bool
+        :param state: The state of this GetDevicesLed200Response.  # noqa: E501
+        :type state: bool
         """
 
         self._state = state
 
-    def to_dict(self):
+    def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
+        def convert(x):
+            if hasattr(x, "to_dict"):
+                args = getfullargspec(x.to_dict).args
+                if len(args) == 1:
+                    return x.to_dict()
+                else:
+                    return x.to_dict(serialize)
+            else:
+                return x
+
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
+            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
+                    lambda x: convert(x),
                     value
                 ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
+                    lambda item: (item[0], convert(item[1])),
                     value.items()
                 ))
             else:
-                result[attr] = value
+                result[attr] = convert(value)
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineResponse200):
+        if not isinstance(other, GetDevicesLed200Response):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, InlineResponse200):
+        if not isinstance(other, GetDevicesLed200Response):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `Icotest-DeviceServer-1.0.0/DeviceServer/rest.py` & `Icotest-DeviceServer-1.0.3/DeviceServer/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # coding: utf-8
 
 """
     DeviceServer
 
     DeviceServer API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.0.3
     Contact: david@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import io
 import json
 import logging
 import re
 import ssl
 
-import certifi
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import urlencode
 import urllib3
 
-from DeviceServer.exceptions import ApiException, ApiValueError
+from DeviceServer.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
 
@@ -59,53 +58,49 @@
 
         # cert_reqs
         if configuration.verify_ssl:
             cert_reqs = ssl.CERT_REQUIRED
         else:
             cert_reqs = ssl.CERT_NONE
 
-        # ca_certs
-        if configuration.ssl_ca_cert:
-            ca_certs = configuration.ssl_ca_cert
-        else:
-            # if not set certificate file, use Mozilla's root certificates.
-            ca_certs = certifi.where()
-
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
             addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
+        if configuration.socket_options is not None:
+            addition_pool_args['socket_options'] = configuration.socket_options
+
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
                 maxsize = 4
 
         # https pool manager
         if configuration.proxy:
             self.pool_manager = urllib3.ProxyManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
-                ca_certs=ca_certs,
+                ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 proxy_url=configuration.proxy,
                 proxy_headers=configuration.proxy_headers,
                 **addition_pool_args
             )
         else:
             self.pool_manager = urllib3.PoolManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
-                ca_certs=ca_certs,
+                ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 **addition_pool_args
             )
 
     def request(self, method, url, query_params=None, headers=None,
                 body=None, post_params=None, _preload_content=True,
@@ -138,15 +133,15 @@
             )
 
         post_params = post_params or {}
         headers = headers or {}
 
         timeout = None
         if _request_timeout:
-            if isinstance(_request_timeout, (int, ) if six.PY3 else (int, long)):  # noqa: E501,F821
+            if isinstance(_request_timeout, six.integer_types + (float, )):  # noqa: E501,F821
                 timeout = urllib3.Timeout(total=_request_timeout)
             elif (isinstance(_request_timeout, tuple) and
                   len(_request_timeout) == 2):
                 timeout = urllib3.Timeout(
                     connect=_request_timeout[0], read=_request_timeout[1])
 
         if 'Content-Type' not in headers:
@@ -218,14 +213,26 @@
         if _preload_content:
             r = RESTResponse(r)
 
             # log response body
             logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
+            if r.status == 401:
+                raise UnauthorizedException(http_resp=r)
+
+            if r.status == 403:
+                raise ForbiddenException(http_resp=r)
+
+            if r.status == 404:
+                raise NotFoundException(http_resp=r)
+
+            if 500 <= r.status <= 599:
+                raise ServiceException(http_resp=r)
+
             raise ApiException(http_resp=r)
 
         return r
 
     def GET(self, url, headers=None, query_params=None, _preload_content=True,
             _request_timeout=None):
         return self.request("GET", url,
```

### Comparing `Icotest-DeviceServer-1.0.0/Icotest_DeviceServer.egg-info/PKG-INFO` & `Icotest-DeviceServer-1.0.3/Icotest_DeviceServer.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Icotest-DeviceServer
-Version: 1.0.0
+Version: 1.0.3
 Summary: DeviceServer API
 Author-email: David Atkins <david@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
-License: Copyright © 2022 3ADesign Limited
+License: Copyright © 2023 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
@@ -20,94 +20,113 @@
 License-File: LICENSE
 
 # DeviceServer
 DeviceServer API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0
-- Package version: 1.0.0
-- Build package: org.openapitools.codegen.languages.PythonClientCodegen
+- API version: 1.0.3
+- Package version: 1.0.3
+- Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 
 ## Requirements.
 
-Python 2.7 and 3.4+
+Python 3.4+
 
 ## Installation & Usage
 ### pip install
 
-```bash
+```sh
 pip install Icotest-DeviceServer
 ```
 
 Then import the package:
 ```python
 import DeviceServer
 ```
 
 ## Getting Started
 
-Please follow the [installation procedure](#installation--usage) and then run the following:
+Please follow the installation procedure and then run the following:
 
 ```python
-from __future__ import print_function
-
 import time
 import DeviceServer
 from DeviceServer.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to http://localhost/DeviceServer
 # See configuration.py for a list of all supported configuration parameters.
 configuration = DeviceServer.Configuration(
     host = "http://localhost/DeviceServer"
 )
 
-
-
 # Enter a context with an instance of the API client
 with DeviceServer.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = DeviceServer.DevicesApi(api_client)
-    
+    device_id = "dedfeda9-1bf0-44c2-ac94-69370afb0c3f"  # str: UUID of device
+
     try:
-        # GET list of devices
-        api_response = api_instance.get_devices()
+        # GET all ports for device
+        api_response = api_instance.get_device_device_id_ports(device_id)
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling DevicesApi->get_devices: %s\n" % e)
-    
+        print(
+            "Exception when calling DevicesApi->get_device_device_id_ports: "
+            "%s\n" % e
+        )
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost/DeviceServer*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*DevicesApi* | [**get_device_device_id_ports**](docs/DevicesApi.md#get_device_device_id_ports) | **GET** /Devices/{device_id}/Ports | GET all ports for device
+*DevicesApi* | [**get_device_id_port_index**](docs/DevicesApi.md#get_device_id_port_index) | **GET** /Devices/{device_id}/Ports/{port_index} | GET status of port
 *DevicesApi* | [**get_devices**](docs/DevicesApi.md#get_devices) | **GET** /Devices | GET list of devices
-*DevicesApi* | [**get_devices_button**](docs/DevicesApi.md#get_devices_button) | **GET** /Devices/Button/{device_id} | GET state of button
-*DevicesApi* | [**get_devices_device_id_ports**](docs/DevicesApi.md#get_devices_device_id_ports) | **GET** /Devices/{device_id}/Ports | GET all ports for device
+*DevicesApi* | [**get_devices_button**](docs/DevicesApi.md#get_devices_button) | **GET** /Devices/{device_id}/Button | GET state of button
 *DevicesApi* | [**get_devices_index**](docs/DevicesApi.md#get_devices_index) | **GET** /Devices/{device_id} | GET single device
-*DevicesApi* | [**get_devices_leds**](docs/DevicesApi.md#get_devices_leds) | **GET** /Devices/{device_id}/Leds/{led_index} | GET state of LED
-*DevicesApi* | [**get_devices_port**](docs/DevicesApi.md#get_devices_port) | **GET** /Devices/{device_id}/Ports/{port_index} | GET status of port
-*DevicesApi* | [**get_port**](docs/DevicesApi.md#get_port) | **GET** /Ports/{port_index} | GET status of port
-*DevicesApi* | [**put_devices_leds_index**](docs/DevicesApi.md#put_devices_leds_index) | **PUT** /Devices/{device_id}/Leds/{led_index} | PUT state of LED
+*DevicesApi* | [**get_devices_led**](docs/DevicesApi.md#get_devices_led) | **GET** /Devices/{device_id}/Leds/{led_index} | GET state of LED
+*DevicesApi* | [**get_devices_temperature**](docs/DevicesApi.md#get_devices_temperature) | **GET** /Devices/{device_id}/Temperature | Your GET endpoint
+*DevicesApi* | [**get_host_config**](docs/DevicesApi.md#get_host_config) | **GET** /Host/Config | Your GET endpoint
+*DevicesApi* | [**get_port**](docs/DevicesApi.md#get_port) | **GET** /Port/{port_id} | GET status of port by id
+*DevicesApi* | [**get_port_states**](docs/DevicesApi.md#get_port_states) | **GET** /PortStates/{port_id} | Your GET endpoint
+*DevicesApi* | [**get_ports**](docs/DevicesApi.md#get_ports) | **GET** /Ports | GET status of all ports
+*DevicesApi* | [**get_relay_state**](docs/DevicesApi.md#get_relay_state) | **GET** /Devices/{device_id}/Relay | Your GET endpoint
+*DevicesApi* | [**get_temperature_range**](docs/DevicesApi.md#get_temperature_range) | **GET** /Devices/{device_id}/Temperature/Range | Your GET endpoint
+*DevicesApi* | [**get_temperature_thresholds**](docs/DevicesApi.md#get_temperature_thresholds) | **GET** /Devices/{device_id}/Temperature/Thresholds | Your GET endpoint
+*DevicesApi* | [**put_device_device_id_description**](docs/DevicesApi.md#put_device_device_id_description) | **PUT** /Device/{device_id}/Description | 
+*DevicesApi* | [**put_device_device_id_name**](docs/DevicesApi.md#put_device_device_id_name) | **PUT** /Device/{device_id}/Name | 
+*DevicesApi* | [**put_device_id_label**](docs/DevicesApi.md#put_device_id_label) | **PUT** /Device/{device_id}/Port/{port_index}/Label | 
+*DevicesApi* | [**put_devices_led_index**](docs/DevicesApi.md#put_devices_led_index) | **PUT** /Devices/{device_id}/Leds/{led_index} | PUT state of LED
 *DevicesApi* | [**put_devices_ports**](docs/DevicesApi.md#put_devices_ports) | **PUT** /Devices/{device_id}/Ports/{port_index} | PUT state of port
 *DevicesApi* | [**put_devices_ports_pulse**](docs/DevicesApi.md#put_devices_ports_pulse) | **PUT** /Devices/{device_id}/Ports/{port_index}/Pulse | PUT port into state for period of time
-*DevicesApi* | [**put_ports**](docs/DevicesApi.md#put_ports) | **PUT** /Ports/{port_index} | PUT state of port
+*DevicesApi* | [**put_host_config**](docs/DevicesApi.md#put_host_config) | **PUT** /Host/Config | 
+*DevicesApi* | [**put_port_port_id_label**](docs/DevicesApi.md#put_port_port_id_label) | **PUT** /Port/{port_id}/Label | 
+*DevicesApi* | [**put_port_states_port_id**](docs/DevicesApi.md#put_port_states_port_id) | **PUT** /PortStates/{port_id} | 
 *DevicesApi* | [**put_ports_pulse**](docs/DevicesApi.md#put_ports_pulse) | **PUT** /Ports/{port_index}/Pulse | PUT port into state for period of time
+*DevicesApi* | [**put_relay_state**](docs/DevicesApi.md#put_relay_state) | **PUT** /Devices/{device_id}/Relay | 
+*DevicesApi* | [**put_socket_refresh**](docs/DevicesApi.md#put_socket_refresh) | **PUT** /Devices/{device_id}/Socket/Refresh | 
+*DevicesApi* | [**put_state_by_port_id**](docs/DevicesApi.md#put_state_by_port_id) | **PUT** /Port/{port_id} | PUT state of port
 
 
 ## Documentation For Models
 
+ - [DbDevicePort](docs/DbDevicePort.md)
+ - [DbPortState](docs/DbPortState.md)
  - [Device](docs/Device.md)
- - [InlineResponse200](docs/InlineResponse200.md)
- - [Port](docs/Port.md)
+ - [DevicePort](docs/DevicePort.md)
+ - [GetDevicesLed200Response](docs/GetDevicesLed200Response.md)
+ - [HostConfig](docs/HostConfig.md)
  - [PortState](docs/PortState.md)
+ - [TempRange](docs/TempRange.md)
+ - [Temperature](docs/Temperature.md)
 
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization.
 
 ## Author
```

### Comparing `Icotest-DeviceServer-1.0.0/Icotest_DeviceServer.egg-info/SOURCES.txt` & `Icotest-DeviceServer-1.0.3/Icotest_DeviceServer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,21 +6,31 @@
 DeviceServer/api_client.py
 DeviceServer/configuration.py
 DeviceServer/exceptions.py
 DeviceServer/rest.py
 DeviceServer/api/__init__.py
 DeviceServer/api/devices_api.py
 DeviceServer/models/__init__.py
+DeviceServer/models/db_device_port.py
+DeviceServer/models/db_port_state.py
 DeviceServer/models/device.py
-DeviceServer/models/inline_response200.py
-DeviceServer/models/port.py
+DeviceServer/models/device_port.py
+DeviceServer/models/get_devices_led200_response.py
+DeviceServer/models/host_config.py
 DeviceServer/models/port_state.py
+DeviceServer/models/temp_range.py
+DeviceServer/models/temperature.py
 Icotest_DeviceServer.egg-info/PKG-INFO
 Icotest_DeviceServer.egg-info/SOURCES.txt
 Icotest_DeviceServer.egg-info/dependency_links.txt
 Icotest_DeviceServer.egg-info/requires.txt
 Icotest_DeviceServer.egg-info/top_level.txt
+docs/DbDevicePort.md
+docs/DbPortState.md
 docs/Device.md
+docs/DevicePort.md
 docs/DevicesApi.md
-docs/InlineResponse200.md
-docs/Port.md
-docs/PortState.md
+docs/GetDevicesLed200Response.md
+docs/HostConfig.md
+docs/PortState.md
+docs/TempRange.md
+docs/Temperature.md
```

### Comparing `Icotest-DeviceServer-1.0.0/LICENSE` & `Icotest-DeviceServer-1.0.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2022 3ADesign Limited
+Copyright © 2023 3ADesign Limited
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `Icotest-DeviceServer-1.0.0/PKG-INFO` & `Icotest-DeviceServer-1.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Icotest-DeviceServer
-Version: 1.0.0
+Version: 1.0.3
 Summary: DeviceServer API
 Author-email: David Atkins <david@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
-License: Copyright © 2022 3ADesign Limited
+License: Copyright © 2023 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
@@ -20,94 +20,113 @@
 License-File: LICENSE
 
 # DeviceServer
 DeviceServer API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0
-- Package version: 1.0.0
-- Build package: org.openapitools.codegen.languages.PythonClientCodegen
+- API version: 1.0.3
+- Package version: 1.0.3
+- Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 
 ## Requirements.
 
-Python 2.7 and 3.4+
+Python 3.4+
 
 ## Installation & Usage
 ### pip install
 
-```bash
+```sh
 pip install Icotest-DeviceServer
 ```
 
 Then import the package:
 ```python
 import DeviceServer
 ```
 
 ## Getting Started
 
-Please follow the [installation procedure](#installation--usage) and then run the following:
+Please follow the installation procedure and then run the following:
 
 ```python
-from __future__ import print_function
-
 import time
 import DeviceServer
 from DeviceServer.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to http://localhost/DeviceServer
 # See configuration.py for a list of all supported configuration parameters.
 configuration = DeviceServer.Configuration(
     host = "http://localhost/DeviceServer"
 )
 
-
-
 # Enter a context with an instance of the API client
 with DeviceServer.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = DeviceServer.DevicesApi(api_client)
-    
+    device_id = "dedfeda9-1bf0-44c2-ac94-69370afb0c3f"  # str: UUID of device
+
     try:
-        # GET list of devices
-        api_response = api_instance.get_devices()
+        # GET all ports for device
+        api_response = api_instance.get_device_device_id_ports(device_id)
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling DevicesApi->get_devices: %s\n" % e)
-    
+        print(
+            "Exception when calling DevicesApi->get_device_device_id_ports: "
+            "%s\n" % e
+        )
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost/DeviceServer*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*DevicesApi* | [**get_device_device_id_ports**](docs/DevicesApi.md#get_device_device_id_ports) | **GET** /Devices/{device_id}/Ports | GET all ports for device
+*DevicesApi* | [**get_device_id_port_index**](docs/DevicesApi.md#get_device_id_port_index) | **GET** /Devices/{device_id}/Ports/{port_index} | GET status of port
 *DevicesApi* | [**get_devices**](docs/DevicesApi.md#get_devices) | **GET** /Devices | GET list of devices
-*DevicesApi* | [**get_devices_button**](docs/DevicesApi.md#get_devices_button) | **GET** /Devices/Button/{device_id} | GET state of button
-*DevicesApi* | [**get_devices_device_id_ports**](docs/DevicesApi.md#get_devices_device_id_ports) | **GET** /Devices/{device_id}/Ports | GET all ports for device
+*DevicesApi* | [**get_devices_button**](docs/DevicesApi.md#get_devices_button) | **GET** /Devices/{device_id}/Button | GET state of button
 *DevicesApi* | [**get_devices_index**](docs/DevicesApi.md#get_devices_index) | **GET** /Devices/{device_id} | GET single device
-*DevicesApi* | [**get_devices_leds**](docs/DevicesApi.md#get_devices_leds) | **GET** /Devices/{device_id}/Leds/{led_index} | GET state of LED
-*DevicesApi* | [**get_devices_port**](docs/DevicesApi.md#get_devices_port) | **GET** /Devices/{device_id}/Ports/{port_index} | GET status of port
-*DevicesApi* | [**get_port**](docs/DevicesApi.md#get_port) | **GET** /Ports/{port_index} | GET status of port
-*DevicesApi* | [**put_devices_leds_index**](docs/DevicesApi.md#put_devices_leds_index) | **PUT** /Devices/{device_id}/Leds/{led_index} | PUT state of LED
+*DevicesApi* | [**get_devices_led**](docs/DevicesApi.md#get_devices_led) | **GET** /Devices/{device_id}/Leds/{led_index} | GET state of LED
+*DevicesApi* | [**get_devices_temperature**](docs/DevicesApi.md#get_devices_temperature) | **GET** /Devices/{device_id}/Temperature | Your GET endpoint
+*DevicesApi* | [**get_host_config**](docs/DevicesApi.md#get_host_config) | **GET** /Host/Config | Your GET endpoint
+*DevicesApi* | [**get_port**](docs/DevicesApi.md#get_port) | **GET** /Port/{port_id} | GET status of port by id
+*DevicesApi* | [**get_port_states**](docs/DevicesApi.md#get_port_states) | **GET** /PortStates/{port_id} | Your GET endpoint
+*DevicesApi* | [**get_ports**](docs/DevicesApi.md#get_ports) | **GET** /Ports | GET status of all ports
+*DevicesApi* | [**get_relay_state**](docs/DevicesApi.md#get_relay_state) | **GET** /Devices/{device_id}/Relay | Your GET endpoint
+*DevicesApi* | [**get_temperature_range**](docs/DevicesApi.md#get_temperature_range) | **GET** /Devices/{device_id}/Temperature/Range | Your GET endpoint
+*DevicesApi* | [**get_temperature_thresholds**](docs/DevicesApi.md#get_temperature_thresholds) | **GET** /Devices/{device_id}/Temperature/Thresholds | Your GET endpoint
+*DevicesApi* | [**put_device_device_id_description**](docs/DevicesApi.md#put_device_device_id_description) | **PUT** /Device/{device_id}/Description | 
+*DevicesApi* | [**put_device_device_id_name**](docs/DevicesApi.md#put_device_device_id_name) | **PUT** /Device/{device_id}/Name | 
+*DevicesApi* | [**put_device_id_label**](docs/DevicesApi.md#put_device_id_label) | **PUT** /Device/{device_id}/Port/{port_index}/Label | 
+*DevicesApi* | [**put_devices_led_index**](docs/DevicesApi.md#put_devices_led_index) | **PUT** /Devices/{device_id}/Leds/{led_index} | PUT state of LED
 *DevicesApi* | [**put_devices_ports**](docs/DevicesApi.md#put_devices_ports) | **PUT** /Devices/{device_id}/Ports/{port_index} | PUT state of port
 *DevicesApi* | [**put_devices_ports_pulse**](docs/DevicesApi.md#put_devices_ports_pulse) | **PUT** /Devices/{device_id}/Ports/{port_index}/Pulse | PUT port into state for period of time
-*DevicesApi* | [**put_ports**](docs/DevicesApi.md#put_ports) | **PUT** /Ports/{port_index} | PUT state of port
+*DevicesApi* | [**put_host_config**](docs/DevicesApi.md#put_host_config) | **PUT** /Host/Config | 
+*DevicesApi* | [**put_port_port_id_label**](docs/DevicesApi.md#put_port_port_id_label) | **PUT** /Port/{port_id}/Label | 
+*DevicesApi* | [**put_port_states_port_id**](docs/DevicesApi.md#put_port_states_port_id) | **PUT** /PortStates/{port_id} | 
 *DevicesApi* | [**put_ports_pulse**](docs/DevicesApi.md#put_ports_pulse) | **PUT** /Ports/{port_index}/Pulse | PUT port into state for period of time
+*DevicesApi* | [**put_relay_state**](docs/DevicesApi.md#put_relay_state) | **PUT** /Devices/{device_id}/Relay | 
+*DevicesApi* | [**put_socket_refresh**](docs/DevicesApi.md#put_socket_refresh) | **PUT** /Devices/{device_id}/Socket/Refresh | 
+*DevicesApi* | [**put_state_by_port_id**](docs/DevicesApi.md#put_state_by_port_id) | **PUT** /Port/{port_id} | PUT state of port
 
 
 ## Documentation For Models
 
+ - [DbDevicePort](docs/DbDevicePort.md)
+ - [DbPortState](docs/DbPortState.md)
  - [Device](docs/Device.md)
- - [InlineResponse200](docs/InlineResponse200.md)
- - [Port](docs/Port.md)
+ - [DevicePort](docs/DevicePort.md)
+ - [GetDevicesLed200Response](docs/GetDevicesLed200Response.md)
+ - [HostConfig](docs/HostConfig.md)
  - [PortState](docs/PortState.md)
+ - [TempRange](docs/TempRange.md)
+ - [Temperature](docs/Temperature.md)
 
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization.
 
 ## Author
```

