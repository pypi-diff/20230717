# Comparing `tmp/urturn-0.1.4.tar.gz` & `tmp/urturn-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urturn-0.1.4.tar", last modified: Fri Jun 23 18:14:41 2023, max compression
+gzip compressed data, was "urturn-0.1.5.tar", last modified: Mon Jul 17 10:51:00 2023, max compression
```

## Comparing `urturn-0.1.4.tar` & `urturn-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:41.891628 urturn-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 18:14:30.000000 urturn-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-23 18:14:41.891628 urturn-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 18:14:30.000000 urturn-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:14:41.891628 urturn-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-23 18:14:30.000000 urturn-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:41.887628 urturn-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-23 18:14:30.000000 urturn-0.1.4/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-23 18:14:30.000000 urturn-0.1.4/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-23 18:14:30.000000 urturn-0.1.4/tests/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-23 18:14:30.000000 urturn-0.1.4/tests/test_webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:41.887628 urturn-0.1.4/urturn/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn/REQUIREMENTS
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:41.891628 urturn-0.1.4/urturn/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/templates/adapted.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/templates/details.css
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/templates/job_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:41.891628 urturn-0.1.4/urturn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:51:00.336634 urturn-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 10:50:46.000000 urturn-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 10:51:00.336634 urturn-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 10:50:46.000000 urturn-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 10:51:00.336634 urturn-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-17 10:50:46.000000 urturn-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:51:00.332635 urturn-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-17 10:50:46.000000 urturn-0.1.5/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-17 10:50:46.000000 urturn-0.1.5/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-17 10:50:46.000000 urturn-0.1.5/tests/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-17 10:50:46.000000 urturn-0.1.5/tests/test_webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:51:00.332635 urturn-0.1.5/urturn/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 10:51:00.000000 urturn-0.1.5/urturn/REQUIREMENTS
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 10:51:00.000000 urturn-0.1.5/urturn/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:50:46.000000 urturn-0.1.5/urturn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-07-17 10:50:46.000000 urturn-0.1.5/urturn/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-17 10:50:46.000000 urturn-0.1.5/urturn/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:51:00.336634 urturn-0.1.5/urturn/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-17 10:50:46.000000 urturn-0.1.5/urturn/templates/adapted.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-17 10:50:46.000000 urturn-0.1.5/urturn/templates/details.css
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-17 10:50:46.000000 urturn-0.1.5/urturn/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-17 10:50:46.000000 urturn-0.1.5/urturn/templates/job_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-17 10:50:46.000000 urturn-0.1.5/urturn/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-17 10:50:46.000000 urturn-0.1.5/urturn/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:51:00.336634 urturn-0.1.5/urturn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 10:51:00.000000 urturn-0.1.5/urturn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-17 10:51:00.000000 urturn-0.1.5/urturn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:51:00.000000 urturn-0.1.5/urturn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 10:51:00.000000 urturn-0.1.5/urturn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 10:51:00.000000 urturn-0.1.5/urturn.egg-info/top_level.txt
```

### Comparing `urturn-0.1.4/LICENSE` & `urturn-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `urturn-0.1.4/setup.py` & `urturn-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.4/tests/test_job.py` & `urturn-0.1.5/tests/test_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     pass
 
 
 class TestJobExecution(unittest.TestCase):
 
     def test_job_execution(self):
         # The command to be executed; here, we use "echo" to print a string.
-        cmd_args = ["echo", "Hello, World!"]
+        cmd_args = ["python", "-c", "print('Hello, World!')"]
 
         # Create a JobExecution instance with the command arguments.
         job_execution = JobExecution(
             'name', cmd_args, None, dummy_logging_callback, 50)
 
         # Start the job execution.
         job_execution.start()
@@ -88,15 +88,16 @@
         self.assertIsNotNone(job_execution.duration)
 
 
 class TestJobConfig(unittest.TestCase):
 
     def test_trigger_if_necessary(self):
         # The command to be executed; here, we use "echo" to print a string.
-        cmd_args = ["echo", "Test JobConfig", "&", "SLEEP", "1"]
+        cmd_args = ["python", "-c",
+                    "print('Hello, World!')", "&", "SLEEP", "1"]
 
         # Create a PeriodicTrigger instance with a very small time delta (e.g., 1 second).
         trigger = PeriodicTrigger(time_delta=timedelta(seconds=1))
 
         # Create a JobConfig instance with a name, command arguments, and trigger.
         job_config = JobConfig("Test Job", cmd_args,
                                trigger, None, dummy_logging_callback, 50, 50)
```

### Comparing `urturn-0.1.4/tests/test_scheduler.py` & `urturn-0.1.5/tests/test_scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
     def test_scheduler_job_trigger(self):
         # Create a periodic trigger that triggers every second
         trigger = PeriodicTrigger(timedelta(seconds=1))
 
         # Create a scheduler and add the mocked job config
         scheduler = Scheduler()
-        scheduler.add_job_config('myjob', ['echo', 'hello'], trigger)
+        scheduler.add_job_config(
+            'myjob', ["python", "-c", "print('hello')"], trigger)
 
         # Run the scheduler for a short duration (5 seconds) and then stop it
         scheduler_thread = Thread(target=scheduler.start)
         scheduler_thread.start()
         time.sleep(5)
         scheduler.stop()
         scheduler_thread.join()
@@ -31,15 +32,16 @@
     def test_scheduler_env(self):
         default_env = {"KEY1": "VALUE1", "KEY2": "VALUE2"}
         scheduler = Scheduler(env=default_env)
 
         trigger1 = PeriodicTrigger(timedelta(seconds=1))
 
         # This job config will use the default environment from the scheduler
-        scheduler.add_job_config("job1", ['echo', 'hello'], trigger1)
+        scheduler.add_job_config(
+            "job1", ["python", "-c", "print('hello')"], trigger1)
 
         # Run the scheduler for 10 seconds and then stop it
         scheduler_thread = Thread(target=scheduler.start)
         scheduler_thread.start()
         time.sleep(5)
         scheduler.stop()
         scheduler_thread.join()
@@ -49,15 +51,15 @@
         scheduler = Scheduler()
 
         trigger1 = PeriodicTrigger(timedelta(seconds=1))
 
         # This job config will use its own environment
         job1_env = {"KEY3": "VALUE3", "KEY4": "VALUE4"}
         scheduler.add_job_config(
-            "job1", ['echo', 'hello'], trigger1, env=job1_env)
+            "job1", ["python", "-c", "print('hello')"], trigger1, env=job1_env)
 
         # Run the scheduler for 10 seconds and then stop it
         scheduler_thread = Thread(target=scheduler.start)
         scheduler_thread.start()
         time.sleep(5)
         scheduler.stop()
         scheduler_thread.join()
@@ -102,15 +104,15 @@
 
     def test_max_executions(self):
         trigger = PeriodicTrigger(timedelta(seconds=1))
         scheduler = Scheduler()
 
         # Create a job config with max_executions limit set to 2
         scheduler.add_job_config(
-            'myjob', ['echo', 'hello'], trigger, max_executions=2)
+            'myjob', ["python", "-c", "print('hello')"], trigger, max_executions=2)
 
         # Run the scheduler for a short duration (10 seconds) and then stop it
         scheduler_thread = Thread(target=scheduler.start)
         scheduler_thread.start()
         time.sleep(10)
         scheduler.stop()
         scheduler_thread.join()
@@ -120,15 +122,15 @@
 
     def test_max_lines(self):
         trigger = PeriodicTrigger(timedelta(seconds=1))
         scheduler = Scheduler()
 
         # Create a job config with max_lines limit set to 3
         scheduler.add_job_config(
-            'myjob', ['echo', 'hello'], trigger, max_lines=3)
+            'myjob', ["python", "-c", "print('hello')"], trigger, max_lines=3)
 
         # Run the scheduler for a short duration (10 seconds) and then stop it
         scheduler_thread = Thread(target=scheduler.start)
         scheduler_thread.start()
         time.sleep(10)
         scheduler.stop()
         scheduler_thread.join()
@@ -140,15 +142,15 @@
 
     def test_max_executions_scheduler(self):
         trigger = PeriodicTrigger(timedelta(seconds=1))
         scheduler = Scheduler(max_executions=2)
 
         # Create a job config with max_executions limit set to 2
         scheduler.add_job_config(
-            'myjob', ['echo', 'hello'], trigger)
+            'myjob', ["python", "-c", "print('hello')"], trigger)
 
         # Run the scheduler for a short duration (10 seconds) and then stop it
         scheduler_thread = Thread(target=scheduler.start)
         scheduler_thread.start()
         time.sleep(10)
         scheduler.stop()
         scheduler_thread.join()
@@ -158,15 +160,15 @@
 
     def test_max_lines_scheduler(self):
         trigger = PeriodicTrigger(timedelta(seconds=1))
         scheduler = Scheduler(max_lines=3)
 
         # Create a job config with max_lines limit set to 3
         scheduler.add_job_config(
-            'myjob', ['echo', 'hello'], trigger)
+            'myjob', ["python", "-c", "print('hello')"], trigger)
 
         # Run the scheduler for a short duration (10 seconds) and then stop it
         scheduler_thread = Thread(target=scheduler.start)
         scheduler_thread.start()
         time.sleep(10)
         scheduler.stop()
         scheduler_thread.join()
```

### Comparing `urturn-0.1.4/tests/test_trigger.py` & `urturn-0.1.5/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.4/tests/test_webapp.py` & `urturn-0.1.5/tests/test_webapp.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.4/urturn/job.py` & `urturn-0.1.5/urturn/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,20 @@
             self.error_message = f"Command not found: {self.execution_cmd_args[0]}"
             self.return_code = -1
             return
 
         for line in io.TextIOWrapper(self.process.stdout, encoding="utf-8", errors='ignore'):
             yield line
 
-        self.return_code = self.process.wait()
+        poll_ret = None
+        while poll_ret is None:
+            poll_ret = self.process.poll()
+
+        self.return_code = self.process.returncode
+
         self.error_message = self.process.stderr.read().decode()
 
     def _trigger_and_log(self) -> None:
         """Execute the job, log its output lines, and measure its duration."""
         self.on_logging_event(JobEvent.STARTED, self.job_name)
 
         start_time = time.time()
```

### Comparing `urturn-0.1.4/urturn/scheduler.py` & `urturn-0.1.5/urturn/scheduler.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.4/urturn/templates/adapted.min.css` & `urturn-0.1.5/urturn/templates/adapted.min.css`

 * *Files identical despite different names*

### Comparing `urturn-0.1.4/urturn/templates/details.css` & `urturn-0.1.5/urturn/templates/details.css`

 * *Files identical despite different names*

### Comparing `urturn-0.1.4/urturn/templates/index.html` & `urturn-0.1.5/urturn/templates/index.html`

 * *Files identical despite different names*

### Comparing `urturn-0.1.4/urturn/templates/job_config.html` & `urturn-0.1.5/urturn/templates/job_config.html`

 * *Files identical despite different names*

### Comparing `urturn-0.1.4/urturn/trigger.py` & `urturn-0.1.5/urturn/trigger.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.4/urturn/webapp.py` & `urturn-0.1.5/urturn/webapp.py`

 * *Files identical despite different names*

