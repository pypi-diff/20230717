# Comparing `tmp/rotarypi-1.0.1.tar.gz` & `tmp/rotarypi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotarypi-1.0.1.tar", last modified: Thu Feb 16 19:41:30 2023, max compression
+gzip compressed data, was "rotarypi-2.0.0.tar", last modified: Mon Jul 17 14:10:36 2023, max compression
```

## Comparing `rotarypi-1.0.1.tar` & `rotarypi-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2023-02-16 19:41:30.838323 rotarypi-1.0.1/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)        0 2022-12-29 18:54:25.000000 rotarypi-1.0.1/MANIFEST.in
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1116 2023-02-16 19:41:30.838323 rotarypi-1.0.1/PKG-INFO
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      562 2023-02-16 19:18:08.000000 rotarypi-1.0.1/README.md
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2023-02-16 19:41:30.838323 rotarypi-1.0.1/rotarypi/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      109 2023-02-15 19:13:46.000000 rotarypi-1.0.1/rotarypi/__init__.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      289 2023-02-16 18:44:26.000000 rotarypi-1.0.1/rotarypi/dialconfig.py
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     2610 2023-02-16 18:40:23.000000 rotarypi-1.0.1/rotarypi/rotaryreader.py
-drwxrwxr-x   0 dinu      (1000) dinu      (1000)        0 2023-02-16 19:41:30.838323 rotarypi-1.0.1/rotarypi.egg-info/
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1116 2023-02-16 19:41:30.000000 rotarypi-1.0.1/rotarypi.egg-info/PKG-INFO
--rw-rw-r--   0 dinu      (1000) dinu      (1000)      258 2023-02-16 19:41:30.000000 rotarypi-1.0.1/rotarypi.egg-info/SOURCES.txt
--rw-rw-r--   0 dinu      (1000) dinu      (1000)        1 2023-02-16 19:41:30.000000 rotarypi-1.0.1/rotarypi.egg-info/dependency_links.txt
--rw-rw-r--   0 dinu      (1000) dinu      (1000)       29 2023-02-16 19:41:30.000000 rotarypi-1.0.1/rotarypi.egg-info/requires.txt
--rw-rw-r--   0 dinu      (1000) dinu      (1000)        9 2023-02-16 19:41:30.000000 rotarypi-1.0.1/rotarypi.egg-info/top_level.txt
--rw-rw-r--   0 dinu      (1000) dinu      (1000)       38 2023-02-16 19:41:30.838323 rotarypi-1.0.1/setup.cfg
--rw-rw-r--   0 dinu      (1000) dinu      (1000)     1038 2023-02-16 19:29:28.000000 rotarypi-1.0.1/setup.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-07-17 14:10:36.585812 rotarypi-2.0.0/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-07-17 12:49:36.000000 rotarypi-2.0.0/MANIFEST.in
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1096 2023-07-17 14:10:36.585812 rotarypi-2.0.0/PKG-INFO
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      562 2023-07-17 12:49:36.000000 rotarypi-2.0.0/README.md
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-07-17 14:10:36.584812 rotarypi-2.0.0/rotarypi/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      174 2023-07-17 13:35:20.000000 rotarypi-2.0.0/rotarypi/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      348 2023-07-17 13:49:34.000000 rotarypi-2.0.0/rotarypi/dialconfig.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      307 2023-07-17 14:06:10.000000 rotarypi-2.0.0/rotarypi/dialdata.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3735 2023-07-17 13:52:12.000000 rotarypi-2.0.0/rotarypi/rotaryreader.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-07-17 14:10:36.585812 rotarypi-2.0.0/rotarypi.egg-info/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1096 2023-07-17 14:10:36.000000 rotarypi-2.0.0/rotarypi.egg-info/PKG-INFO
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      279 2023-07-17 14:10:36.000000 rotarypi-2.0.0/rotarypi.egg-info/SOURCES.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        1 2023-07-17 14:10:36.000000 rotarypi-2.0.0/rotarypi.egg-info/dependency_links.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       29 2023-07-17 14:10:36.000000 rotarypi-2.0.0/rotarypi.egg-info/requires.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        9 2023-07-17 14:10:36.000000 rotarypi-2.0.0/rotarypi.egg-info/top_level.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       38 2023-07-17 14:10:36.585812 rotarypi-2.0.0/setup.cfg
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1038 2023-07-17 13:13:03.000000 rotarypi-2.0.0/setup.py
```

### Comparing `rotarypi-1.0.1/PKG-INFO` & `rotarypi-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: rotarypi
-Version: 1.0.1
+Version: 2.0.0
 Summary: Reading the rotary dial of an old phone with a RaspberryPi
 Home-page: https://gitlab.com/rotaryphone/rotarypi
 Author: Martin Obrist
 Author-email: martin.obrist@buero.io
 License: MIT
 Project-URL: Documentation, https://rotarypi.readthedocs.io
 Project-URL: Source Code, https://gitlab.com/rotaryphone/rotarypi
 Project-URL: Issue Tracker, https://gitlab.com/rotaryphone/rotarypi/-/issues
-Platform: UNKNOWN
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # RotaryPi
 
 Python library to read the rotary dial of an old telephone with a Raspberry Pi.
@@ -21,9 +20,7 @@
 Targets Python `>3.9` on a Raspberry Pi.
 
 This library was developed using a **Tfg 3-39.205** desktop telephone from 1974, but it should work with a wide variety of rotary dials since the basic principle is pretty strait forward and probably very similar on various models. But I only have this particular model, so I've only tested it on that particular one.
 
 ## Documentation
 
 Read the full documentation on [readthedocs](https://rotarypi.readthedocs.io/en/latest/).
-
-
```

### Comparing `rotarypi-1.0.1/README.md` & `rotarypi-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `rotarypi-1.0.1/rotarypi/rotaryreader.py` & `rotarypi-2.0.0/rotarypi/rotaryreader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from queue import Queue
 import RPi.GPIO as GPIO
 from typing import Optional
 import logging
 import sys
+import time
 
-from rotarypi import DialPinout, DialConfiguration
+from rotarypi import DialPinout, DialConfiguration, EventType, HandsetState, DialEvent
 
 
 class RotaryReader:
 
-    def __init__(self, queue: Queue[int], pinout: Optional[DialPinout] = None, config: Optional[DialConfiguration] = None):
-        self.queue: Queue[int] = queue
+    def __init__(self, queue: Queue[DialEvent], pinout: Optional[DialPinout] = None, config: Optional[DialConfiguration] = None):
+        self.queue: Queue[DialEvent] = queue
         self.pinout = pinout if pinout is not None else DialPinout()
         self.config = config if config is not None else DialConfiguration()
         self.logger = self._setup_logging()
         self.gpio = GPIO
         self.gpio.setmode(GPIO.BCM)
         self.rotating = False
         self.counter = 0
@@ -28,47 +29,76 @@
         logger.addHandler(handler)
         logger.setLevel(self.config.loglevel)
         return logger
 
     def _setup(self):
         self.gpio.setup(self.pinout.dial_pin, GPIO.IN, pull_up_down=GPIO.PUD_UP)
         self.gpio.setup(self.pinout.counter_pin, GPIO.IN, pull_up_down=GPIO.PUD_UP)
+        self.gpio.setup(self.pinout.handset_pin, GPIO.IN, pull_up_down=GPIO.PUD_UP)
 
     def _dialpin_callback(self, channel):
         self.logger.debug("Dial pin callback")
         state = self.gpio.input(channel)
         if state:
             self.rotating = False
             self.logger.debug("Rotation finished")
             if self.counter > 0:
                 val = self.counter % 10
-                self.queue.put(val)
+                msg = DialEvent(
+                    type=EventType.DIAL_EVENT,
+                    data=val
+                )
+                self.queue.put(msg)
                 self.logger.info(f"queued {val}")
             self.counter = 0
         else:
             self.rotating = True
             self.logger.debug("Rotation started")
 
     def _count_dial_callback(self, channel):
         self.logger.debug("Count pin callback")
         self.counter += 1
 
+    def _handset_callback(self, channel):
+        self.logger.debug("Handset callback")
+        time.sleep(0.01)
+        state = self.gpio.input(channel)
+        if state:
+            msg = DialEvent(
+                type=EventType.HANDSET_EVENT,
+                data=HandsetState.HUNG_UP
+            )
+            self.logger.info("Handset was hung up")
+        else:
+            msg = DialEvent(
+                type=EventType.HANDSET_EVENT,
+                data=HandsetState.PICKED_UP
+            )
+            self.logger.info("Handset was picked up")
+        self.queue.put(msg)
+
     def start(self):
         self.gpio.add_event_detect(
-            self.pinout.dial_pin, GPIO.BOTH,
+            self.pinout.dial_pin, self.gpio.BOTH,
             callback=self._dialpin_callback,
             bouncetime=self.config.dial_debounce
         )
         self.gpio.add_event_detect(
-            self.pinout.counter_pin, GPIO.RISING,
+            self.pinout.counter_pin, self.gpio.RISING,
             callback=self._count_dial_callback,
             bouncetime=self.config.counter_debounce
         )
+        self.gpio.add_event_detect(
+            self.pinout.handset_pin, self.gpio.BOTH,
+            callback=self._handset_callback,
+            bouncetime=self.config.handset_debounce
+        )
         self.logger.info("Callbacks attached, started listening")
 
     def stop(self):
         self.gpio.remove_event_detect(self.pinout.dial_pin)
         self.gpio.remove_event_detect(self.pinout.counter_pin)
+        self.gpio.remove_event_detect(self.pinout.handset_pin)
         self.logger.info("Callbacks detached, stopped listening")
 
     def cleanup(self):
         self.gpio.cleanup()
```

### Comparing `rotarypi-1.0.1/rotarypi.egg-info/PKG-INFO` & `rotarypi-2.0.0/rotarypi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: rotarypi
-Version: 1.0.1
+Version: 2.0.0
 Summary: Reading the rotary dial of an old phone with a RaspberryPi
 Home-page: https://gitlab.com/rotaryphone/rotarypi
 Author: Martin Obrist
 Author-email: martin.obrist@buero.io
 License: MIT
 Project-URL: Documentation, https://rotarypi.readthedocs.io
 Project-URL: Source Code, https://gitlab.com/rotaryphone/rotarypi
 Project-URL: Issue Tracker, https://gitlab.com/rotaryphone/rotarypi/-/issues
-Platform: UNKNOWN
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # RotaryPi
 
 Python library to read the rotary dial of an old telephone with a Raspberry Pi.
@@ -21,9 +20,7 @@
 Targets Python `>3.9` on a Raspberry Pi.
 
 This library was developed using a **Tfg 3-39.205** desktop telephone from 1974, but it should work with a wide variety of rotary dials since the basic principle is pretty strait forward and probably very similar on various models. But I only have this particular model, so I've only tested it on that particular one.
 
 ## Documentation
 
 Read the full documentation on [readthedocs](https://rotarypi.readthedocs.io/en/latest/).
-
-
```

### Comparing `rotarypi-1.0.1/setup.py` & `rotarypi-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 
 setup(
     name='rotarypi',
-    version='1.0.1',
+    version='2.0.0',
     description="Reading the rotary dial of an old phone with a RaspberryPi",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
     author='Martin Obrist',
     author_email='martin.obrist@buero.io',
     url='https://gitlab.com/rotaryphone/rotarypi',
```

