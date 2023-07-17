# Comparing `tmp/crjbsim-0.7.tar.gz` & `tmp/crjbsim-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crjbsim-0.7.tar", last modified: Mon Jan  9 15:48:16 2023, max compression
+gzip compressed data, was "crjbsim-1.0.tar", last modified: Mon Jul 17 10:45:02 2023, max compression
```

## Comparing `crjbsim-0.7.tar` & `crjbsim-1.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:48:16.649379 crjbsim-0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:48:16.645378 crjbsim-0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:48:16.645378 crjbsim-0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-01-09 15:48:08.000000 crjbsim-0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-09 15:48:08.000000 crjbsim-0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-01-09 15:48:16.649379 crjbsim-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-09 15:48:08.000000 crjbsim-0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-09 15:48:08.000000 crjbsim-0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-01-09 15:48:16.649379 crjbsim-0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:48:16.645378 crjbsim-0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:48:16.645378 crjbsim-0.7/src/crjbsim/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 15:48:08.000000 crjbsim-0.7/src/crjbsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-09 15:48:08.000000 crjbsim-0.7/src/crjbsim/des_aware_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-01-09 15:48:08.000000 crjbsim-0.7/src/crjbsim/discrete_event_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-09 15:48:08.000000 crjbsim-0.7/src/crjbsim/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-01-09 15:48:08.000000 crjbsim-0.7/src/crjbsim/time_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:48:16.645378 crjbsim-0.7/src/crjbsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-01-09 15:48:16.000000 crjbsim-0.7/src/crjbsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-09 15:48:16.000000 crjbsim-0.7/src/crjbsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 15:48:16.000000 crjbsim-0.7/src/crjbsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-09 15:48:16.000000 crjbsim-0.7/src/crjbsim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:48:16.645378 crjbsim-0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-01-09 15:48:08.000000 crjbsim-0.7/tests/test_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.910710 crjbsim-1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.906710 crjbsim-1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.910710 crjbsim-1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-17 10:44:52.000000 crjbsim-1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 10:44:52.000000 crjbsim-1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-17 10:45:02.910710 crjbsim-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 10:44:52.000000 crjbsim-1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-17 10:44:52.000000 crjbsim-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 10:44:52.000000 crjbsim-1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-17 10:45:02.910710 crjbsim-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.906710 crjbsim-1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.910710 crjbsim-1.0/src/crjbsim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/asncio_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/des_aware_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/discrete_event_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/time_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.910710 crjbsim-1.0/src/crjbsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-17 10:45:02.000000 crjbsim-1.0/src/crjbsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 10:45:02.000000 crjbsim-1.0/src/crjbsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:45:02.000000 crjbsim-1.0/src/crjbsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 10:45:02.000000 crjbsim-1.0/src/crjbsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.910710 crjbsim-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-17 10:44:52.000000 crjbsim-1.0/tests/test_asyncio_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-17 10:44:52.000000 crjbsim-1.0/tests/test_sim.py
```

### Comparing `crjbsim-0.7/setup.cfg` & `crjbsim-1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `crjbsim-0.7/src/crjbsim/des_aware_logging.py` & `crjbsim-1.0/src/crjbsim/des_aware_logging.py`

 * *Files identical despite different names*

### Comparing `crjbsim-0.7/src/crjbsim/discrete_event_scheduler.py` & `crjbsim-1.0/src/crjbsim/discrete_event_scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,22 @@
         return len(self._events)
 
 
 class Event:
     def __init__(self, time, runnable):
         self.time = time
         self.runnable = runnable
+        self.cancelled = False
 
     def execute(self):
-        self.runnable()
+        if not self.cancelled:
+            self.runnable()
+
+    def cancel(self):
+        self.cancelled = True
 
     def __repr__(self):
         return f"Event({self.time}, {self.runnable})"
 
 
 class DiscreteEventScheduler:
     def __init__(self):
@@ -46,11 +51,13 @@
             event = self._events.pop_next()
             assert event.time >= time_provider.get_time()
             time_provider.set_time(event.time)
             logger.debug(f"Executing event {event}")
             event.execute()
 
     def do_at(self, time, runnable):
-        self._events.add(Event(time, runnable))
+        event = Event(time, runnable)
+        self._events.add(event)
+        return event
 
     def do_in(self, time_delta, runnable):
-        self._events.add(Event(time_provider.get_time() + time_delta, runnable))
+        return self.do_at(time_provider.get_time() + time_delta, runnable)
```

