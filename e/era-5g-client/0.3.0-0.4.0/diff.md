# Comparing `tmp/era_5g_client-0.3.0.tar.gz` & `tmp/era_5g_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_client-0.3.0.tar", last modified: Thu Jul  6 12:58:31 2023, max compression
+gzip compressed data, was "era_5g_client-0.4.0.tar", last modified: Mon Jul 17 13:05:24 2023, max compression
```

## Comparing `era_5g_client-0.3.0.tar` & `era_5g_client-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 12:58:31.643878 era_5g_client-0.3.0/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      420 2023-07-06 12:58:31.643878 era_5g_client-0.3.0/PKG-INFO
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      749 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/backend_shim.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 12:58:31.639879 era_5g_client-0.3.0/era_5g_client/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    11907 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/client.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6599 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/client_base.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1759 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/data_sender_gstreamer.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2813 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/data_sender_gstreamer_from_file.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2904 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/data_sender_gstreamer_from_source.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      986 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/dataclasses.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      662 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/exceptions.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2635 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/middleware_resource_checker.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/py.typed
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 12:58:31.643878 era_5g_client-0.3.0/era_5g_client.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      420 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      609 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      127 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       14 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/top_level.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-06 12:58:31.643878 era_5g_client-0.3.0/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1015 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/setup.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 13:05:24.169156 era_5g_client-0.4.0/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       12 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/MANIFEST.in
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      420 2023-07-17 13:05:24.169156 era_5g_client-0.4.0/PKG-INFO
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      749 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/backend_shim.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 13:05:24.169156 era_5g_client-0.4.0/era_5g_client/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/__init__.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)    11799 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/client.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     8530 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/client_base.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      523 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/dataclasses.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      662 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/exceptions.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     2715 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/middleware_resource_checker.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/py.typed
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 13:05:24.169156 era_5g_client-0.4.0/era_5g_client.egg-info/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      420 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/PKG-INFO
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      470 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      127 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/requires.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       14 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/top_level.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       38 2023-07-17 13:05:24.169156 era_5g_client-0.4.0/setup.cfg
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1015 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/setup.py
```

### Comparing `era_5g_client-0.3.0/backend_shim.py` & `era_5g_client-0.4.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.3.0/era_5g_client/client.py` & `era_5g_client-0.4.0/era_5g_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import logging
 import os
 from collections.abc import Callable
 from enum import Enum
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, Optional
 
-import numpy as np
 import requests
 from requests import HTTPError
 
 from era_5g_client.client_base import NetAppClientBase
-from era_5g_client.dataclasses import MiddlewareInfo, NetAppLocation
+from era_5g_client.dataclasses import MiddlewareInfo
 from era_5g_client.exceptions import FailedToConnect, NetAppNotReady
 from era_5g_client.middleware_resource_checker import MiddlewareResourceChecker
 
-buffer: List[Tuple[np.ndarray, Optional[str]]] = []
-
 # port of the netapp's server
 NETAPP_PORT = int(os.getenv("NETAPP_PORT", 5896))
 
 
 class RunTaskMode(Enum):
     # deploy the task but don't wait until it is ready, do not register with it
     DO_NOTHING = 1
@@ -38,14 +35,16 @@
     def __init__(
         self,
         results_event: Callable,
         image_error_event: Optional[Callable] = None,
         json_error_event: Optional[Callable] = None,
         control_cmd_event: Optional[Callable] = None,
         control_cmd_error_event: Optional[Callable] = None,
+        logging_level: int = logging.INFO,
+        socketio_debug: bool = False,
     ) -> None:
         """Constructor.
 
         Args:
             results_event (Callable): Callback where results will arrive.
             image_error_event (Callable, optional): Callback which is emitted when server
                 failed to process the incoming image.
@@ -60,15 +59,23 @@
         Raises:
             FailedToConnect: When connection to the middleware could not be set or
                 login failed
             FailedToObtainPlan: When the plan was not successfully returned from
                 the middleware
         """
 
-        super().__init__(results_event, image_error_event, json_error_event, control_cmd_event, control_cmd_error_event)
+        super().__init__(
+            results_event,
+            image_error_event,
+            json_error_event,
+            control_cmd_event,
+            control_cmd_error_event,
+            logging_level,
+            socketio_debug,
+        )
 
         self.host: Optional[str] = None
         self.action_plan_id: Optional[str] = None
         self.resource_checker: Optional[MiddlewareResourceChecker] = None
         self.middleware_info: Optional[MiddlewareInfo] = None
         self.token: Optional[str] = None
 
@@ -85,15 +92,15 @@
         """
         self.middleware_info = middleware_info
         self.middleware_info.address = self.middleware_info.address.rstrip("/")
         try:
             # connect to the middleware
             self.token = self.gateway_login(self.middleware_info.user_id, self.middleware_info.password)
         except FailedToConnect as ex:
-            logging.error(f"Can't connect to middleware: {ex}")
+            self.logger.error(f"Can't connect to middleware: {ex}")
             raise
 
     def run_task(
         self,
         task_id: str,
         robot_id: str,
         resource_lock: bool,
@@ -105,89 +112,83 @@
 
         Args:
             task_id (str): The GUID of the task which should be deployed.
             robot_id (str): The GUID of the robot that deploys the NetApp.
             resource_lock (bool): TBA
             mode (Optional[RunTaskMode]): Specify the mode in which the run_task
                 works
-            gstreamer (Optional[bool], optional):  Indicates if a GStreamer pipeline
-                should be initialized for image transport. Applied only if register
-                is True. Defaults to False.
-            ws_data (Optional[bool], optional): Indicates if a separate websocket channel
-                for data transport should be set. Applied only if register
-                is True. Defaults to False.
             args (Optional[Dict], optional): NetApp-specific arguments. Applied only if register
                 is True. Defaults to None.
 
         Raises:
             FailedToConnect: Raised when running the task failed.
         """
         assert self.middleware_info
         try:
             self.action_plan_id = self.gateway_get_plan(
                 task_id, resource_lock, robot_id
             )  # Get the plan_id by sending the token and task_id
-
             if not self.action_plan_id:
                 raise FailedToConnect("Failed to obtain action plan id...")
 
             self.resource_checker = MiddlewareResourceChecker(
                 str(self.token),
                 self.action_plan_id,
                 self.middleware_info.build_api_endpoint("orchestrate/orchestrate/plan"),
                 daemon=True,
             )
 
             self.resource_checker.start()
             if mode in [RunTaskMode.WAIT, RunTaskMode.WAIT_AND_REGISTER]:
                 self.wait_until_netapp_ready()
                 self.load_netapp_address()
-                if not self.netapp_location:
-                    raise FailedToConnect("Failed to obtain NetApp URI or port")
+                if not self.netapp_address:
+                    raise FailedToConnect("Failed to obtain network application address")
                 if mode == RunTaskMode.WAIT_AND_REGISTER:
-                    self.register(self.netapp_location, args)
+                    self.register(self.netapp_address, args, wait_until_available=True)
         except (FailedToConnect, NetAppNotReady) as ex:
             self.delete_all_resources()
-            logging.error(f"Failed to run task: {ex}")
+            self.logger.error(f"Failed to run task: {ex}")
             raise
 
     def register(
         self,
-        netapp_location: NetAppLocation,
+        netapp_address: str,
         args: Optional[Dict] = None,
+        wait_until_available: bool = False,
+        wait_timeout: int = -1,
     ) -> None:
         """Calls the /register endpoint of the NetApp interface and if the
         registration is successful, it sets up the WebSocket connection for
         results retrieval.
 
         Args:
-            netapp_location (NetAppLocation): The URI and port of the NetApp interface.
-            gstreamer (Optional[bool], optional):  Indicates if a GStreamer pipeline
-                should be initialized for image transport. Defaults to False.
-            ws_data (Optional[bool], optional): Indicates if a separate websocket channel
-                for data transport should be set. Defaults to False.
-            use_control_cmds (Optional[bool], optional): Indicates if a websocket channel
-                for control commands should be used. Control commands are indended for
-                changing the internal state of a stateful NetApp. Defaults to False.
+            netapp_address (str): The URL of the network application interface,
+                including the scheme and optionally port and path to the interface,
+                e.g. http://localhost:80 or http://gateway/path_to_interface
             args (Optional[Dict], optional): NetApp-specific arguments. Defaults to None.
+            wait_until_available: If True, the client will repeatedly try to register
+                with the Network Application until it is available. Defaults to False.
+            wait_timeout: How long the client will try to connect to network application.
+                Only used if wait_until_available is True. If negative, the client
+                will waits indefinitely. Defaults to -1.
 
         Raises:
             NetAppNotReady: Raised when register called before the NetApp is ready.
 
         Returns:
             Response: The response from the NetApp.
         """
-
         if not self.resource_checker:
             raise NetAppNotReady("Not connected to the middleware.")
 
         if not self.resource_checker.is_ready():
             raise NetAppNotReady("Not ready.")
 
-        super().register(netapp_location, args)
+        super().register(netapp_address, args, wait_until_available, wait_timeout)
 
     def disconnect(self) -> None:
         """Calls the /unregister endpoint of the server and disconnects the
         WebSocket connection."""
         super().disconnect()
         if self.resource_checker is not None:
             self.resource_checker.stop()
@@ -202,19 +203,20 @@
         if not self.resource_checker:
             raise FailedToConnect("Not connected to middleware.")
         self.resource_checker.wait_until_resource_ready()
 
     def load_netapp_address(self) -> None:
         if not (self.resource_checker and self.resource_checker.is_ready()):
             raise NetAppNotReady
-        self.netapp_location = NetAppLocation(str(self.resource_checker.url), NETAPP_PORT)
+        # TODO: check somehow that the url is correct?
+        self.netapp_address = str(self.resource_checker.url)
 
     def gateway_login(self, user_id: str, password: str) -> str:
         assert self.middleware_info
-        print("Trying to log into the middleware")
+        self.logger.debug("Trying to log into the middleware")
         # Request Login
         try:
             r = requests.post(
                 self.middleware_info.build_api_endpoint("Login"), json={"Id": user_id, "Password": password}
             )
             response = r.json()
             if "errors" in response:
@@ -231,15 +233,15 @@
             raise FailedToConnect(f"Could not login to the middleware gateway, the response does not contain {e}")
 
     def gateway_get_plan(self, taskid: str, resource_lock: bool, robot_id: str) -> str:
         assert self.middleware_info
         # Request plan
 
         try:
-            print("Goal task is: " + str(taskid))
+            self.logger.debug("Goal task is: " + str(taskid))
             hed = {"Authorization": f"Bearer {str(self.token)}"}
             data = {
                 "TaskId": str(taskid),
                 "LockResourceReUse": resource_lock,
                 "RobotId": robot_id,
             }
             response = requests.post(
@@ -249,15 +251,15 @@
                 raise FailedToConnect("Invalid response.")
 
             if "statusCode" in response and (response["statusCode"] == 500 or response["statusCode"] == 400):
                 raise FailedToConnect(f"response {response['statusCode']}: {response['message']}")
             # todo:             if "errors" in response:
             #                 raise FailedToConnect(str(response["errors"]))
             action_plan_id = str(response["ActionPlanId"])
-            print("ActionPlanId ** is: " + str(action_plan_id))
+            self.logger.debug("ActionPlanId ** is: " + str(action_plan_id))
             return action_plan_id
         except KeyError as e:
             raise FailedToConnect(f"Could not get the plan: {e}")
 
     def delete_all_resources(self) -> None:
         if self.token is None or self.action_plan_id is None:
             return
@@ -267,20 +269,20 @@
             if self.middleware_info:
                 url = self.middleware_info.build_api_endpoint(
                     f"orchestrate/orchestrate/plan/{str(self.action_plan_id)}"
                 )
                 response = requests.delete(url, headers=hed)
 
                 if response.ok:
-                    print("Resource deleted")
+                    self.logger.debug("Resource deleted")
 
         except HTTPError as e:
-            print(e.response.status_code)
+            self.logger.debug(e.response.status_code)
             raise FailedToConnect("Error, could not get delete the resource, revisit the log files for more details.")
 
     def delete_single_resource(self) -> None:
         raise NotImplementedError  # TODO
 
     def gateway_log_off(self) -> None:
-        print("Middleware log out successful")
+        self.logger.debug("Middleware log out successful")
         # TODO
         pass
```

### Comparing `era_5g_client-0.3.0/era_5g_client/client_base.py` & `era_5g_client-0.4.0/era_5g_client/client_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import base64
 import logging
-import os
+import time
 from collections.abc import Callable
 from dataclasses import asdict
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, Optional, Union
 
 import cv2
 import numpy as np
 import socketio
 from socketio.exceptions import ConnectionError
 
-from era_5g_client.dataclasses import NetAppLocation
 from era_5g_client.exceptions import FailedToConnect
 from era_5g_interface.dataclasses.control_command import ControlCmdType, ControlCommand
+from era_5g_interface.h264_encoder import H264Encoder, H264EncoderError
 
-# port of the netapp's server
-NETAPP_PORT = int(os.getenv("NETAPP_PORT", 5896))
+logging.basicConfig()
 
 
 class NetAppClientBase:
     """Basic implementation of the NetApp client.
 
     It creates the Requests object with session and bind callbacks for
     connection info and results from the NetApp.
@@ -28,14 +27,16 @@
     def __init__(
         self,
         results_event: Callable,
         image_error_event: Optional[Callable] = None,
         json_error_event: Optional[Callable] = None,
         control_cmd_event: Optional[Callable] = None,
         control_cmd_error_event: Optional[Callable] = None,
+        logging_level: int = logging.INFO,
+        socketio_debug: bool = False,
     ) -> None:
         """Constructor.
 
         Args:
 
             results_event (Callable): Callback where results will arrive.
             image_error_event (Callable, optional): Callback which is emited when server
@@ -50,68 +51,85 @@
 
         Raises:
             FailedToConnect: When connection to the middleware could not be set or
                 login failed
             FailedToObtainPlan: When the plan was not successfully returned from
                 the middleware
         """
-
-        self._sio = socketio.Client()
-        self.netapp_location: Union[NetAppLocation, None] = None
+        self._sio = socketio.Client(logger=socketio_debug)
+        self.netapp_address: Union[str, None] = None
         self._sio.on("message", results_event, namespace="/results")
         self._sio.on("connect", self.on_connect_event, namespace="/results")
         self._sio.on("image_error", image_error_event, namespace="/data")
         self._sio.on("json_error", json_error_event, namespace="/data")
         self._sio.on("connect_error", self.on_connect_error, namespace="/results")
         self._sio.on("control_cmd_result", control_cmd_event, namespace="/control")
         self._sio.on("control_cmd_error", control_cmd_error_event, namespace="/control")
         self._session_cookie: Optional[str] = None
-        # holds the gstreamer port
-        self.gstreamer_port: Optional[int] = None
-        self._buffer: List[Tuple[np.ndarray, Optional[str]]] = []
+        self.h264_encoder: Optional[H264Encoder] = None
         self._image_error_event = image_error_event
         self._json_error_event = json_error_event
         self._control_cmd_event = control_cmd_event
         self._control_cmd_error_event = control_cmd_error_event
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(logging_level)
 
     def register(
         self,
-        netapp_location: NetAppLocation,
+        netapp_address: str,
         args: Optional[Dict] = None,
+        wait_until_available: bool = False,
+        wait_timeout: int = -1,
     ) -> None:
         """Calls the /register endpoint of the NetApp interface and if the
         registration is successful, it sets up the WebSocket connection for
         results retrieval.
 
         Args:
-            netapp_location (NetAppLocation): The URI and port of the NetApp interface.
-            gstreamer (Optional[bool], optional): Indicates if a GStreamer pipeline
-                should be initialized for image transport. Defaults to False.
+            netapp_address (str): The URL of the network application interface,
+                including the scheme and optionally port and path to the interface,
+                e.g. http://localhost:80 or http://gateway/path_to_interface
             args (Optional[Dict], optional): Optional parameters to be passed to
             the NetApp, in the form of dict. Defaults to None.
+            wait_until_available: If True, the client will repeatedly try to register
+                with the Network Application until it is available. Defaults to False.
+            wait_timeout: How long the client will try to connect to network application.
+                Only used if wait_until_available is True. If negative, the client
+                will waits indefinitely. Defaults to -1.
 
         Raises:
             FailedToConnect: _description_
 
         Returns:
             Response: response from the NetApp.
         """
 
-        self.netapp_location = netapp_location
-
+        self.netapp_address = netapp_address
         namespaces_to_connect = ["/data", "/control", "/results"]
-        try:
-            self._sio.connect(
-                self.netapp_location.build_api_endpoint(""),
-                namespaces=namespaces_to_connect,
-                wait_timeout=10,
-            )
-        except ConnectionError as ex:
-            raise FailedToConnect(ex)
-        logging.info(f"Client connected to namespaces: {namespaces_to_connect}")
+        start_time = time.time()
+        while True:
+            try:
+                self.logger.debug("Trying to connect to the network application")
+                self._sio.connect(
+                    netapp_address,
+                    namespaces=namespaces_to_connect,
+                    wait_timeout=10,
+                )
+                break
+            except ConnectionError as ex:
+                self.logger.debug(f"Failed to connect: {ex}")
+                if not wait_until_available or (wait_timeout > 0 and start_time + wait_timeout < time.time()):
+                    raise FailedToConnect(ex)
+                self.logger.warn("Failed to connect to network application. Retrying in 1 second.")
+                time.sleep(1)
+
+        self.logger.info(f"Client connected to namespaces: {namespaces_to_connect}")
+
+        if args and args.get("h264") is True:
+            self.h264_encoder = H264Encoder(float(args["fps"]), int(args["width"]), int(args["height"]))
 
         if args is None:  # TODO would be probably better to handle in ControlCommand
             args = {}
 
         # initialize the network application with desired parameters using the set_state command
         control_cmd = ControlCommand(ControlCmdType.SET_STATE, clear_queue=True, data=args)
         self.send_control_command(control_cmd)
@@ -122,46 +140,68 @@
 
     def wait(self) -> None:
         """Blocking infinite waiting."""
         self._sio.wait()
 
     def on_connect_event(self) -> None:
         """The callback called once the connection to the NetApp is made."""
-        print("Connected to server")
+        self.logger.info("Connected to server")
 
-    def on_connect_error(self, data: str) -> None:
+    def on_connect_error(self, message=None) -> None:
         """The callback called on connection error."""
-        print(f"Connection error: {data}")
-        # self.disconnect()
+        self.logger.error(f"Connection error: {message}")
+        self.disconnect()
 
-    def send_image_ws(self, frame: np.ndarray, timestamp: Optional[str] = None, metadata: Optional[str] = None):
-        """Encodes the image frame to the jpg format and sends it over the
-        websocket, to the /data namespace.
+    def send_image_ws(self, frame: np.ndarray, timestamp: Optional[int] = None, metadata: Optional[str] = None):
+        """Encodes the image frame to the jpg or h264 format and sends it over
+        the websocket, to the /data namespace.
 
         Args:
             frame (np.ndarray): Image frame
-            timestamp (Optional[str], optional): Frame timestamp The timestamp format
-            is defined by the NetApp. Defaults to None.
+            timestamp (Optional[int], optional): Frame timestamp
+            metadata (Optional[str], optional): Optional metadata
+        """
+
+        try:
+            if self.h264_encoder:
+                frame_encoded = self.h264_encoder.encode_ndarray(frame)
+            else:
+                _, frame_jpeg = cv2.imencode(".jpg", frame)
+                # TODO: check why type: ignore is needed for next line
+                frame_encoded = base64.b64encode(frame_jpeg)  # type: ignore
+            data = {"timestamp": timestamp, "frame": frame_encoded}
+            if metadata:
+                data["metadata"] = metadata
+            self._sio.emit("image", data, "/data")
+        except H264EncoderError as e:
+            self.logger.error(f"H264 encoder error: {e}")
+            self.disconnect()
+            raise e
+        except Exception as e:
+            self.logger.error(f"Send image emit error: {e}")
+            self.disconnect()
+            raise e
+
+    def send_image_ws_raw(self, data: Dict):
+        """Sends already encoded image data to /data namespace.
+
+        Args:
+            data (Dict): _description_
         """
-        _, img_encoded = cv2.imencode(".jpg", frame)
-        f = base64.b64encode(img_encoded)
-        data = {"timestamp": timestamp, "frame": f}
-        if metadata:
-            data["metadata"] = metadata
         self._sio.emit("image", data, "/data")
 
     def send_json_ws(self, json: Dict) -> None:
         """Sends netapp-specific json data using the websockets.
 
         Args:
             json (dict): Json data in the form of Python dictionary
         """
-        self._sio.call("json", json, "/data")
+        self._sio.emit("json", json, "/data")
 
     def send_control_command(self, control_command):
         """Sends control command over the websocket.
 
         Args:
             control_command (ControlCommand): Control command to be sent.
         """
 
-        self._sio.emit("command", asdict(control_command), "/control")
+        self._sio.call("command", asdict(control_command), "/control")
```

### Comparing `era_5g_client-0.3.0/era_5g_client/exceptions.py` & `era_5g_client-0.4.0/era_5g_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.3.0/era_5g_client/middleware_resource_checker.py` & `era_5g_client-0.4.0/era_5g_client/middleware_resource_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import time
 from threading import Event, Thread
 from typing import Callable, Dict, Optional
 
 import requests
 from requests import HTTPError
 
@@ -25,23 +26,23 @@
     def stop(self) -> None:
         self.stop_event.set()
 
     def run(self) -> None:
         while not self.stop_event.is_set():
             resource_state = self.get_resource_status()
 
-            seq = resource_state.get("ActionSequence", [])
+            seq = resource_state.get("actionSequence", [])
             if seq:
                 services = seq[0].get("Services", [])
                 if services:
                     self.resource_state = services[0]
                     assert isinstance(self.resource_state, dict)
-                    self.status = self.resource_state.get("ServiceStatus", None)
-                    self.url = self.resource_state.get("ServiceUrl", None)
-
+                    self.status = self.resource_state.get("serviceStatus", None)
+                    self.url = self.resource_state.get("serviceUrl", None)
+                    logging.debug(f"{self.status=}, {self.url=}")
             if self.state_callback:
                 self.state_callback(self.resource_state)
             time.sleep(0.5)  # TODO: adjust or use something similar to rospy.rate.sleep()
 
     def get_resource_status(self) -> Dict:
         try:  # query orchestrator for latest information regarding the status of resources.
             hed = {"Authorization": "Bearer " + str(self.token)}
```

### Comparing `era_5g_client-0.3.0/setup.py` & `era_5g_client-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,19 @@
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
     ],
     'description': 'A client for 5G-ERA NetApps',
     'install_requires': (
-        'era-5g-interface~=0.3.0',
-        'numpy~=1.24.4',
-        'opencv-python~=4.6.0.66',
-        'python-socketio~=5.8.0',
-        'requests~=2.31.0',
+        'era-5g-interface~=0.4.0',
+        'numpy>=1.24.2',
+        'opencv-python>=4.6.0.66',
+        'python-socketio>=5.8.0',
+        'requests>=2.28.2',
         'types-requests==2.31.0.1',
     ),
     'license': 'LGPL',
     'name': 'era_5g_client',
     'namespace_packages': (
     ),
     'package_data': {
@@ -31,9 +31,9 @@
             'py.typed',
         ),
     },
     'packages': (
         'era_5g_client',
     ),
     'python_requires': '>=3.8,<3.11',
-    'version': '0.3.0',
+    'version': '0.4.0',
 })
```

