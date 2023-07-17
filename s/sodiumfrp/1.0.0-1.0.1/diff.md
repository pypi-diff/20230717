# Comparing `tmp/sodiumfrp-1.0.0.tar.gz` & `tmp/sodiumfrp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sodiumfrp-1.0.0.tar", last modified: Tue Jul 19 15:00:08 2022, max compression
+gzip compressed data, was "sodiumfrp-1.0.1.tar", last modified: Mon Jul 17 05:51:39 2023, max compression
```

## Comparing `sodiumfrp-1.0.0.tar` & `sodiumfrp-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 mode      (1000) mode      (1000)        0 2022-07-19 15:00:08.504669 sodiumfrp-1.0.0/
--rw-r--r--   0 mode      (1000) mode      (1000)     1287 2022-07-19 15:00:08.504669 sodiumfrp-1.0.0/PKG-INFO
--rw-r--r--   0 mode      (1000) mode      (1000)      834 2022-07-19 14:59:04.000000 sodiumfrp-1.0.0/README.md
--rw-r--r--   0 mode      (1000) mode      (1000)       38 2022-07-19 15:00:08.504669 sodiumfrp-1.0.0/setup.cfg
--rw-r--r--   0 mode      (1000) mode      (1000)      806 2022-07-19 14:38:05.000000 sodiumfrp-1.0.0/setup.py
-drwxr-xr-x   0 mode      (1000) mode      (1000)        0 2022-07-19 15:00:08.504669 sodiumfrp-1.0.0/sodiumfrp/
--rw-r--r--   0 mode      (1000) mode      (1000)      214 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/__init__.py
--rw-r--r--   0 mode      (1000) mode      (1000)      956 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/lazy.py
--rw-r--r--   0 mode      (1000) mode      (1000)      960 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/listener.py
--rw-r--r--   0 mode      (1000) mode      (1000)     1503 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/node.py
--rw-r--r--   0 mode      (1000) mode      (1000)     2442 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/operational.py
--rw-r--r--   0 mode      (1000) mode      (1000)    39989 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/primitives.py
--rw-r--r--   0 mode      (1000) mode      (1000)        0 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/py.typed
--rw-r--r--   0 mode      (1000) mode      (1000)     6367 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/time.py
--rw-r--r--   0 mode      (1000) mode      (1000)     8659 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/transaction.py
--rw-r--r--   0 mode      (1000) mode      (1000)      225 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/typing.py
--rw-r--r--   0 mode      (1000) mode      (1000)       32 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/sodiumfrp/unit.py
-drwxr-xr-x   0 mode      (1000) mode      (1000)        0 2022-07-19 15:00:08.504669 sodiumfrp-1.0.0/sodiumfrp.egg-info/
--rw-r--r--   0 mode      (1000) mode      (1000)     1287 2022-07-19 15:00:08.000000 sodiumfrp-1.0.0/sodiumfrp.egg-info/PKG-INFO
--rw-r--r--   0 mode      (1000) mode      (1000)      571 2022-07-19 15:00:08.000000 sodiumfrp-1.0.0/sodiumfrp.egg-info/SOURCES.txt
--rw-r--r--   0 mode      (1000) mode      (1000)        1 2022-07-19 15:00:08.000000 sodiumfrp-1.0.0/sodiumfrp.egg-info/dependency_links.txt
--rw-r--r--   0 mode      (1000) mode      (1000)       16 2022-07-19 15:00:08.000000 sodiumfrp-1.0.0/sodiumfrp.egg-info/top_level.txt
-drwxr-xr-x   0 mode      (1000) mode      (1000)        0 2022-07-19 15:00:08.504669 sodiumfrp-1.0.0/tests/
--rw-r--r--   0 mode      (1000) mode      (1000)        0 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/tests/__init__.py
--rw-r--r--   0 mode      (1000) mode      (1000)      990 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/tests/memory1.py
--rw-r--r--   0 mode      (1000) mode      (1000)      798 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/tests/memory3.py
--rw-r--r--   0 mode      (1000) mode      (1000)      775 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/tests/memory4.py
--rw-r--r--   0 mode      (1000) mode      (1000)      692 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/tests/memory5.py
--rw-r--r--   0 mode      (1000) mode      (1000)    10717 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/tests/test_cell.py
--rw-r--r--   0 mode      (1000) mode      (1000)     3387 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/tests/test_common.py
--rw-r--r--   0 mode      (1000) mode      (1000)     6816 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/tests/test_stream.py
--rw-r--r--   0 mode      (1000) mode      (1000)     3415 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/tests/test_time.py
--rw-r--r--   0 mode      (1000) mode      (1000)      484 2022-07-19 14:34:26.000000 sodiumfrp-1.0.0/tests/test_transaction.py
+drwxr-xr-x   0 mode      (1000) mode      (1000)        0 2023-07-17 05:51:39.093912 sodiumfrp-1.0.1/
+-rw-r--r--   0 mode      (1000) mode      (1000)     3836 2023-07-17 05:51:39.093912 sodiumfrp-1.0.1/PKG-INFO
+-rw-r--r--   0 mode      (1000) mode      (1000)     3383 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/README.md
+-rw-r--r--   0 mode      (1000) mode      (1000)       38 2023-07-17 05:51:39.093912 sodiumfrp-1.0.1/setup.cfg
+-rw-r--r--   0 mode      (1000) mode      (1000)      806 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/setup.py
+drwxr-xr-x   0 mode      (1000) mode      (1000)        0 2023-07-17 05:51:39.091912 sodiumfrp-1.0.1/sodiumfrp/
+-rw-r--r--   0 mode      (1000) mode      (1000)      214 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/sodiumfrp/__init__.py
+-rw-r--r--   0 mode      (1000) mode      (1000)      956 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/sodiumfrp/lazy.py
+-rw-r--r--   0 mode      (1000) mode      (1000)      960 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/sodiumfrp/listener.py
+-rw-r--r--   0 mode      (1000) mode      (1000)     1503 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/sodiumfrp/node.py
+-rw-r--r--   0 mode      (1000) mode      (1000)     2442 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/sodiumfrp/operational.py
+-rw-r--r--   0 mode      (1000) mode      (1000)    39989 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/sodiumfrp/primitives.py
+-rw-r--r--   0 mode      (1000) mode      (1000)        0 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/sodiumfrp/py.typed
+-rw-r--r--   0 mode      (1000) mode      (1000)     6493 2023-07-17 05:50:39.000000 sodiumfrp-1.0.1/sodiumfrp/time.py
+-rw-r--r--   0 mode      (1000) mode      (1000)     8659 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/sodiumfrp/transaction.py
+-rw-r--r--   0 mode      (1000) mode      (1000)      225 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/sodiumfrp/typing.py
+-rw-r--r--   0 mode      (1000) mode      (1000)       32 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/sodiumfrp/unit.py
+drwxr-xr-x   0 mode      (1000) mode      (1000)        0 2023-07-17 05:51:39.092912 sodiumfrp-1.0.1/sodiumfrp.egg-info/
+-rw-r--r--   0 mode      (1000) mode      (1000)     3836 2023-07-17 05:51:39.000000 sodiumfrp-1.0.1/sodiumfrp.egg-info/PKG-INFO
+-rw-r--r--   0 mode      (1000) mode      (1000)      571 2023-07-17 05:51:39.000000 sodiumfrp-1.0.1/sodiumfrp.egg-info/SOURCES.txt
+-rw-r--r--   0 mode      (1000) mode      (1000)        1 2023-07-17 05:51:39.000000 sodiumfrp-1.0.1/sodiumfrp.egg-info/dependency_links.txt
+-rw-r--r--   0 mode      (1000) mode      (1000)       16 2023-07-17 05:51:39.000000 sodiumfrp-1.0.1/sodiumfrp.egg-info/top_level.txt
+drwxr-xr-x   0 mode      (1000) mode      (1000)        0 2023-07-17 05:51:39.093912 sodiumfrp-1.0.1/tests/
+-rw-r--r--   0 mode      (1000) mode      (1000)        0 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/tests/__init__.py
+-rw-r--r--   0 mode      (1000) mode      (1000)      990 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/tests/memory1.py
+-rw-r--r--   0 mode      (1000) mode      (1000)      798 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/tests/memory3.py
+-rw-r--r--   0 mode      (1000) mode      (1000)      775 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/tests/memory4.py
+-rw-r--r--   0 mode      (1000) mode      (1000)      692 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/tests/memory5.py
+-rw-r--r--   0 mode      (1000) mode      (1000)    10717 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/tests/test_cell.py
+-rw-r--r--   0 mode      (1000) mode      (1000)     3387 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/tests/test_common.py
+-rw-r--r--   0 mode      (1000) mode      (1000)     6816 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/tests/test_stream.py
+-rw-r--r--   0 mode      (1000) mode      (1000)     3905 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/tests/test_time.py
+-rw-r--r--   0 mode      (1000) mode      (1000)      484 2023-07-17 05:43:15.000000 sodiumfrp-1.0.1/tests/test_transaction.py
```

### Comparing `sodiumfrp-1.0.0/setup.py` & `sodiumfrp-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def get_long_description():
     with open("README.md", "r") as readme_file:
         return readme_file.read()
 
 setuptools.setup(
     name="sodiumfrp",
-    version="1.0.0",
+    version="1.0.1",
     author="Stephen Blackheath",
     description= \
         "Python implementation of Sodium - "
         "Functional Reactive Programming (FRP) library",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/mode89/sodium-python",
```

### Comparing `sodiumfrp-1.0.0/sodiumfrp/lazy.py` & `sodiumfrp-1.0.1/sodiumfrp/lazy.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/sodiumfrp/listener.py` & `sodiumfrp-1.0.1/sodiumfrp/listener.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/sodiumfrp/node.py` & `sodiumfrp-1.0.1/sodiumfrp/node.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/sodiumfrp/operational.py` & `sodiumfrp-1.0.1/sodiumfrp/operational.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/sodiumfrp/primitives.py` & `sodiumfrp-1.0.1/sodiumfrp/primitives.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/sodiumfrp/time.py` & `sodiumfrp-1.0.1/sodiumfrp/time.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 Timer = namedtuple("Timer", ["time", "streams"])
 
 class TimerSystem:
 
     def __init__(self) -> None:
         self._time_ms: CellSink[int] = CellSink(int(_now_ms()))
         self._timers: List[Timer] = []
+        # WARNING: running a transaction with _timers_changed locked
+        # may cause a deadlock
         self._timers_changed = Condition()
         self._stop = Event()
         self._released = False
 
         worker = Thread(target=self._thread)
         worker.daemon = True
         worker.start()
@@ -49,28 +51,30 @@
     def _thread(self) -> None:
         """
         Timers are executed at the beginning of a transaction. If there are
         not transactions, no timers will be executed. Thus, we need
         a separate thread that would generate transactions firing timers.
         """
         while not self._stop.is_set():
+            trigger_timers = False
             with self._timers_changed:
                 timeout = None
-                while self._timers:
+                if self._timers:
                     earliest_timer = self._timers[0]
                     now = _now_ms()
                     if earliest_timer.time > now:
                         timeout = (earliest_timer.time - now) * 0.001
-                        break
                     else:
-                        # If the time of the earliest timer has passed,
-                        # start an empty transaction to trigger all passed
-                        # timers through the transaction start hook
-                        Transaction.run(lambda: None)
-                self._timers_changed.wait(timeout)
+                        trigger_timers = True
+                if not trigger_timers:
+                    self._timers_changed.wait(timeout)
+            if trigger_timers:
+                # Start an empty transaction to trigger all passed timers
+                # through the transaction start hook
+                Transaction.run(lambda: None)
 
     def _on_transaction_start(self) -> None:
         """
         This should be used as a :meth:`Transaction.on_start()
         <sodiumfrp.transaction.Transaction.start>` hook. At the
         beginning of each transaction, update `self._time_ms` and execute
         all timers that should've been fired by this time.
```

### Comparing `sodiumfrp-1.0.0/sodiumfrp/transaction.py` & `sodiumfrp-1.0.1/sodiumfrp/transaction.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/sodiumfrp.egg-info/SOURCES.txt` & `sodiumfrp-1.0.1/sodiumfrp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/tests/memory1.py` & `sodiumfrp-1.0.1/tests/memory1.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/tests/memory3.py` & `sodiumfrp-1.0.1/tests/memory3.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/tests/memory4.py` & `sodiumfrp-1.0.1/tests/memory4.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/tests/memory5.py` & `sodiumfrp-1.0.1/tests/memory5.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/tests/test_cell.py` & `sodiumfrp-1.0.1/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/tests/test_common.py` & `sodiumfrp-1.0.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/tests/test_stream.py` & `sodiumfrp-1.0.1/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `sodiumfrp-1.0.0/tests/test_time.py` & `sodiumfrp-1.0.1/tests/test_time.py`

 * *Files 9% similar despite different names*

```diff
@@ -101,7 +101,21 @@
             return alarm.listen(out.append)
         l = Transaction.run(transaction)
         sleep(0.055)
         alarm_time.send(None)
         sleep(0.055)
         l.unlisten()
         assert len(out) == 0
+
+def test_thread_deadlock() -> None:
+    with TimerSystem() as ts:
+        out: List[int] = []
+        def init() -> None:
+            t0 = ts.time_ms().sample()
+            for i in range(1000):
+                alarm = ts.at(Cell.constant(t0 + 50 + int(0.1 * i)))
+                alarm.listen(out.append)
+        Transaction.run(init)
+        sleep(0.2)
+        # This test may fail occasionally, because there is no way to measure
+        # time precisely
+        assert len(out) == 1000
```

