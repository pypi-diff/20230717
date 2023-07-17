# Comparing `tmp/era_5g_interface-0.3.0.tar.gz` & `tmp/era_5g_interface-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_interface-0.3.0.tar", last modified: Thu Jul  6 09:18:53 2023, max compression
+gzip compressed data, was "era_5g_interface-0.4.0.tar", last modified: Mon Jul 17 12:18:02 2023, max compression
```

## Comparing `era_5g_interface-0.3.0.tar` & `era_5g_interface-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.998852 era_5g_interface-0.3.0/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      427 2023-07-06 09:18:52.994852 era_5g_interface-0.3.0/PKG-INFO
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      749 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/backend_shim.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.994852 era_5g_interface-0.3.0/era_5g_interface/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/__init__.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.994852 era_5g_interface-0.3.0/era_5g_interface/dataclasses/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/dataclasses/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1285 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/dataclasses/control_command.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/py.typed
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1730 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/task_handler.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2837 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/task_handler_gstreamer.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      968 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/task_handler_gstreamer_internal_q.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2158 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/task_handler_internal_q.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.994852 era_5g_interface-0.3.0/era_5g_interface/utils/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/utils/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5875 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/utils/rate_timer.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.994852 era_5g_interface-0.3.0/era_5g_interface.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      427 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      674 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       17 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/top_level.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-06 09:18:52.998852 era_5g_interface-0.3.0/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      972 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/setup.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       12 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/MANIFEST.in
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      427 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/PKG-INFO
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      749 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/backend_shim.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/era_5g_interface/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/__init__.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/era_5g_interface/dataclasses/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/dataclasses/__init__.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1285 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/dataclasses/control_command.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1468 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/h264_decoder.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1699 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/h264_encoder.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     4178 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/interface_helpers.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/py.typed
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1470 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/task_handler.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     2483 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/task_handler_internal_q.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/era_5g_interface/utils/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/utils/__init__.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     5899 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/utils/rate_timer.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/era_5g_interface.egg-info/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      427 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/PKG-INFO
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      681 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/namespace_packages.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       67 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/requires.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       17 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/top_level.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       38 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/setup.cfg
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1023 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/setup.py
```

### Comparing `era_5g_interface-0.3.0/backend_shim.py` & `era_5g_interface-0.4.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.3.0/era_5g_interface/dataclasses/control_command.py` & `era_5g_interface-0.4.0/era_5g_interface/dataclasses/control_command.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.3.0/era_5g_interface/task_handler.py` & `era_5g_interface-0.4.0/era_5g_interface/task_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 from abc import ABC, abstractmethod
-from threading import Event, Thread
 from typing import Optional
 
 import numpy as np
 
 from era_5g_interface.dataclasses.control_command import ControlCommand
 
 
 class TaskHandlerInitializationFailed(Exception):
     pass
 
 
-class TaskHandler(Thread, ABC):
+class TaskHandler(ABC):
     """Abstract class.
 
-    Thread-based task handler which takes care of receiving data from
-    the NetApp client and passing them to the NetApp worker.
+    Task handler which takes care of receiving data from the NetApp
+    client and passing them to the NetApp worker.
     """
 
-    def __init__(self, sid: str, **kw) -> None:
-        super().__init__(**kw)
-        self.stop_event = Event()
+    def __init__(self, sid: str, decoder=None) -> None:
         self.sid = sid
         self.websocket_id: Optional[str] = None
-
-    def stop(self):
-        self.stop_event.set()
-
-    @abstractmethod
-    def run(self) -> None:
-        """This method is run once the thread is started and could be used for
-        periodical retrieval of images."""
-
-        pass
+        self.frame_id = 0
+        self.decoder = decoder
+        self.last_timestamp = 0
 
     @abstractmethod
     def store_image(self, metadata: dict, image: np.ndarray) -> None:
         """This method is intended to pass the image to the worker (using
         internal queues, message broker or anything else).
 
         Args:
```

### Comparing `era_5g_interface-0.3.0/era_5g_interface/task_handler_internal_q.py` & `era_5g_interface-0.4.0/era_5g_interface/task_handler_internal_q.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 from queue import Empty, Full, Queue
 
 import numpy as np
 
 from era_5g_interface.dataclasses.control_command import ControlCommand
 from era_5g_interface.task_handler import TaskHandler
 
+logger: logging.Logger = logging.getLogger(__name__)
+
 
 class TaskHandlerInternalQ(TaskHandler):
     """Task handler which takes care of passing the data to the python internal
     queue for future processing.
 
     It could either be inherited to implement the _run method and read
     the data from any source or used directly and call the store_image
@@ -22,50 +25,53 @@
             sid (str): The session id obtained from NetApp client. It is used to
                 match the results with the data sender.
             image_queue (Queue): The queue where the image and metadata should
                 be passed to.
         """
 
         super().__init__(sid=sid, **kw)
-        self._q = image_queue
-        self.index = 0
+        self._q: Queue = image_queue
+
+    def image_queue_size(self) -> int:
+        return self._q.qsize()
+
+    def image_queue_occupancy(self) -> float:
+        return self._q.qsize() / self._q.maxsize
 
     def store_image(self, metadata: dict, image: np.ndarray) -> None:
         """Method which will store the image to the queue for processing.
 
         Args:
             metadata (dict): Arbitrary dictionary with metadata related to the image.
                 The format is NetApp-specific.
             image (_type_): The image to be processed.
         """
-
+        self.frame_id += 1
+        # logger.info(f"TaskHandlerInternalQ received frame id: {self.frame_id} with timestamp: {metadata['timestamp']}")
         try:
             self._q.put((metadata, image), block=False)
         except Full:
             pass
             # TODO: raise an exception
 
     def store_control_data(self, data: ControlCommand) -> None:
         """Pass control commands to the worker using internal queue.
 
         Args:
             data (ControlCommand): ControlCommand with control data.
         """
 
         try:
-            self._q.put((data), block=False)
+            self._q.put(data, block=False)
         except Full:
             pass
             # TODO: raise an exception
 
     def clear_storage(self) -> None:
         """Clear all items from internal queue."""
 
         while not self._q.empty():
             try:
                 self._q.get(block=False)
             except Empty:
                 break
             self._q.task_done()
-
-    def run(self) -> None:
-        pass
```

### Comparing `era_5g_interface-0.3.0/era_5g_interface/utils/rate_timer.py` & `era_5g_interface-0.4.0/era_5g_interface/utils/rate_timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import time
 from typing import Callable, Optional
 
+logger = logging.getLogger("Rate timer")
+
 
 class RateTimer:
     """Iteration timer used to control the speed of a loop.
 
     The timer takes into account the time consumed by processed work
     and sleeps only for the time remaining to complete the iteration.
     Code is loosely inpired by ROS Rate object and by
@@ -70,15 +72,15 @@
 
         self.missed_iterations = 0
         self.times_called = 0
         self.creation_time = self.time_function()
         self.next_iteration_time = self.creation_time + self.total_iteration_time
 
         if self.verbose:
-            logging.info(f"RateTimer ({self.name}) created.")
+            logger.info(f"RateTimer ({self.name}) created.")
 
     def sleep(self) -> None:
         self.times_called += 1
 
         current_time = self.time_function()
         if current_time > self.next_iteration_time:
             # Processing took longer than defined iteration time. Do not sleep.
@@ -90,18 +92,18 @@
             else:
                 # Another possibility is to try to keep the old interval between the iterations as before miss
                 # (this may be problematic in case of larger time miss, because more iterations may then happen without sleep)
                 self.next_iteration_time += self.total_iteration_time
 
             miss_msg = f"RateTimer ({self.name}): Iteration missed."
             if self.iteration_miss_warning:
-                logging.warning(miss_msg)
+                logger.warning(miss_msg)
             else:
                 if self.verbose:
-                    logging.info(miss_msg)
+                    logger.info(miss_msg)
 
             # Do not perform any sleep
             return
 
         # time remaining to next iteration
         sleep_time = self.next_iteration_time - self.time_function()
         if sleep_time < 0:
@@ -122,25 +124,25 @@
 
 
 def rate_timer_example() -> None:
     """Example usage of RateTimer."""
 
     import random
 
-    logging.getLogger().setLevel(logging.INFO)
+    logger.setLevel(logging.INFO)
 
     rate = 2  # FPS
     iteration_time = 1.0 / rate
-    logging.info(f"Using rate timer with rate {rate} Hz ({iteration_time} s).")
+    logger.info(f"Using rate timer with rate {rate} Hz ({iteration_time} s).")
 
     # RateTimer should be created right before the loop starts
     rate_timer = RateTimer(rate, verbose=True, iteration_miss_warning=True)
 
     while True:
-        logging.info(f"Time is: {time.time()}")
+        logger.info(f"Time is: {time.time()}")
 
         # Generate random sleep time which is sometimes too long and forces iteration miss
         rand_time = random.uniform(iteration_time * 0.5, iteration_time * 1.1)
         time.sleep(rand_time)  # simulate work
 
         # Sleep until next interation
         rate_timer.sleep()
```

### Comparing `era_5g_interface-0.3.0/setup.py` & `era_5g_interface-0.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,16 +11,18 @@
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
     ],
     'description': 'An interface for 5G-ERA NetApps',
     'install_requires': (
-        'numpy~=1.24.4',
-        'opencv-python~=4.6.0.66',
+        'av>=10.0.0',
+        'numpy>=1.24.4',
+        'requests>=2.28.2',
+        'types-requests==2.31.0.1',
     ),
     'license': 'LGPL',
     'name': 'era_5g_interface',
     'namespace_packages': (
     ),
     'package_data': {
         'era_5g_interface': (
@@ -29,9 +31,9 @@
     },
     'packages': (
         'era_5g_interface',
         'era_5g_interface.dataclasses',
         'era_5g_interface.utils',
     ),
     'python_requires': '>=3.8,<3.11',
-    'version': '0.3.0',
+    'version': '0.4.0',
 })
```

