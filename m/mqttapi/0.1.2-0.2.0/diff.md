# Comparing `tmp/mqttapi-0.1.2.tar.gz` & `tmp/mqttapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqttapi-0.1.2.tar", last modified: Sat Jul 15 04:27:39 2023, max compression
+gzip compressed data, was "mqttapi-0.2.0.tar", last modified: Mon Jul 17 01:12:01 2023, max compression
```

## Comparing `mqttapi-0.1.2.tar` & `mqttapi-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 04:27:39.822895 mqttapi-0.1.2/
--rw-r--r--   0 davi      (1000) davi      (1000)     1066 2023-07-15 04:13:08.000000 mqttapi-0.1.2/LICENSE
--rw-r--r--   0 davi      (1000) davi      (1000)      629 2023-07-15 04:27:39.821895 mqttapi-0.1.2/PKG-INFO
-drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 04:27:39.813359 mqttapi-0.1.2/mqttapi/
--rw-r--r--   0 davi      (1000) davi      (1000)      183 2023-07-15 04:20:29.000000 mqttapi-0.1.2/mqttapi/__init__.py
--rw-r--r--   0 davi      (1000) davi      (1000)       22 2023-07-15 04:26:59.000000 mqttapi-0.1.2/mqttapi/__version__.py
--rw-r--r--   0 davi      (1000) davi      (1000)     1050 2023-07-15 04:13:08.000000 mqttapi-0.1.2/mqttapi/bd_manipulator.py
--rw-r--r--   0 davi      (1000) davi      (1000)      559 2023-07-15 04:13:08.000000 mqttapi-0.1.2/mqttapi/json_manipulator.py
--rw-r--r--   0 davi      (1000) davi      (1000)     1597 2023-07-15 04:13:08.000000 mqttapi-0.1.2/mqttapi/main.py
--rw-r--r--   0 davi      (1000) davi      (1000)     1472 2023-07-15 04:13:08.000000 mqttapi-0.1.2/mqttapi/mqtt_communicator.py
--rw-r--r--   0 davi      (1000) davi      (1000)     2275 2023-07-15 04:23:34.000000 mqttapi-0.1.2/mqttapi/websocket_server.py
-drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 04:27:39.821895 mqttapi-0.1.2/mqttapi.egg-info/
--rw-r--r--   0 davi      (1000) davi      (1000)      629 2023-07-15 04:27:39.000000 mqttapi-0.1.2/mqttapi.egg-info/PKG-INFO
--rw-r--r--   0 davi      (1000) davi      (1000)      340 2023-07-15 04:27:39.000000 mqttapi-0.1.2/mqttapi.egg-info/SOURCES.txt
--rw-r--r--   0 davi      (1000) davi      (1000)        1 2023-07-15 04:27:39.000000 mqttapi-0.1.2/mqttapi.egg-info/dependency_links.txt
--rw-r--r--   0 davi      (1000) davi      (1000)       47 2023-07-15 04:27:39.000000 mqttapi-0.1.2/mqttapi.egg-info/requires.txt
--rw-r--r--   0 davi      (1000) davi      (1000)        8 2023-07-15 04:27:39.000000 mqttapi-0.1.2/mqttapi.egg-info/top_level.txt
--rw-r--r--   0 davi      (1000) davi      (1000)       38 2023-07-15 04:27:39.822895 mqttapi-0.1.2/setup.cfg
--rw-r--r--   0 davi      (1000) davi      (1000)     1182 2023-07-15 04:23:13.000000 mqttapi-0.1.2/setup.py
+drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-17 01:12:01.457057 mqttapi-0.2.0/
+-rw-r--r--   0 davi      (1000) davi      (1000)     1066 2023-07-15 04:13:08.000000 mqttapi-0.2.0/LICENSE
+-rw-r--r--   0 davi      (1000) davi      (1000)      629 2023-07-17 01:12:01.456047 mqttapi-0.2.0/PKG-INFO
+drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-17 01:12:01.435724 mqttapi-0.2.0/mqttapi/
+-rw-r--r--   0 davi      (1000) davi      (1000)      228 2023-07-15 15:36:52.000000 mqttapi-0.2.0/mqttapi/__init__.py
+-rw-r--r--   0 davi      (1000) davi      (1000)       22 2023-07-17 01:08:31.000000 mqttapi-0.2.0/mqttapi/__version__.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1050 2023-07-15 04:13:08.000000 mqttapi-0.2.0/mqttapi/bd_manipulator.py
+-rw-r--r--   0 davi      (1000) davi      (1000)      559 2023-07-15 04:13:08.000000 mqttapi-0.2.0/mqttapi/json_manipulator.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1597 2023-07-15 04:13:08.000000 mqttapi-0.2.0/mqttapi/main.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1632 2023-07-16 23:04:38.000000 mqttapi-0.2.0/mqttapi/mqtt_communicator.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1488 2023-07-16 22:56:46.000000 mqttapi-0.2.0/mqttapi/websocket_client.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1351 2023-07-15 16:16:24.000000 mqttapi-0.2.0/mqttapi/websocket_server.py
+drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-17 01:12:01.454540 mqttapi-0.2.0/mqttapi.egg-info/
+-rw-r--r--   0 davi      (1000) davi      (1000)      629 2023-07-17 01:12:00.000000 mqttapi-0.2.0/mqttapi.egg-info/PKG-INFO
+-rw-r--r--   0 davi      (1000) davi      (1000)      368 2023-07-17 01:12:00.000000 mqttapi-0.2.0/mqttapi.egg-info/SOURCES.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)        1 2023-07-17 01:12:00.000000 mqttapi-0.2.0/mqttapi.egg-info/dependency_links.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)       47 2023-07-17 01:12:00.000000 mqttapi-0.2.0/mqttapi.egg-info/requires.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)        8 2023-07-17 01:12:00.000000 mqttapi-0.2.0/mqttapi.egg-info/top_level.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)       38 2023-07-17 01:12:01.457057 mqttapi-0.2.0/setup.cfg
+-rw-r--r--   0 davi      (1000) davi      (1000)     1182 2023-07-15 07:37:18.000000 mqttapi-0.2.0/setup.py
```

### Comparing `mqttapi-0.1.2/LICENSE` & `mqttapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.2/PKG-INFO` & `mqttapi-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttapi
-Version: 0.1.2
+Version: 0.2.0
 Summary: simplified mqtt library
 Home-page: https://github.com/davifurao/mqttapi
 Author: Davi Luna
 Author-email: Sdavi738@gmail.com
 Keywords: mqtt api,mosquitto api,real-time,messaging,simplified mqtt,paho-mqtt api
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mqttapi-0.1.2/mqttapi/bd_manipulator.py` & `mqttapi-0.2.0/mqttapi/bd_manipulator.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.2/mqttapi/json_manipulator.py` & `mqttapi-0.2.0/mqttapi/json_manipulator.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.2/mqttapi/main.py` & `mqttapi-0.2.0/mqttapi/main.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.2/mqttapi/mqtt_communicator.py` & `mqttapi-0.2.0/mqttapi/mqtt_communicator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import paho.mqtt.client as mqtt
 import datetime
 
 class MQTTCommunicator:
     def __init__(self, host, port, keepalive, bind_address):
         self.host = host
         self.port = port
@@ -10,15 +11,16 @@
         self.client = mqtt.Client("python3")
         self.connected = False
 
     def connect(self):
         self.client.on_connect = self.on_connect
         self.client.on_message = self.on_message
         self.client.connect(self.host, self.port, self.keepalive, self.bind_address)
-        self.client.loop_start()
+        
+        
 
     def disconnect(self):
         self.client.disconnect()
         self.client.loop_stop()
         self.connected = False
 
     def on_connect(self, client, userdata, flags, rc):
@@ -35,7 +37,13 @@
 
     def on_message(self, client, userdata, msg):
         print("=============================")
         print("Topic: " + str(msg.topic))
         print("Payload: " + str(msg.payload))
         print("Hora: " + datetime.datetime.now(datetime.timezone.utc).strftime("%H:%M:%S"))
         print("=============================")
+
+    async def run(self):
+        while self.connected:
+            # Processar eventos MQTT
+            self.client.loop()
+            await asyncio.sleep(0.1)
```

### Comparing `mqttapi-0.1.2/mqttapi/websocket_server.py` & `mqttapi-0.2.0/mqttapi/websocket_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 import asyncio
-import json
-import threading
 import websockets
-import websocket
-
-
 
 class WebSocketServer:
     def __init__(self, host, port):
         self.host = host
         self.port = port
         self.connected_clients = set()
         self.server = None
@@ -37,35 +32,8 @@
         # Executar o servidor em um loop de eventos
         asyncio.get_event_loop().run_until_complete(self.server)
         asyncio.get_event_loop().run_forever()
 
     def stop_server(self):
         if self.server:
             self.server.close()
-            
-    def send_message_to_websocket(topic, payload):
-        if websocket and websocket.sock and websocket.sock.connected:
-            message = {
-                'topic': topic,
-                'payload': payload
-            }
-            websocket.send(json.dumps(message))
-            
-    def connect_to_websocket(self):
-        global websocket
-        websocket_server = f"ws://{self.host}:{self.port}/"
-        websocket = websocket.WebSocketApp(websocket_server, on_message=self.on_message)
-        websocket.run_forever()
-        
-    def on_message(ws, message):
-        data = json.loads(message)
-        topic = data['topic']
-        payload = data['payload']
-
-    def start_websocket_thread(self):
-        websocket_thread = threading.Thread(target=self.connect_to_websocket)
-        websocket_thread.daemon = True
-        websocket_thread.start()
-
-
-
-            
+
```

### Comparing `mqttapi-0.1.2/mqttapi.egg-info/PKG-INFO` & `mqttapi-0.2.0/mqttapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttapi
-Version: 0.1.2
+Version: 0.2.0
 Summary: simplified mqtt library
 Home-page: https://github.com/davifurao/mqttapi
 Author: Davi Luna
 Author-email: Sdavi738@gmail.com
 Keywords: mqtt api,mosquitto api,real-time,messaging,simplified mqtt,paho-mqtt api
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mqttapi-0.1.2/setup.py` & `mqttapi-0.2.0/setup.py`

 * *Files identical despite different names*

