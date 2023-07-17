# Comparing `tmp/terminal_manager-0.8.1.tar.gz` & `tmp/terminal_manager-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.8.1.tar", last modified: Mon Jul 17 07:10:42 2023, max compression
+gzip compressed data, was "terminal_manager-0.8.2.tar", last modified: Mon Jul 17 08:30:40 2023, max compression
```

## Comparing `terminal_manager-0.8.1.tar` & `terminal_manager-0.8.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 07:10:42.107653 terminal_manager-0.8.1/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.8.1/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-17 07:10:42.107653 terminal_manager-0.8.1/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.8.1/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-17 07:09:42.000000 terminal_manager-0.8.1/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-17 07:10:42.107653 terminal_manager-0.8.1/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 07:10:42.099654 terminal_manager-0.8.1/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 07:10:42.103654 terminal_manager-0.8.1/src/terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7006 2023-07-17 07:02:19.000000 terminal_manager-0.8.1/src/terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/collection.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     6322 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/command.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 07:10:42.107653 terminal_manager-0.8.1/src/terminal_manager/default_collections/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/default_collections/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/default_collections/const.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4312 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/default_collections/linux.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/default_collections/windows_cmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5374 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/default_collections/windows_ps.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/event.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/helpers.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8387 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/sensor.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-17 06:20:45.000000 terminal_manager-0.8.1/src/terminal_manager/synchronizer.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 07:10:42.103654 terminal_manager-0.8.1/src/terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-17 07:10:42.000000 terminal_manager-0.8.1/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-17 07:10:42.000000 terminal_manager-0.8.1/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-17 07:10:42.000000 terminal_manager-0.8.1/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-17 07:10:42.000000 terminal_manager-0.8.1/src/terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-17 07:10:42.000000 terminal_manager-0.8.1/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:30:40.466247 terminal_manager-0.8.2/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.8.2/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-17 08:30:40.466247 terminal_manager-0.8.2/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.8.2/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-17 08:27:15.000000 terminal_manager-0.8.2/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-17 08:30:40.466247 terminal_manager-0.8.2/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:30:40.458247 terminal_manager-0.8.2/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:30:40.462247 terminal_manager-0.8.2/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7006 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     6322 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:30:40.466247 terminal_manager-0.8.2/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4359 2023-07-17 08:14:03.000000 terminal_manager-0.8.2/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5374 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/helpers.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8387 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:30:40.466247 terminal_manager-0.8.2/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-17 08:30:40.000000 terminal_manager-0.8.2/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-17 08:30:40.000000 terminal_manager-0.8.2/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-17 08:30:40.000000 terminal_manager-0.8.2/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-17 08:30:40.000000 terminal_manager-0.8.2/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-17 08:30:40.000000 terminal_manager-0.8.2/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.8.1/LICENSE` & `terminal_manager-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.1/PKG-INFO` & `terminal_manager-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal_manager
-Version: 0.8.1
+Version: 0.8.2
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.8.1/pyproject.toml` & `terminal_manager-0.8.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `terminal_manager-0.8.1/src/terminal_manager/__init__.py` & `terminal_manager-0.8.2/src/terminal_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.1/src/terminal_manager/collection.py` & `terminal_manager-0.8.2/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.1/src/terminal_manager/command.py` & `terminal_manager-0.8.2/src/terminal_manager/command.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.1/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.8.2/src/terminal_manager/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.1/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.8.2/src/terminal_manager/default_collections/linux.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,17 @@
                     SensorName.FREE_MEMORY,
                     SensorKey.FREE_MEMORY,
                     unit="KiB",
                 )
             ],
         ),
         SensorCommand(
-            'df -k | awk \'/^\\/dev\\// {x=$0; sub(/^[^ ]+( +[^ ]+){4} /,"",x); print x "|" $4}\'',
+            "df -k | awk '/^\/dev\// {"
+            + 'x=$0; sub(/^[^ ]+ +[^ ]+ +[^ ]+ +[^ ]+ +[^ ]+ /,"",x); '
+            + 'print x "|" $4}\'',
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     dynamic=True,
                     separator="|",
```

### Comparing `terminal_manager-0.8.1/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.8.2/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.1/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.8.2/src/terminal_manager/default_collections/windows_ps.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.1/src/terminal_manager/event.py` & `terminal_manager-0.8.2/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.1/src/terminal_manager/sensor.py` & `terminal_manager-0.8.2/src/terminal_manager/sensor.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.1/src/terminal_manager/synchronizer.py` & `terminal_manager-0.8.2/src/terminal_manager/synchronizer.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.1/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.8.2/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-manager
-Version: 0.8.1
+Version: 0.8.2
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.8.1/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.8.2/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

